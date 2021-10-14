# Library API

The API for a non-existent library.

### Book

Each book is an entity with the following information:

- author
- name of the book
- annotation
- genre (drama, detective etc., maybe several)

Also, translated books must contain additional fields:

- author in original language
- title in original language

Subscribers can take most of the books with them from the library to read them at home, but some of them are read-only in the reading room.

### Subscriber

Each library subscriber is an entity with the following information:

- name
- surname
- address

Each subscriber can take up to 10 books to the reading room and a maximum of 3 books with him from the library, but for a maximum of 30 seconds (conditionality of the problem). For every minute of delay, a fine is imposed on each expired book: for 20 seconds, the subscriber cannot take a single book at all.

### UI

The UI for a subscriber should allow:

- enter the library
- exit the library
- see a list of available books (it should be presented as a searchable sorted and filtered table)
- take a book to read in the reading room or with you

The UI for the administrator of library should allow:

- see a list of subscribers, with the ability to create and delete
- the ability to impose fines on the user or vice versa clearing him of them
- see a table of references with the ability to create and delete

### API

API for the library must be implemented according to the rules and requirements of REST
