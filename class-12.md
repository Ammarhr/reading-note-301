## EJS Partials:
When using the default view engine (ejs), Sails supports the use of partials (i.e. "view partials"). Partials are basically just views that are designed to be used from within other views.
They are particularly useful for reusing the same markup between different views, layouts, and even other partials.

### Partials and view locals

**Partials** automatically inherit the view locals that are available wherever they are used.

### Overriding locals in a partial
Automatic inheritance of view locals takes care of most use cases for partials, but sometimes you might want to pass in additional, dynamic data.

>>
**Notes:**

- Partials are rendered synchronously, so they will block Sails from serving more requests until they're done loading. It's something to keep in mind while developing your app, especially if you anticipate a large number of connections.

- Built-in support for partials in Sails is only for the default view engine, ejs. If you decide to customize your Sails install and use a view engine other than ejs, then please be aware that support for partials (sometimes known as "blocks", "includes", etc.) may or may not be included, and that the usage will vary. Refer to the documentation for your view engine of choice for more information on its syntax and conventions.
>>
