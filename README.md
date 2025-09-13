# Java-Task
📚 Library Management System

This is a simple Java-based Library Management System that demonstrates the use of OOP concepts, interfaces, and JUnit testing.

The project allows:

Adding books to a library collection.

Borrowing (issuing) and returning books.

Checking book availability.

Running unit tests to validate functionality.

🚀 Features

Interface Issueable
Defines the contract for borrowing and returning books.

Class Book
Implements Issueable. Contains book details like title, author, ISBN, and availability status.

Class Library
Maintains a collection of books, allows borrowing, returning, and checking library size.

JUnit Tests (LibraryUnitTests)
Tests the borrowing, returning, and availability functionality.

📂 Project Structure
library-management/
│
├── src/
│   └── library/
│       ├── Issueable.java      # Interface defining borrow/return contract
│       ├── Book.java           # Book class implementing Issueable
│       ├── Library.java        # Library class to manage collection
│       └── LibraryUnitTests.java # JUnit test cases
│
└── README.md                   # Project documentation

⚙️ How It Works

Include a Book

libraryInstance.includeBook(new Book("Book Title", "Author", "ISBN-001"));


Borrow a Book

libraryInstance.borrowBook("ISBN-001"); 
// Returns "Publication checkout successful" if available


Return a Book

libraryInstance.bringBackBook("ISBN-001"); 
// Returns "Return Successful" if previously borrowed


Check Collection Size

libraryInstance.collectionSize();

🧪 Running Tests

The project uses JUnit 5 for testing.

Run with Maven
mvn test

Run in VS Code / IntelliJ IDEA

Right-click on LibraryUnitTests.java

Select Run Tests

✅ Sample Output (from tests)

Borrowing a book → Publication checkout successful

Returning a book → Return Successful

Borrowing an unavailable book → Publication currently unavailable

Returning a non-existent book → Publication not in collection

🛠️ Requirements

Java 8 or later

JUnit 5

Maven/Gradle (optional for build & test automation)

👨‍💻 Author

Developed as a practice project for Object-Oriented Programming (OOP) in Java and Unit Testing.
