`#My First Project`
`##Introduction`
Welcome to my first project it is a project mainly involving Java Script solving three challenges .This to help any developer in this three challenges.I hope to add more challenges in future.
Let us start with;Creating a repository from github account ;create a folder with three files for each solution
As we start of with this challenge.We will start by navigating to promp sync https://www.npmjs.com/package/prompt-sync install 
npm i prompt-sync then run it in your terminal to install prompt.then we can start of with our first challenge.

### Student Grade Generator
In this challenge we  are required to have a function that prompt the user to input student marks.Whereby the input should be  from 0-100 .The grade are when u have an A = greaater than 79 ,B = 60-79,C=59-49, D 40-49 ,E =less than 40,
*We start off by creating a js file e.g student.js 
*Then we crate a function e.g `studentGreading()`
 *then we create a variable for prompt using a function known as require
 `let prompt = require('prompt-sync')`
 *Now let us get input for the users
 we create
 `let marks = prompt('input your marks: ')`,
 *Still in the function we use conditional statements for grading g
 that is `if`.`else if`.`else`. 
 `if(marks > 79 && marks <= 100){`
     `   console.log('Your Grade is A');`
    `}`
    `else if(marks >= 60 && marks <= 79){`
     `   console.log("Your grade is B")`
    `}`
    `else if ( marks >= 49 && marks <=59){`
        `console.log('Your grade is C')`
    `}`
    `else if (marks >= 40 && marks <= 48){`
        `console.log('Your grade is D' )`
    `}`
    `else if (marks < 40 && marks >=0){`
        `console.log("Your grade is E")`
    `}`
    `else{`
        `console.log('Invalid marks');`
    `}`
    Then u can close the function
    *if u wish to call the function just run the function
    `studentGrading()`

#### Speed Detector
We are moving on quite well.
* for our second challenge make another file  like `speed.js` inside our folder
*we are required ;
 To write a program that takes the speed of a car as input e.g 80. If the speed is less than 70, it should print “Ok”. Otherwise, for every 5 km/s above the speed limit (70), it should give the driver one demerit point and print the total number of demerit points.

   For example, if the speed is 80, it should print: “Points: 2”. If the driver gets more than 12 points, the function should print: “License suspended”.
   In this challenge we are going  to start of with writing a variable to hold the speed limit (i.e)
   `const speedLimit=70`
   also for the demerit point
   `const demeritSpeed=5`
   like in challenge 1 we create a variable for prompt using a function
   `const prompt = require('prompt-sync)`
then 
    `const speed=prompt("what is the car speed: ")`
    we still use the conditional statements `if` . `else if`
    for the first one when the speed is <=70 the return should "OK"so we run
    `if (speed <= 70) {`
    `console.log('Ok');//returns ok if the limit ii 70 and below`
`}`
However,we need to get the number of points when its greater than 70 therefore we need an equation
to divide the speed will be divided to get the points
we will have to use the function `Math.floor()` to round off to the smallest number.We need to create a variable e.g 
`else {`
    `const points = Math.floor(((speed - speedLimit) / demeritSpeed))` calculate the number of Demerit Points then continue the if statement
    `if (points > 12)`
     `{ console.log('license suspended') }`returns license suspended if points are more than 12
    `else {`
        `console.log(`points:${points}` )`
    ``}` returns number of points if they are less than 12
`}`
##### License
MIT License

Copyright © 2023 Simon Nganga

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

`#####license`
MIT License

Copyright © 2023 Simon Nganga

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.