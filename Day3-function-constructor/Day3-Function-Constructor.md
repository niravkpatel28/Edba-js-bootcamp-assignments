## Day 3 : Random Expense Generator

In the exercise, the learner will practice the concept of using function
constructor for generating objects with consistent structure. The learner will
create following functions

1.  First function is a function constructor, named Expense. This function will
    generate an object of type Expense, with the following structure

    ```****

    const e1 = {
        // Use some unique id generator to create id for each expense
        // This id will be a string id: "Unique Expense Id",

        amount: Amount of expense,
        description: "Title or reason for expense",

        //This category will be a predefined list and category will be of type string
        category: "Category of expense",

        // Use Date JS object type for storing value
        date: Date of expense,

    }

    ```

    **Note: You can add additional properties based on your application
    requirement**

2.  Second function will be used for generating an array of random expenses. The
    function will take an integer as input and return a single array containing
    random expenses. The number of elements in this array is equal to the input
    integer. You can use any random logic to chose category of expense, amount
    and description.

    Hint: use [Faker.js](https://fakerjs.dev/guide/usage.html) to generate
    description and random amount.

For generating unique ids for each expense, the learner can use the following
function. In the function below `generateUniqueId({prefix:"exp"})` will generate
a unique id with prefix `"exp"`.

```
const generateUniqueId = (config = {}) => {
  // destructing
  const { prefix } = config;
  if (prefix) {
    return prefix + "-" + Math.random().toString(36).substring(2);
  }
  return Math.random().toString(36).substring(2);
};
```

This exercise is designed to help the learner understand the creation of objects
and importing external libraries for generating dummy data. Once this exercise
is done,the learner will be aware of "JavaScript Modules".
