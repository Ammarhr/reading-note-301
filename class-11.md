## What is EJS:
**EJS** (Embedded JavaScript) is a templating engine for for JavaScript. So, font-end stuff.

 **to install EJS with NPM.**:
 ``npm install ejs``

### EJS Features :

1. Fast compilation and rendering
2. Simple template tags: <% %>
3. Custom delimiters (e.g., use <? ?> instead of <% %>)
4. Includes: Includes are relative to the template with the include call. (This requires the 'filename' option.)  ``<%- include('user/show'); %>.``
5. Both server JS and browser support
6. Static caching of intermediate JavaScript
7. Static caching of templates
8. Complies with the Express view system

#### Caching:
**EJS** ships with a basic in-process cache for caching the intermediate JavaScript functions used to render templates

**EX:**
```
let ejs = require('ejs'),
    LRU = require('lru-cache');
ejs.cache = LRU(100); 
```

#### Layouts:
**EJS** does not specifically support blocks, but layouts can be implemented by including headers and footers

**EX:**
```
<%- include('header'); -%>
<h1>
  Title
</h1>
<p>
  My page
</p>
<%- include('footer'); -%>
```

#### Caveats
Most of EJS will work as expected; however, there are a few things to note:
1. Obviously, since you do not have access to the filesystem, `ejs.renderFile` won't work.
2. For the same reason, includes do not work unless you use an include callback.

-------------------------------
## Working with volumes
Performing a search
You can perform a volumes search by sending an HTTP GET request to the following URI:
``https://www.googleapis.com/books/v1/volumes?q=search+terms``

### Request
Here is an example of searching for Daniel Keyes' "Flowers for Algernon":
``GET https://www.googleapis.com/books/v1/volumes?q=flowers+inauthor:keyes&key=yourAPIKey``

>>**Note**: Performing a search does not require authentication, so you do not have to provide the Authorization HTTP header with the GET request.
>>

### Response
If the request succeeds, the server responds with a 200 OK HTTP status code and the volume results.


