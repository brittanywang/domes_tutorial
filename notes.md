#H1 Components
A React component represents a piece of the page as shown below. Each component is a Javascript function that returns a piece of code that represents a piece of a web page. To build the page, we call these functions in a certain order and then it is shown to the user.  
![components](https://user-images.githubusercontent.com/35832643/41438251-837689ec-6fdb-11e8-8752-b5fb2344fc24.png)

Functions can be written as:
```
<script type="text/babel">
  function MyComponent = (props) => {
    return (
      <elementOrComponent .../>
    );
  }
  const placeWeWantToPutComponent = document.getElementById('hook');
  ReactDOM.render(<MyComponent />, placeWeWantToPutComponent);
</script>

```

The function component receives an object of properties which is usually named props. It returns JSX, or JavaScript syntax. Function components cannot have state. A class component is a more featured way to define a React component because it acts like a function that receives props.


#H1 Talking Between Components
`Props` are used as a way for components to interact with one another (from parent to child component). For instance, we can tell the `PlayButton` if music is playing or not.  
