1. When would you use a Class Component over a Functional Component?
  * If your component has state or a lifecycle method, user a Class component. Otherwise, use a Functional component.
2. What are refs?
  * Used to return a reference to the element, for example, value of an input
  * Useful when we need DOM measurements or to add methods to the components
  * Not so good because... It moves away from the "React" way of thinking.
  * [Refs in React - All you need to know](https://hackernoon.com/refs-in-react-all-you-need-to-know-fb9c9e2aeb81)
3. Controlled vs. Uncontrolled components
  * controlled -
    - gets values through props.
    - notifies parent component of changes through callbacks
    - parent handles callback and manages state, then passes new values as props to controlled component
    - AKA "dumb component"
  * uncontrolled -
     - stores its own state internally
     - query DOM using ref to fing current value
  * [controlled vs uncontrolled inputs](https://goshakkk.name/controlled-vs-uncontrolled-inputs-react/#conclusion)
  * [controlled vs uncontrolled components](https://www.sitepoint.com/video-controlled-vs-uncontrolled-components-in-react/)
4. What are Lifecycle methods?
  * everything that happens from before a component mounts (pre-mounting) to unmounting.
  * componentWillMount: can’t do anything will dom because before render
  * componentdidmount: after component mounts. add event listeners
  * componentWillReceiveprops: gets new props from parent component. You can check which props will change, you can act on new props
  * shouldComponentUpdate: always returns boolean. should i re-render?
  * componentWillUpdate: no access to previous props, but used to take action when shouldcomponentupdate is present.
  * componentDidUpdate: update DOM in response to prop or state changes
  * componentWillUnmount: last min requests before component goes away. clean up leftover debris
  * [react lifecycle methods](https://engineering.musefind.com/react-lifecycle-methods-how-and-when-to-use-them-2111a1b692b1)
5. What are Higher Order Components?
  * Wraps other components and passes data into it
  * [HOC in depth](https://medium.com/@franleplant/react-higher-order-components-in-depth-cf9032ee6c3e)
6. Pros and cons of using React?
  * Performant
  * Reusability
  
