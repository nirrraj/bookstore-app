A sample app that stores one resource, books! A book object follows the standard schema:

```
{
  "isbn": "0691161518",
  "amazon_url": "http://a.co/eobPtX2",
  "author": "Matthew Lane",
  "language": "english",
  "pages": 264,
  "publisher": "Princeton University Press",
  "title": "Power-Up: Unlocking the Hidden Mathematics in Video Games",
  "year": 2017
}
```

Routes:
---
GET /books

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Responds with a list of all the books

POST /books

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Creates a book and responds with the newly created book

GET /books/[isbn]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Responds with a single book found by its isbn

PUT /books/[isbn]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Updates a book and responds with the updated book

DELETE /books/[isbn]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Deletes a book and responds with a message of “Book deleted”

Features:
---
Uses JSONSchema to validate the creation and updating of a product. Displays an error message containing all of the validation errors if book creation or updating fails.

Integration tests
