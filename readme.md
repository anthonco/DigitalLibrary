# Digital Library JavaScript Class

Created by Corey Anthony

## Points for discussion during code review:

Bind event on delete checkbox quits working when table rows deleted and table is updated.  Had to redo the bind event in the function that updates the row to re-attach it.  So it is bound wwhen the buttons are created and not in the custom bind events method.  Is there a better way?

Kyle suggested a delegation so that when the table changes it re-binds the buttons.

Created keys on each td to reference with find so that adjusting columns is completely detached (not hard) coded

## UI Classes:

UI super classes that prototype Library

```
ShowAuthorsUI
AddBooksUI
```
## Features:
-Node server and CRUD routes are in use
-Async/await used when books are updated
-Table headers are pulled from the book property names
-jQuery init(), bindEvents(), and eventHandlers()
-Local Storage
-Singleton design pattern
-observer design pattern
-Mongodb using mLabs mongo database in cloud
-custom event handlers updates the table when changes are made
-form serialization is used from add books form into the book object.  Local storage and dynamic table generation will automatically compensate if a new data point is added.  The only changes needed are adding a field to the add books form and adding a property to the books class.
-event properties are used to change the behavior of the search button to toggle between search results and default book listing on the books table.

## Tools used:
Atom IDE - for code editor
Postman - for sending requests to Mongodb
Robo 3T - for administering mLabs mongodb instance
Node server - ReST layer
Git/Git Hub - Code repository
Sourcetree - Git repository management

## Other:
