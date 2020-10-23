# Readings: API Server

## [express()](https://expressjs.com/en/4x/api.html#router.param)

<!-- ### Author -->

The express() function is a top-level function exported by the express module.

Methods

  - express.json()

    This is a built-in middleware function in Express. It parses incoming requests with JSON payloads and is based on body-parser.

    Returns middleware that only parses JSON and only looks at requests where the Content-Type header matches the type option. This parser accepts any Unicode encoding of the body and supports automatic inflation of gzip and deflate encodings.

    A new body object containing the parsed data is populated on the request object after the middleware (i.e. req.body), or an empty object ({}) if there was no body to parse, the Content-Type was not matched, or an error occurred.

  - express.raw()

    This is a built-in middleware function in Express. It parses incoming request payloads into a Buffer and is based on body-parser.

    Returns middleware that parses all bodies as a Buffer and only looks at requests where the Content-Type header matches the type option. This parser accepts any Unicode encoding of the body and supports automatic inflation of gzip and deflate encodings.

    A new body Buffer containing the parsed data is populated on the request object after the middleware (i.e. req.body), or an empty object ({}) if there was no body to parse, the Content-Type was not matched, or an error occurred.

  - express.Router()

    Creates a new [router](https://expressjs.com/en/4x/api.html#router) object.

  - express.static()

    This is a built-in middleware function in Express. It serves static files and is based on serve-static.

    The root argument specifies the root directory from which to serve static assets. The function determines the file to serve by combining req.url with the provided root directory. When a file is not found, instead of sending a 404 response, it instead calls next() to move on to the next middleware, allowing for stacking and fall-backs.

  - express.text()

    This is a built-in middleware function in Express. It parses incoming request payloads into a string and is based on body-parser.

    Returns middleware that parses all bodies as a string and only looks at requests where the Content-Type header matches the type option. This parser accepts any Unicode encoding of the body and supports automatic inflation of gzip and deflate encodings.

    A new body string containing the parsed data is populated on the request object after the middleware (i.e. req.body), or an empty object ({}) if there was no body to parse, the Content-Type was not matched, or an error occurred.

  - express.urlencoded()

    This is a built-in middleware function in Express. It parses incoming requests with urlencoded payloads and is based on body-parser.

    Returns middleware that only parses urlencoded bodies and only looks at requests where the Content-Type header matches the type option. This parser accepts only UTF-8 encoding of the body and supports automatic inflation of gzip and deflate encodings.

    A new body object containing the parsed data is populated on the request object after the middleware (i.e. req.body), or an empty object ({}) if there was no body to parse, the Content-Type was not matched, or an error occurred. This object will contain key-value pairs, where the value can be a string or array (when extended is false), or any type (when extended is true).  



---

## [Middleware](https://mongoosejs.com/docs/middleware.html)

  Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins.

  Types of Middleware

  Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.


---

[Back to Home](https://pdariuslee.github.io/reading-notes/)