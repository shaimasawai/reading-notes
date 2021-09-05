React.js is one of the most widely used JavaScript libraries that every front-end developer should know. Understanding what props and state are and the differences between them is a big step towards learning React.

# *What are props?*

Props is short for properties and they are used to pass data between React components. React’s data flow between components is uni-directional (from parent to child only).

# *How do you pass data with props?*

Here is an example of how data can be passed by using props:
```
class ParentComponent extends Component {    
    render() {    
        return (        
            <ChildComponent name="First Child" />    
        );  
    }
}

const ChildComponent = (props) => {    
    return <p>{props.name}</p>; 
};
```
# *What is state?*
React has another special built-in object called state, which allows components to create and manage their own data. So unlike props, components cannot pass data with state, but they can create and manage it internally.
```
class Test extends React.Component {    
    constructor() {    
        this.state = {      
            id: 1,      
            name: "test"    
        };  
    }    
    
    render() {    
        return (      
            <div>        
              <p>{this.state.id}</p>        
              <p>{this.state.name}</p>      
            </div>    
        );  
    }
}
```
# *What are the differences between props and state?*
    1- ponents receive data from outside with props, whereas they can create and manage their own data with state
    
    2- ps are used to pass data, whereas state is for managing data
    
    3- a from props is read-only, and cannot be modified by a component that is receiving it from outside
    
    4-data can be modified by its own component, but is private (cannot be accessed from outside)
    
    5- ps can only be passed from parent component to child (unidirectional flow)
    
    6- ifying state should happen with the setState ( ) method
    
![](https://res.cloudinary.com/practicaldev/image/fetch/s--xKWyj8SG--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/http://live-linguine-code.pantheonsite.io/wp-content/uploads/2019/03/react-state-vs-props.jpg)
