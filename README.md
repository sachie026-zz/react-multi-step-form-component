# react-multi-step-form-component

A NPM package which lets user add their personal components as a step


### Installation:

```JavaScript
npm install multi-step-form-ui 
or 
yarn add multi-step-form-ui
```

### Usage:

```JavaScript
import MultiSteps from "multi-step-form-ui";
```

```JavaScript
 <MultiSteps>
    <Component1 />
    <Component2 />
    <Component3/>
</MultiSteps>
```


You can pass your submit callback function in following way:

```JavaScript
 <MultiSteps submitForm = {`<your_submit_callback>`}>
    <Component1 />
    <Component2 />
    <Component3/>
</MultiSteps>
```

To mark the step as completd you have to call completed function in following way inside each component:

- To set step as incomplete `this.props.completed(this.props.stepindex, false)`
- To set step as complete `this.props.completed(this.props.stepindex, true)`

Here `this.props.stepindex` is mandatory paramater


You can set title for your step in following way:

```JavaScript
 <MultiSteps submitForm = {`<your_submit_callback>`}>
    <Component1 title = "Step1"/>
    <Component2 title = "Step1"/>
    <Component3/>
</MultiSteps>
```

Here title property is optional.



