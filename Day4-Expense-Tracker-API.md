## Day 4 : REST API using Array

Array and Array functions

Working with Arrays and objects is an important skill for designing
applications. In this exercise you will create an array of expenes. Each item in
the "Expenses" array of is an Expense object. The expense object should have the
following structure

```
const e1 = {
    // Use some unique id generator to create id for each expense
    // This id will be a string
    id: "Unique Expense Id",

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

This array then becomes the source of data for creating following functions.

Write functions that will perform the following operation on the above array.

1. Find an expense with specific id. (id is the unique primary key for search)
   Example `findExpenseById(id: "1")` should return a single object from the
   array that has `"id = 1"`.

2. Write a function that will take input as "category" and return an object that
   contains an array with all the expenses under that category along with total
   expense incurred under that category. Example
   `findExpenseByCategory(category)` will return an object that will have the
   following structure

   ```
    {
      expenses: [Array containg all expenses with matching category],
      totalExpense: Sum of expenses with a matching category
    }

   ```

3. Update expense with a specific id. This function will take in arguments as id
   and an update object. Update object will contain a key value pairs that needs
   to be updated. eg. { category:  "updated  category" } Example
   `updateExpenseById(id: "1",{update Object: updated values})` should update a
   single object from the array that has `"id=1"`. Assume that the
   `updateObject` will contain keys that are present in the Expense object.
   **Restrict** updating key properties like `id`.

4. Delete an object with a specific id. This function should take in an argument
   as id and delete the same from the array of Expenses.

5. Write a function, that will take a date range and return the total expenses
   incurred in that duration

This exercise is designed to help learner understand Array functions. For
completing this assignment efficiently, learners are encouraged to read and
practice array functions before attempting to solve this. They should be
comfortable with using functions like

```
1. Array.prototype.find()
2. Array.prototype.filter()
3. Array.prototype.every()
4. Array.prototype.map()
```

The above function list is not an exhaustive list, but instead a list of
commonly used functions.
