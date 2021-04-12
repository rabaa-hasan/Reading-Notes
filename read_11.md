# EJS
An api developed by google that can be used to assist in searching for content any book in the world.

To install it :

```
install express with body-parse using this line:

npm install --save express body-parser cors ejs
```
### Volumnes:
can perform search by volumes by making a get request to the following: https://www.googleapis.com/books/v1/volumes?q=search+terms

the get request takes in a single required parameter, q which represents a specific string of text. plugged into a search query.

example of search by author. https://www.googleapis.com/books/v1/volumes?q=flowers+inauthor:keyes&key=yourAPIKey

if successful, the server will respond with a 200 OK HTTP status message.

returned data will come in the following format.

```
{
 "kind": "books#volumes",
 "items": [
  {
   "kind": "books#volume",
   "id": "_ojXgsadfqsC",
   "etag": "OTX2tA42qn4",
   "selfLink": "https://www.googleapis.com/books/v1/volumes/_ojXNuzgHRcC",
   "volumeInfo": {
    "title": "Flowers",
    "authors": [
     "Vijaya Khisty Bodach"
    ],
   ...
  }}]
  }
```

You use the download parame to restrict the returned results to volumes that have a downloadable format of epub by setting download=epub.

GET https://www.googleapis.com/books/v1/volumes?q=pride+prejudice&download=epub&key=yourAPIKey

can also set a filter parameter, which can have the following values

* partial
* full
* free-ebooks
* paid-ebooks
* ebooks
* Pagination parameters: startIndex, maxResults

You can use the projection parameter with one of the following values to specify a predefined set of Volume fields to return: full, lite

Can sort results using. sortBy = relevance/newest