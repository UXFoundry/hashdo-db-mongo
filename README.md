# \#Do MongoDB

This is a database implementation plugin for persisting [\#Do](https://github.com/UXFoundry/hashdo) card state to [MongoDB](https://www.mongodb.org/) .

## Getting Started
To make use of MongoDB for state in a [\#Do](https://github.com/UXFoundry/hashdo) project, you simply replace the built-in `db` object property with this implementation.

```js
var hashdo = require('hashdo');

// Use the MongoDB database plugin.
hashdo.db = require('hashdo-db-mongo');

// Using the hashdo-web project?
var hashdoweb = require('hashdo-web');

hashdoweb.hashdo.db = require('hashdo-db-mongo');
```

## MongoDB
A local or remote instance of [MongoDB](https://www.mongodb.org/) is required.

## Environment Variables
To use a custom database connection, you will need to set the following environment variable.

#### `MONGO`
This variable is optional, if a value is not set then a connection to `mongodb://localhost/hashdo` will be attempted.

## License
Copyright 2015 (c). All rights reserved.

Licensed under the Apache License, Version 2.0 (the "License"); you
may not use this file except in compliance with the License. You may
obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
implied. See the License for the specific language governing permissions
and limitations under the License.