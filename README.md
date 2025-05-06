## NSDLC & HDLC UML assignments 
## Basic Assignment: 
## Library Management System
## -> Class Diagram:
Classes & Attributes:
  Book:

    title: The name of the book.

    author: Name of the book's writer.

    ISBN: Unique identifier for the book.

    status: Availability status (e.g., borrowed, available).

  Member (inherits from Person):

    name: Full name of the member.

    memberID: Unique identifier for the member.

    borrowedBooks: List of books currently borrowed.

    borrowBook(Book): Method to borrow a book.

    returnBook(Book): Method to return a book.

  Librarian (inherits from Person):

    name: Full name of the librarian.

    librarianID: Unique identifier for the librarian.

    registerMember(Member): Method to register new members.

    addBook(Book): Method to add new books.

  Person (Superclass for Member & Librarian):

    name: Common attribute inherited by Member and Librarian.

Relationships:
Inheritance: Member and Librarian inherit attributes from Person.
This Class Diagram showcases key entities within the Library Management System. The Book, Member, and Librarian classes define the main functionalities of the system. The inheritance relationship between Person, Member, and Librarian ensures efficient data management. The associations illustrate interactions, such as borrowing books, registering members, and adding books to the collection.
![class diagram library](https://github.com/user-attachments/assets/477ecec1-d3eb-4afa-814e-1772c99a0a0e)

## -> Use Case Diagram:
Actors:
Member:Can borrow and return books.

Librarian:Registers new members.
Adds books to the collection.

Use Cases & Relationships:
Borrow Book (Member → System): Members can borrow books for up to 3 weeks.

Return Book (Member → System): Members return borrowed books.

Register Member (Librarian → System): Librarians register new members.

Add New Book (Librarian → System): Librarians add new books to the collection.
This Use Case Diagram visualizes the Library Management System’s primary functions, showing the interactions between Members and Librarians. Members borrow and return books, while Librarians manage books and register new users. The relationships between actors and use cases illustrate a clear workflow within the system.
![use case library](https://github.com/user-attachments/assets/8e2aaf00-944e-40b0-962c-80dcff3558e6)
