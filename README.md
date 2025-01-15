# HBnB Version 1

## AirBnB Clone: The Console

**Group Project**
- **Python OOP**
- **Team Members:**
  - Ojotule Attah
  - Eddy UWAMBAJE

This project is a team effort with a manual QA review required upon completion. An auto review will be initiated at the project deadline.

---

### Concepts
For this project, we expect you to understand and apply the following concepts:
- **Python Packages**
- **Object-Oriented Programming**
- **Serialization and Deserialization**

---

## Project Description

The **HBnB console** is a command-line interpreter for managing AirBnB objects. It includes the following features:
- Creation of all classes for AirBnB (e.g., `User`, `City`, `Place`) inheriting from a `BaseModel`.
- A class to handle initialization, serialization, and deserialization of instances.
- An abstracted storage engine for managing data.
- Unit tests to validate all classes and the storage engine.

---

## How to Use

### Interactive Mode
```bash
$ ./console.py
(hbnb) help
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
(hbnb)
(hbnb) quit
$
```

### Non-Interactive Mode
```bash
$ echo "help" | ./console.py
(hbnb)
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```

---

## Console Commands

### Command Descriptions:
- **`quit`**: Exit the program.
- **`EOF`**: Exit the program using `CTRL + D`.
- **Empty Line**: No action is taken when pressing `ENTER` on an empty line.
- **`create`**: Create a new object (e.g., a new `User` or a new `Place`).
- **`show`**: Display the string representation of an instance based on its class name and ID.
- **`destroy`**: Delete an instance based on its class name and ID.
- **`all`**: Display string representations of all instances or instances of a specific class.
- **`update`**: Update attributes of an object.

---

## Directory and File Descriptions

- **`models/`**: Contains all models used in the AirBnB clone project.

  - **`models/engine/file_storage.py`**: Handles serialization and deserialization of Python objects to and from a JSON file.
  - **`models/base_model.py`**: The base class for all models. Includes methods for converting an object to a dictionary and saving it to the storage engine.
  - **`models/city.py`**, **`amenity.py`**, **`place.py`**, **`review.py`**, **`state.py`**, **`user.py`**: Define different entities inheriting from `base_model.py`. Each file serves a specific purpose as suggested by its name.

- **`console.py`**: The command-line interpreter used to perform CRUD operations on the models.
- **`AUTHORS`**: A list of all contributors to the repository.

---

## Authors

- Ojotule Attah
- Eddy UWAMBAJE
