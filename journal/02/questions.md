# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > Var let const 

02. What is the definition of a function?

    > a block of code that defines a certain task 

03. What are the `SOLID` principles?

    > | ANSWER HERE |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > fruit = fruit.filter(item => item !== 'pineapple');

console.log(fruit);

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > function addFriends(person1, person2) {
    person1.friends.push(person2);
    person2.friends.push(person1);

06. Give an example of a JavaScript `Conditional`:

    > let x = 45;
if (x > 0) {
    console.log("wow");
} else {
    console.log("not big enough");
}

07. What is the main difference between `parameters` and `arguments`?

    > paramaters are used in a function and arguments are passed to a function 

08. Instead of writing everything to the console, what is a better way to debug your code?

    > debugger tools or console logging 

09. What is the difference between a `primitive` value and a `reference` value?

    > primatives hold an imutable value and reference objects are mutable 

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for (let i = -100; i <= 100; i++) {
    console.log(i);
