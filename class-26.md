# Read: 26 - Android Fundamentals

## Android fundamentals

- There are four different types of app components:
  - Activities
    - An activity is the entry point for interacting with the user.
    - It represents a single screen with a user interface.
    - For example, an email app might have one activity that shows a list of new emails, another activity to compose an email, and another activity for reading emails.
    - You implement an activity as a subclass of the **Activity** class.
  - Services
    - A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons.
    - It is a component that runs in the background to perform long-running operations or to perform work for remote processes.
    - A service does not provide a user interface.
    - For example, a service might play music in the background while the user is in a different app, or it might fetch data over the network without blocking user interaction with an activity.
    - A service is implemented as a subclass of **Service**
  - Broadcast receivers
    - A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.
    - So, for example, an app can schedule an alarm to post a notification to tell the user about an upcoming event... and by delivering that alarm to a BroadcastReceiver of the app, there is no need for the app to remain running until the alarm goes off.
    - A broadcast receiver is implemented as a subclass of **BroadcastReceiver** and each broadcast is delivered as an **Intent** object.
  - Content providers
    - A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access.
    - For example, the Android system provides a content provider that manages the user's contact information.
    - A content provider is implemented as a subclass of **ContentProvider** and must implement a standard set of APIs that enable other apps to perform transactions.

[Back to README](README.md)
