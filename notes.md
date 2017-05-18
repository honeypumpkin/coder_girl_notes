# JAVASCRIPT    
Building blocks
- arrays
- variables
- objects
- functions
- loops
- conditionals

## Object oriented programming
1. will reduce and reuse
1. makes it scaleable and maintainable

### *Classes*:
The point of classes is to *encapsulate* all the functionality around one object
___
Example of using OOP:
``` js
//creating a printout of students with address and info//
function Student (lastName, firstName, email){
    this.lastName = lastName;
    this.firstName = firstName;
    this.email = email;
    this.major = "Undecided";
    this.photo = "";
    this.grades = [];
    
}

Student.prototype = {
    constructor: Student,
    addGrade: function (grade){
        this.grades.push(grade);
    },
    totalGrade: function (){
        var sum = 0;
        for (var i = 0; i < this.grades.length; i++){
            sum += this.grades [i];
        }
        return (sum / this.grades.length) * 100;
    },
    changeEmail: function (newEmail){
        this.email = newEmail;
    },
    fullName; function () {
        return this.lastName + ", " + this.firstName;
    }
}

var student1 = new Student ("Mathews:, "Katie", "email@gmail.com");

```

OBJECTS
___
properties: 
- last name (str)
- first name (str)
- email (str)
- major (str)
- photo (file source)
- grades [array]

actions/functions/methods:
- add grade
- total grade
-


