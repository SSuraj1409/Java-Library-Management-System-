# 📚 Library Management System

## 🧾 Introduction

The Library Management System, developed with JavaFX and SceneBuilder, is a user-friendly platform designed to automate administrative tasks within libraries. It includes functions such as adding and deleting books, managing members, and handling issuing and returning processes.

---
## 🧠 Programming Concepts and Structures Used

This project incorporates several important Java and JavaFX concepts to ensure modularity, usability, and scalability:

### 1. JavaFX
- JavaFX is used for building the graphical user interface (GUI) of the application.
- It provides classes and APIs for creating UI components, handling user events, and managing scene graphs.
- In the `IssueBookController`, annotations such as `@FXML` are used to inject references to UI components defined in the corresponding FXML file.

### 2. FXML and SceneBuilder
- FXML files located in the `view` package define the structure and layout of UI components using XML.
- These FXML files are loaded by the `FXMLLoader` to create the UI hierarchy at runtime.
- **SceneBuilder** is used as a drag-and-drop visual tool to design FXML layouts efficiently and clearly.

### 3. MVC (Model-View-Controller) Architecture
- The project follows the MVC design pattern:
  - **Model**: Represents the data (e.g., `Book` objects).
  - **View**: Defined using FXML files for layout and styling.
  - **Controller**: Manages the interaction between the user and the system (e.g., `BooksController`, `IssueBookController`).
- Each controller acts as a mediator between the UI elements and the underlying data model.

### 4. File I/O
- File input/output operations are used for data persistence.
- `loadDataFromFile()` reads book data from a file (e.g., `books.txt`), while `handleSaveBooks()` exports updated book data back to the file.

### 5. Collections
- Java collections such as `ArrayList<Book>` and `Vector<Book>` are used to store and manage lists of books.
- `FXCollections.observableArrayList()` is used to create observable lists that bind to JavaFX TableView components for dynamic UI updates.

### 6. Exception Handling
- The program uses `try-catch` blocks to handle potential exceptions.
- Proper error messages are shown to the user to ensure a smoother user experience during file read/write or invalid input scenarios.

### 7. Event Handling Structure
- JavaFX's event handling model is used to respond to user actions.
- Controller methods are annotated with `@FXML` and tied to events like button clicks and text input actions.
- This ensures clear interaction between the UI and underlying logic.

---
## 📊 Flowchart


---

## 📸 GUI Preview

<p align="center">
  <img src="images/library_gui.png" alt="Library Management GUI" width="500"/>
</p>

> ⚠️ Make sure to upload your `library_gui.png` screenshot into an `images` folder in your repo.

---

## 📂 Project Structure

