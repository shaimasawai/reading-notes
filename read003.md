# *Passing Functions as Props*
![](https://dev.to/social_previews/article/133971.png)
### How do I pass an event handler (like onClick) to a component?
```<button onClick={this.handleClick}>```
### How do I bind a function to a component instance?
There are several ways to make sure functions have access to component attributes like this.props and this.state, depending on which syntax and build steps you are using.
```
class Foo extends Component {
  constructor(props) {
    super(props);
    this.handleClick = this.handleClick.bind(this);
  }
  handleClick() {
    console.log('Click happened');
  }
  render() {
    return <button onClick={this.handleClick}>Click Me</button>;
  }
}

```
![](https://cdn-media-1.freecodecamp.org/images/1*Rzaf_TyulUee7xEdDs3bRw.png)

### Passing Data Through Props
To get our feet wet, let’s try passing some data from our Board component to our Square component.

We strongly recommend typing code by hand as you’re working through the tutorial and not using copy/paste. This will help you develop muscle memory and a stronger understanding.

```
class Board extends React.Component {
  renderSquare(i) {
    return <Square value={i} />;
  }
}
```



