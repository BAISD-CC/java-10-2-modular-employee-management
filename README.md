We've got so many employees at this point that we need to start modularizing our employee management software. The important thing for this challenge is remembering that you may need to add to it later and will want to make minimal changes when that time comes. To do this, you'll split employee data into a general `Employee` class and a more specific `Astronaut` class that **inherits** from it.

## Step 1

Complete the `Employee` class (`src/Employee.java`).

This class should have the following attributes:
- A `String` for an employee's name.
- A `String` for an employee's ID number.
- A `double` for an employee's salary.

It should also have the following methods:
- A no-arg constructor that sets name to `""`, ID to `""`, and salary to `0.0`.
- An overload constructor that accepts and assigns name, ID, and salary.
- A setter and getter for name (`setName`, `getName`).
- A setter and getter for ID number (`setID`, `getID`).
- A setter and getter for salary (`setSalary`, `getSalary`).

## Step 2

Complete the `Astronaut` class (`src/Astronaut.java`).

This class should **extend** the `Employee` class and have the following attributes:
- A `String` for mission name.
- A `String` for mission role.

It should also have the following methods:
- A no-arg constructor that sets mission name to `""` and mission role to `""`, while also invoking `super()` to build the associated `Employee` part of the object.
- An overload constructor that accepts and assigns name, ID, salary, mission name, and mission role, while also invoking `super(...)` with name, ID, and salary as arguments.
- A setter and getter for mission name (`setMissionName`, `getMissionName`).
- A setter and getter for mission role (`setMissionRole`, `getMissionRole`).

Because `Astronaut` extends `Employee`, it does **not** redeclare name, ID, or salary — those come from `Employee`.

## Step 3

Complete the `EmployeeManager` class (`src/EmployeeManager.java`) to create a new astronaut using the prompts already listed in that file:

- `Enter the astronaut's name: `
- `Enter the astronaut's ID: `
- `Enter the astronaut's salary: `
- `Enter the astronaut's mission name: `
- `Enter the astronaut's mission role: `

Read each value with a `Scanner`, then:

1. Create an `Astronaut` object with the overload constructor, using the five values entered by the user.
2. Create a second `Astronaut` object with the no-arg constructor, just to confirm that constructor works too. You do not need to display this second object's data.
3. Display the first astronaut's data (the one built from user input) using its getter methods, in exactly this format, one item per line:

```
Name: [name]
ID: [ID]
Salary: [salary]
Mission Name: [missionName]
Mission Role: [missionRole]
```

### Example run

```
Enter the astronaut's name: Buzz Aldrin
Enter the astronaut's ID: AST001
Enter the astronaut's salary: 100000.0
Enter the astronaut's mission name: Apollo 11
Enter the astronaut's mission role: Lunar Module Pilot
Name: Buzz Aldrin
ID: AST001
Salary: 100000.0
Mission Name: Apollo 11
Mission Role: Lunar Module Pilot
```

Your program will be tested with several different astronauts, not just the one shown above, so make sure your output always reflects whatever the user actually typed in rather than these exact example values.

**Hint:** Remember, this needs to be modular. You will be asked to expand upon it later. Use inheritance to solve this challenge.

{Submit|assessment}(test-3455788452)
