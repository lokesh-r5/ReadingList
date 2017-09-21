Reading List Application using Angular JS

Installation instructions:

To run the app, clone this repository and run the following:

1. "npm install"
2. "bower install"
3. "grunt serve"

Broser will be opened and run http://localhost:3000. If not enter http://localhost:3000 in the browser.

App usage instructions:

### When you have read or want read a Book, you can add it to a Reading List so that you won't forget about it.

A Book should have:

* **title** - a text field
* **authors** - a list of names
* **ain** - the AIN from Amazon.com (optional)
* **review** - a few paragraphs of text
* **rating** - 1 to 5, like stars (or tomatoes)
* **genre** - a name like "fiction" or "non-fiction"

### You can view a list of all the Books on my Reading List so that you can see which ones you have added.

* For each Book, show:
    * the cover image (from Amazon.com)
    * rating (out of max)
    * the title
    * author byline
    * review text
    * genre(s)
* Link to Amazon.com:
    * the cover image
    * the title
* Display in the order they were added to the Reading List
* The URL for a book cover image from Amazon.com can be generated, given the AIN:
    http://images.amazon.com/images/P/{{book.ain}}.01.ZTZZZZZZ.jpg
* The URL for a book on Amazon.com can be generated, given the AIN:
    http://www.amazon.com/gp/product/{{book.ain}}

### You can edit a Book on my Reading List so that you can add or update the information about it.

* Essentially opens the "New Review" form for the existing Book

### You can mark a Book as "READ" or "READING" so that you can remind myself which ones you have already read.

Add **currently** to Book, a state indicator of "UNREAD", "READ" or "READING"

Reminders:

* Don't forget to update the "Edit Book" form!
* Maybe provide an easier way to update than editing it?

### You can _sort_ the list of Books so that you can see which ones to read next.

The list of Books can be _sorted_ by:

* date added e.g. oldest to newest
* alpha by title
* rating e.g. higest first, unrated first

## You can _filter_ the list of Books so that you can

The list of Books can be _filtered_ by:

* state e.g. "only UNREAD" or "not READ yet"
* reviewed e.g. "review" is not empty
* "good reads" e.g. ratings greater than "3"
