## Functional VS Class Components
🎥 [7 mins video](https://www.youtube.com/watch?v=wwl6iH5D0LU)
### Functional Component
Example:
```
import React, {useState} from "react";

const FunctionalComponent=()=>{
    const[count , setCount]=useState(0);
 
    const increase=()=>{
        setCount(count+1);
    }
 
    return
        <div style={{margin:'50px'}}>
            <h1>Welcome to Geeks for Geeks </h1>
            <h3>Counter App using Functional Component : </h3>
          <h2>{count}</h2>
            <button onClick={increase}>Add</button>
        </div>
    )
} 
 
 
export default FunctionalComponent;
```
- plain JS function that takes in `props` as argument and `returns` an element
- in the past, functional components do not allow you to manage the state
- now, things are different, React provides us [Hooks](https://github.com/chienleow/react-notes#hooks) - gives us features a class component would have
- example: `useState`, `useEffect`



### Class Component
Example:
```
import React from "react";
 
class ClassComponent extends React.Component{
    constructor(){
        super();
        this.state={
            count :0
        };
        this.increase=this.increase.bind(this);
    }
     
   increase(){
       this.setState({count : this.state.count +1});
   }
 
    render(){
        return (
            <div style={{margin:'50px'}}>
               <h1>Welcome to Geeks for Geeks </h1>
               <h3>Counter App using Class Component : </h3>
               <h2> {this.state.count}</h2> 
               <button onClick={this.increase}> Add</button>
 
            </div>
        )
    }
}
 
export default ClassComponent;
```
- requires to extend from React, creates a `render` function which `returns` an element.
- comes with `constructor`, use to set up initial state
- you can manage the state of your component, `setState` allows you to hold the data throughout the life cycle of the component
- gives you access to "lifecycle functions" - functions that are invoked during the lifecycle of a component
- 
