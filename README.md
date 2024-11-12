We've got so many employees at this point that we need to start modularizing our employee management software. The important thing for this challenge is remembering that you may need to add to it later and will want to do minimal changes when that time comes.

## Step 1
Complete the `Employee` class. 
This class should have the following attributes:
- A String for an employee's name.
- A String for an employee's ID number.
- A double for an employee's salary.

It should also have the following methods:
- A no-arg constructor that sets name to "", ID to "" and salary to 0.0.
- An overload constructor that accepts and assigns name, ID, and salary.
- A setter and getter for name.
- A setter and getter for ID number.
- A setter and getter for salary.

## Step 2
Complete the `Astronaut` class.
This class should extend the Employee class and have the following attributes:
- A String for mission name.
- A String for mission role.

It should also have the following methods:
- A no-arg constructor that sets the mission name to "" and mission role to "" while also invoking super to create an associated employee object.
- An overload constructor that accepts and assigns name, ID, salary, mission name, and mission role while also invoking super with name, ID, and salary as arguments.
- A setter and getter for mission name.
- A setter and getter for mission role.

## Step 3
Complete the `EmployeeManager` class to create a new astronaut using the prompts provided in that file.

**Hint:** Remember, this needs to be modular. You will be asked to expand upon it later. Use inheritance to solve this challenge.

{Submit|assessment}(test-3455788452)
