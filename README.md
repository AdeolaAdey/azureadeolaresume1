# azureadeolaresume1
My azure resume from project [video by ACG.](https://www.youtube.com/watch?v=ieYrBWmkfno)

## My First Steps
- frontend folder contains code for the static web app
-main.js contains visitor counter code
```js
const getVisitCount = () => {
    let count = 30;
    fetch(functionApi).then(response =>{
        return response.json()
    }).then(response=>{
        console.log("Website called function API");
        count = response.count;
        document.getElementById("counter").innerText = count;
    }).catch(function(error){
        console.log(error);
    });
    return count;

```

## Step 2: Creating A Functions

- aloows us to create peices of code that are event driven. wont have to worry about the infrastructure behind the code.
- Has things called bindings that allows to connect for other resources to the functions.
-I must create a function and connect the azure cosmos DB bindings to the function that I made.