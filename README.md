# The Beginner's Guide to React

+ How babel works in the browser
+ Use React.Fragment to combine multiple elements for rendering
  - React.createElement(React.Fragment, null, element1, element2, element3, etc)
  - Use <>...<> as a shortcut
+ Use propTypes to validate properties. Don't need to use them if typing with typescript.
+ Using javascript expressions inside JSX using interpolation
+ Styling components
+ useState to maintain state
+ useEffect for data fetching, subscriptions, etc. immediately after render.
+ Pass a function to useState as default value to call it only once with this value.
+ eslint-plugin-react-hooks package will help maintain useEffect dependencies.
+ useRef to access mounted dom elements from within the component or track value of over time without re-rendering the component.
  - Use "ref" attribute on elements and useRef(<element ref>) to access it within the component.
  - Use in useEffect, return <instance>.destroy()
+ https://github.com/donavon/hook-flow
+ In forms, use "value" attribue to show value other than what user is typing.
+ ErrorBoundaries can be used to handle errors from the React call stack (render, useEffect). This allows for backup components in case of an error.
+ List elements must have a unique key for each item. Don't use index.
+ All async calls need to be in a useEffect()
+ Handling http request errors
+ Using React devtools to debug