﻿# Student System Migration in C++

This project is focused on migrating an existing student management system to a new platform using C++. The objective is to implement and extend the functionality of the current system to manage a roster of students within a specific course. The system is designed with two primary classes: `Student` and `Roster`.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Technical Details](#technical-details)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The Student System Migration project is a C++ application that maintains a roster of students. The system allows for the manipulation and retrieval of student data, including the addition, removal, and listing of students. This project serves as a practical example of object-oriented programming principles in C++, focusing on class design, data encapsulation, and dynamic memory management.

## Features

- **Student Class:**
  - Manages student information including ID, first name, last name, email, age, days to complete each course, and degree program.
  - Provides accessor and mutator methods for secure data handling.
  - Includes a method to print student details in a formatted output.

- **Roster Class:**
  - Maintains a dynamic array of student objects.
  - Supports operations such as adding and removing students, printing the full roster, calculating and displaying average days in course, and validating email addresses.
  - Filters and prints students based on their degree program.

## Installation

To run this project, ensure you have a C++ compiler and an integrated development environment (IDE) installed on your system.

1. Clone the repository:
   ```bash
   git clone https://github.com/selvawen/student-system-migration.git

2. Open the project in your IDE.

3. Compile the project:
```bash
g++ main.cpp student.cpp roster.cpp -o StudentSystem
```
4. Run the executable:
```bash
./StudentSystem
```

### Usage
The application reads student data from a predefined array, parses it, and populates the `classRosterArray` with `Student` objects. The main function then demonstrates various operations such as printing all students, removing a student by ID, and listing students by degree program.

### Example Function Calls:
```cpp
classRoster.printAll();
classRoster.printInvalidEmails();
classRoster.printAverageDaysInCourse("A1");
classRoster.printByDegreeProgram(SOFTWARE);
classRoster.remove("A3");
```

### File Structure

The project consists of six source files:

- `degree.h` – Contains the `DegreeProgram` enumeration.
- `student.h` and `student.cpp` – Define and implement the `Student` class.
- `roster.h` and `roster.cpp` – Define and implement the `Roster` class.
- `main.cpp` – Contains the `main` function and demonstrates the program’s functionality.

## Technical Details

- **Language:** C++
- **IDE:** Compatible with any C++ IDE
- **Memory Management:** The `Roster` class implements a destructor to manage dynamic memory.

### Key Concepts:
- **Object-Oriented Design:** Encapsulation, inheritance, and polymorphism.
- **Dynamic Memory Allocation:** Handling student data using pointers and arrays.
- **Data Parsing:** Extracting and manipulating data from a structured format.

## Screenshots

Include screenshots demonstrating the console output and program functionality.

![Screenshot_29 (1)](https://github.com/user-attachments/assets/e91b4edb-637a-4f87-b721-1ed32398947f)

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. Make sure to follow the coding standards and include appropriate tests.

## License

MIT License

Copyright (c) 2024 Benjamin Anderson

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
