# Read: 31 - Espresso

## Espresso Testing (read Overview, Basics, and Recipes, plus any others that look interesting)

- Use Espresso to write concise, beautiful, and reliable Android UI tests.
- Each time your test invokes onView(), Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met:
  - The message queue is empty.
  - There are no instances of AsyncTask currently executing a task.
  - All developer-defined idling resources are idle.
- API Components
  - The main components of Espresso include the following:
    - **Espresso** – Entry point to interactions with views. Also exposes APIs that are not necessarily tied to any view, such as pressBack().
    - **ViewMatchers** – A collection of objects that implement the ``Matcher<? super View>`` interface. You can pass one or more of these to the onView() method to locate a view within the current view hierarchy.
    - **ViewActions** – A collection of ViewAction objects that can be passed to the ViewInteraction.perform() method, such as click().
    - **ViewAssertions** – A collection of ViewAssertion objects that can be passed the ViewInteraction.check() method. Most of the time, you will use the matches assertion, which uses a View matcher to assert the state of the currently selected view.
- Assertions can be applied to the currently selected view with the check() method.
  - The most used assertion is the matches() assertion. 
  - It uses a ViewMatcher object to assert the state of the currently selected view.
- AdapterView is a special type of widget that loads its data dynamically from an Adapter.
  - The most common example of an AdapterView is ListView.
- The ``ActionBarTestActivity`` has two different action bars: a normal action bar and a contextual action bar that is created from a options menu.
  - Both action bars have one item that is always visible and two items that are only visible in overflow menu.
- The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code.
- Espresso tests consist of two primary components: UI interactions and assertions on View elements.
  - UI interactions include tap and type actions that a person may use to interact with your app.
  - Assertions verify the existence or contents of visual elements on the screen.
- Link to follow steps to record UI interactions and add assertions to verify UI elements
  - [Espresso Testing](https://developer.android.com/studio/test/espresso-test-recorder)
