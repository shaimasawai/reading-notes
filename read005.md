# *Putting it all together*
This part of the book pulls together everything covered in the previous chapters—styling, navigation, animations, and some of the cross-platform components—into a single app. We’ll start by looking at the final design and walking through a basic overview of what the app will do.

You’ll create a new React Native application and install the React Navigation library, dive deep into styling both the components as well as the navigation UI, work with data from external network resources by using the Fetch API, and ultimately build out an application that allows users to view information about their favorite Star Wars characters.
## *With A Mock*
Imagine that we already have a JSON API and a mock from our designer. The mock looks like this
Step 1: Break The UI Into A Component Hierarchy
The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!

Step 2: Build A Static Version in React
Now that you have your component hierarchy, it’s time to implement your app. The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. It’s best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing. We’ll see why.

Step 3: Identify The Minimal (but complete) Representation Of UI State
To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state.

Step 4: Identify Where Your State Should Live
Step 5: Add Inverse Data Flow
![](https://i.pinimg.com/originals/6a/bf/cc/6abfcce1fa6d8ef54f0b24ad08ae4c93.jpg)

