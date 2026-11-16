# **Mobile App Development – Practical Pseudocode**

## **1. Flutter Environment Setup & First App**

**Aim:** Create and run a Hello World Flutter application.

**Pseudocode:**

```
START
    Install Flutter SDK and Dart
    Install Android Studio or VS Code
    Configure Flutter environment
    Create a new Flutter project
    Open the project
    Create the main() function
    Run the Flutter application
    Display "Hello World" on screen
    Run on emulator or physical device
STOP
```

**Output:** Hello World is displayed on the screen.

## **2. Dart Basics Lab**

**Aim:** Demonstrate variables, data types, loops, functions and collections.

**Pseudocode:**

```
START
    Declare integer, string and double variables

    Display all variables

    Use IF-ELSE to check a condition

    Use FOR loop to print numbers

    Create a function
    Call the function

    Create a List
    Add and display elements

    Create a Map
    Display key and value

    Create a Set
    Display unique elements

    Check null safety
STOP
```

**Output:** Displays variables, conditions, loops, functions and collections.

## **3. Flutter UI Layouts**

**Aim:** Create a screen using Row, Column, Container, Scaffold and AppBar.

**Pseudocode:**

```
START
    Create a Flutter application

    Create Scaffold
        Add AppBar with title

        Create Body
            Add Container

            Add Column
                Add Text
                Add Row
                    Add Button
                    Add Button

    Create second screen

    When button is clicked
        Navigate to second screen

    When back button is pressed
        Return to first screen
STOP
```

**Output:** Displays a screen with buttons and navigation between two screens.

## **4. Forms & Responsive UI**

**Aim:** Create a registration form with validation and responsive layout.

**Pseudocode:**

```
START
    Create registration screen

    Add TextField for Name
    Add TextField for Email
    Add TextField for Password

    Add Submit Button

    When Submit Button is clicked
        Check if Name is empty
        Check if Email is valid
        Check if Password is empty

        IF all inputs are valid
            Display "Registration Successful"
        ELSE
            Display error message
        ENDIF

    Adjust layout according to screen size
STOP
```

**Output:** Registration form with input validation and responsive design.

## **5. State Management & Local Storage**

**Aim:** Create a counter and save data using SharedPreferences.

**Pseudocode:**

```
START
    Set counter = 0

    Display counter

    When Increment Button is clicked
        Increase counter by 1
        Update screen

    When Decrement Button is clicked
        Decrease counter by 1
        Update screen

    Save counter using SharedPreferences

    When application opens
        Load saved counter
        Display saved counter
STOP
```

**Output:** Counter increases and decreases, and its value remains saved after restarting the app.

## **6. REST API Integration**

**Aim:** Fetch JSON data from a public API and display it in ListView.

**Pseudocode:**

```
START
    Create application

    Show Loading Indicator

    Send HTTP GET request to API

    IF response is successful
        Receive JSON data
        Convert JSON into usable data
        Display data in ListView
    ELSE
        Display error message
    ENDIF

    Hide Loading Indicator
STOP
```

**Output:** Data from the API is displayed in a list.

## **7. Firebase Integration**

**Aim:** Implement Email/Password Authentication and CRUD operations using Firestore.

**Pseudocode:**

```
START
    Connect application to Firebase

    Create Login and Registration screen

    Enter Email and Password

    IF user registers
        Create new Firebase account
    ELSE IF user logs in
        Verify Email and Password

        IF credentials are correct
            Open Home Screen
        ELSE
            Display error
        ENDIF
    ENDIF

    Perform Firestore operations
        Create data
        Read data
        Update data
        Delete data
STOP
```

**Output:** User can register, log in and perform CRUD operations.

## **8. iOS / SwiftUI Basics**

**Aim:** Create a basic SwiftUI application with Text, Image and Button.

**Pseudocode:**

```
START
    Create a new SwiftUI project

    Create ContentView

    Add VStack

        Add Text
        Add Image
        Add Button

    When Button is clicked
        Display a message

    Run application on iOS Simulator
STOP
```

**Output:** Displays text, image and button in an iOS application.

## **9. SwiftUI Navigation & State**

**Aim:** Create multiple screens using NavigationStack and manage data using @State and @Binding.

**Pseudocode:**

```
START
    Create first screen

    Declare a variable using @State

    Display variable value

    Add NavigationStack

    Add NavigationLink to second screen

    Pass data using @Binding

    Update variable on second screen

    Return to first screen

    Read local JSON file
    Decode JSON data
    Display data in List
STOP
```

**Output:** Navigation between screens with updated data and JSON list display.

## **10. Testing, Debugging & Deployment**

**Aim:** Test, debug and prepare a Flutter application for deployment.

**Pseudocode:**

```
START
    Create Flutter application

    Open Flutter DevTools
    Check application performance

    Write Unit Tests
    Write Widget Tests

    Run all tests

    IF tests pass
        Build signed APK
        Prepare iOS IPA
        Follow Play Store submission steps
        Follow App Store submission steps
    ELSE
        Find errors
        Fix errors
        Run tests again
    ENDIF
STOP
```

**Output:** Tested and debugged application ready for deployment.

# **Important concepts to remember for your practical exam**

|Practical|Important concepts|
|---|---|
|1|Flutter SDK, Dart, Emulator|
|2|Variables, Loops, Functions, List, Map, Set|
|3|Row, Column, Scaffold, AppBar|
|4|TextField, Validation, MediaQuery|
|5|setState, Provider, SharedPreferences|
|6|HTTP GET, JSON, ListView|
|7|Firebase Auth, Firestore, CRUD|
|8|SwiftUI, VStack, HStack, Button|
|9|NavigationStack, @State, @Binding, JSON|
|10|DevTools, Unit Testing, Widget Testing, APK, IPA|

**My exam tip:** Learn the START → PROCESS → IF/ELSE → DISPLAY → STOP structure. Most of these practicals can be explained using this structure.

