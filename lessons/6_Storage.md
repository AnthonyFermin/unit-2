### Storing Files

#### Objective

Students will understand how to store data using shared preferences and internal and external storage.

#### Do Now (Morning)

> Create a `User` class. A User has a name and an age. Create a constructor and getters and setters for this object, and override toString so that it returns "$name, $age".

> Create an app with one main activity. The activity should include an EditText that takes in a user's name and
> a number representing the user's age, and a submission button.

> When a user hits the submit button, use the name and age fields to create a `User` object with that name and age. Store the `Users` in an array.

#### Lesson (Morning)

##### Shared Preferences

> Exercise

> Add a `total_users` counter to your app. Every time a user gets added, increment this value and toast how many users you've seen. Store/retrieve `total_users` in shared preferences so that this number always increases across uses.

##### File Object

[File](http://developer.android.com/reference/java/io/File.html) - The File object represents a File and can be used to create, delete, read from, and write to a File. You can also use this object to manage File permissions and metadata.

##### Serializing Data

> Exercise

> 

#### Do Now (Afternoon)

> Add a spinner (dropdown), and populate the spinner with your `Users` array.

#### Lesson (Afternoon)

##### Querying Free Space

##### Internal vs External Storage



##### Saving a file to internal storage

> Exercise

> Using the serialized `User` object, whenever a new `User` is added, add it as a line in the file. Use this file
to populate the spinner.

##### Saving a file to external storage

###### Permissions

In the Manifest file, you must add permissions to access external storage. In order to read from external storage, include the line:

```
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
```

In order to write to external storage, include the line:

```
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
```

Note that, as with the File object, read permissions and write permissions are separate (as are execution permissions). This division of permissions is typical.

###### Reading and Writing

> Exercise

> Do the same thing, saving the serialized `User` object and populating the spinner, but instead saving to and reading from external storage.

##### Deleting a File

> Exercise

> Add a "clear all" button to the main activity. When this button gets pressed, delete the file.

##### Tools

(Accessing a file with ADB etc.)

#### Assessment

#### Resources
