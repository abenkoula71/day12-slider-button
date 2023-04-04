# Day12_slider_button_flutter

This package provides an easy implementation of a Slider Button to cancel current transaction or screen. Highly customizable iphone alike looking widget

# 1-Add the sqflite dependency in your pubspec.yaml file.

```
dependencies:
  sqflite: ^2.0.0+3
```

# 2-Import the sqflite package in your dart file.

```
import 'package:sqflite/sqflite.dart';
```

# 3-Open a database by using the openDatabase() method. You can create a new database by specifying the database name, version, and a callback function that creates the necessary tables.

```
final database = await openDatabase(
    'my_database.db',
    version: 1,
    onCreate: (db, version) async {
        await db.execute('CREATE TABLE IF NOT EXISTS users (id INTEGER PRIMARY KEY, name TEXT)');
    },
);
```

# 4-Perform CRUD operations using the database object. For example, to insert data into the users table, you can use the insert() method.


```
await database.insert('users', {'name': 'John Doe'});
```

# 5-Close the database by calling the close() method.

```
await database.close();
```

That's it! You can now use SQLite3 with Flutter by using the sqflite plugin.
