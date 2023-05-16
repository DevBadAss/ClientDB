# ClientDB

ClientDB is a JavaScript module for storing and manipulating data in Local and Session Storage in browsers.

## Installation

To use ClientDB in your project, you can include the module directly in your HTML file or import it as a module in your JavaScript code.

### Directly in HTML

```html

  <script src="path/to/clientdb.js"></script>

```

### Import as a module

```javascript

import ClientDB from 'path/to/clientdb.js';

```

    

## Usage

### Creating a Database

To create a new database, instantiate the `ClientDB` class with the desired name and database type:

```javascript

const localDB = new ClientDB('myLocalDB', { type: 'local' });

const sessionDB = new ClientDB('mySessionDB', { type: 'session' });

```

### Retrieving the Database

To retrieve the database and its contents, use the `getDb()` method:

```javascript

const data = localDB.getDb();

console.log(data);

```

### Querying Data

To query data from the database, use the `query(key)` method:

```javascript

const result = localDB.query('name');

console.log(result);

```

### Inserting Data

To insert data into the database, use the `insert(data)` method:

```javascript

localDB.insert({ name: 'John Doe', age: 30 });

```

### Deleting the Database

To delete the entire database, use the `delete()` method:

```javascript

localDB.delete();

```

## Authors

- [@DevBadAss](https://www.github.com/devbadass)

## License

This project is licensed under the [MIT Licence](https://choosealicense.com/licenses/mit/)

