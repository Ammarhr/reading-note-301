## What is Node.js?
Node.js is an open source server environment, runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.) , it uses JavaScript on the server. and it is free.

## Why Node.js?
it is about how Node.js handles a file request:
A common task for a web server can be to open a file on the server and return the content to the client:
node.js handles a file request by folowing:
1. Sends the task to the computer's file system.
2. Ready to handle the next request.
3. When the file system has opened and read the file, the server returns the content to the client.

**Node.js** eliminates the waiting, and simply continues with the next request. and runs single-threaded, non-blocking, asynchronously programming, which is very memory efficient.

### What Can Node.js Do?
**Node.js** can :
1. generate dynamic page content
2. create, open, read, write, delete, and close files on the server
3. collect form data
4. add, delete, modify data in your database

### What is a Node.js File?
- Node.js files contain tasks that will be executed on certain events
- A typical event is someone trying to access a port on the server
- Node.js files must be initiated on the server before having any effect
- Node.js files have extension ".js"

### What Kind of Apps Is Node.js Suited To?
Node is particularly suited to building applications that require some form of real-time interaction or collaboration — for example, chat sites, or apps such as CodeShare, where you can watch a document being edited live by someone else.

### What Are the Advantages of Node.js?
Aside from speed and scalability, an often-touted advantage of using JavaScript on a web server — as well as in the browser — is that your brain no longer needs to switch modes. You can do everything in the same language, which, as a developer, makes you more productive . For example, you can easily share code between the server and the client.

-------------------------------------------------
### What Is Lazy Loading?
Lazy loading images means loading images on websites asynchronously — that is, after the above-the-fold content is fully loaded, or even conditionally, only when they appear in the browser’s viewport. This means that if users don’t scroll all the way down, images placed at the bottom of the page won’t even be loaded.
and to solve this problem there are 5 techniques:

1. **Native Lazy Loading:**
Native lazy loading of images and iframes is super cool.
2. **Lazy Loading Using the Intersection Observer API**
The Intersection Observer API is a modern interface that you can leverage for lazy loading images and other content.
3. **Lozad.js**
A quick and easy alternative for implementing lazy loading of images is to let a JS library do most of the job for you.
4. **Lazy Loading with Blurred Image Effect**
If you’re a Medium reader, you have certainly noticed how the site loads the main image inside a post.
5. **Yall.js**
Yall is a feature-packed, lazy-loading script for images, videos, and iframes.