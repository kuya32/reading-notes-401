# Read: 27 - Intents, Activities, and SharedPreferences

## Android Tasks and the Back Stack

- If the user presses the **Back** button, that new activity is finished and popped off the stack.
- The affinity indicates which task an activity prefers to belong to.

## Android SharedPreferences

- SharedPreference
  - A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them.
  - Each SharedPreferences file is managed by the framework and can be private or shared.
- ``getSharedPreferences()``
  - Use this if you need multiple shared preference files identified by name, which you specify with the first parameter. You can call this from any Context in your app.
- ``getPreferences()``
  - Use this from an Activity if you need to use only one shared preference file for the activity. Because this retrieves a default shared preference file that belongs to the activity, you don't need to supply a name.
- SharedPreferences.Editor
  - ``apply()`` changes the in-memory SharedPreferences object immediately but writes the updates to disk asynchronously. 
  - Alternatively, you can use ``commit()`` to write the data to disk synchronously.

[Back to README](README.md)
