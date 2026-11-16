# **Mobile App Development – Complete Easy Explanation**

First, understand that your practicals mainly cover two technologies:

[Natlov](https://images.openai.com/static-rsc-4/hQgBHFlEAmNQpqYrag5U2jd4QJtNBGHBKf7LSMAOLhDyYCphMIYyqccbQHiB7gM0bmgwkauIIDlOD1d2hupU-o2ygsVHxqSFHfxc76DNuysMKieoLNbrcPlXj2a6U8ZAD5eGk0n090V4itFvEK-_fJYbeVoGYdLc_DbR24nAiis?purpose=inline)

**Flutter + Dart**

Used to build Android and iOS applications.

Practicals 1–7 and 10

[Apple Invites Some Developers to Try Swift Playgrounds 4 Ahead of Launch - MacRumors](https://images.openai.com/static-rsc-4/1XcB4JyIYRLzLM8XZmhuhaR_Bn09XRSfhBmZLX9vaqhNa8SRbzOwoFfX816tzYlipsF5hEyK4XBTKkUuz68We2lbLsZ9088f4M1M2tvVB9WXcJbZX5CnDTaZn412-GNJNxs6xvjpXyTpb-0gK-wxB1PZrlSyaGoDOoHFsTtAXGI?purpose=inline)

**Swift + SwiftUI**

Used to build iOS applications.

Practicals 8–9

# **Part 1: Dart Basics (Practical 2)**

Let's start with the basics.

## **1. Variables**

A variable is like a container that stores information.

For example:

- Your age
- Your name
- Your marks

```
int age = 20;
String name = "Atharv";
double marks = 85.5;
bool isStudent = true;
```

| Data type | Meaning        | Example |
| --------- | -------------- | ------- |
| int       | Whole number   | 20      |
| double    | Decimal number | 85.5    |
| String    | Text           | "Hello" |
| bool      | True or False  | true    |

**Remember:** A variable stores data.

## **2. Conditions (IF-ELSE)**

Conditions help a program make decisions.

Example: Check whether a student has passed.

```
int marks = 75;

if (marks >= 40) {
  print("Pass");
} else {
  print("Fail");
}
```

If marks are 40 or more, it prints Pass. Otherwise, it prints Fail.

**Real-life example:** If it is raining, take an umbrella. Otherwise, don't take one.

## **3. Loops**

Loops are used when you want to repeat something multiple times.

Example:

```
for (int i = 1; i <= 5; i++) {
  print(i);
}
```

Output:

```
1
2
3
4
5
```

Instead of writing print five times, a loop does the work.

## **4. Functions**

A function is a block of code that performs a particular task.

Example:

```
void greet() {
  print("Hello Atharv");
}

void main() {
  greet();
}
```

Whenever you call `greet()`, it executes that code.

**Real-life example:** A calculator's addition function adds two numbers whenever you use it.

## **5. Collections**

This is an important concept.

Collections mean storing multiple values together in one variable.

Dart has three important collections:

### **A. List**

A List stores multiple values in an ordered manner. It allows duplicate values.

```
List<String> names = [
  "Rahul",
  "Amit",
  "Priya"
];

print(names[0]);
```

Output: `Rahul`

Think of a List as a shopping list.

**List example**

0

Rahul

1

Amit

2

Priya

Each item has an index starting from 0.

### **B. Set**

A Set stores unique values. It automatically removes duplicates.

```
Set<int> numbers = {1, 2, 3, 3, 4};

print(numbers);
```

Output:

```
{1, 2, 3, 4}
```

Think of a Set as a guest list where each person can appear only once.

### **C. Map**

A Map stores information in key-value pairs.

Example:

```
Map<String, dynamic> student = {
  "name": "Atharv",
  "age": 20,
  "marks": 85
};

print(student["name"]);
```

Output: `Atharv`

Think of a Map as a student ID card.

| Key   | Value  |
| ----- | ------ |
| name  | Atharv |
| age   | 20     |
| marks | 85     |

**Easy trick to remember:**

- List = Multiple values in order.
- Set = Unique values.
- Map = Key and value.

## **6. Null Safety**

Null means that a variable has no value.

For example:

```
String? name;
name = null;
```

The `?` means the variable is allowed to contain null.

Without `?`:

```
String name = "Atharv";
```

It must contain a String value and cannot be null.

**Why is it useful?**

It helps prevent errors caused by missing data.

# **Part 2: Flutter UI Concepts (Practical 3 and 4)**

Now let's understand how Flutter creates the screen of an application.

## **7. Scaffold**

[liveBook · Manning](https://images.openai.com/static-rsc-4/ICECYb74xaOSc570dpMwvVrYbZTHxrC_qrDIzehZC5yPxQYYhGFAIVKWmP3HWLNoguWxxsfpxfUYi4ZuJKcG2YMAIO_KNNzBVwsv2XgweChC3Sd9ormMbwPLCeQAfq-kGDWpcUmxjyUG-S0UUq9hXLt3qWyQioIxz0LygTcK_Sg?purpose=inline)

**Scaffold = Basic structure of an app screen.**

It provides the standard layout for a screen, such as:

- AppBar
- Body
- Floating Action Button
- Bottom Navigation Bar

Example:

```
Scaffold(
  appBar: AppBar(
    title: Text("My App"),
  ),
  body: Text("Hello World"),
);
```

Think of Scaffold as the structure of a house. It gives you the basic spaces where you put things.

## **8. AppBar**

AppBar is the top bar of an application.

It usually contains:

- Application title
- Back button
- Settings icon
- Menu icon

```
AppBar(
  title: Text("Home Page"),
)
```

## **9. Row and Column**

These are used to arrange widgets.

[Expanded Widgets in Flutter](https://images.openai.com/static-rsc-4/s9fKmvh_J1h98Nwp8M1_Ozs9OBj28c7iYaG-3lpzZzzdBrbE769M74n4VyKPWmqWS6ceyaJKrG9A3xCxBHjVaWEwGynSaIKW78HcHeOZY4J3Jj6w-NvExEjfst78jxcf1uDOPA-cEQbMSk4PmHjw9o-xM9XCk2sYkG1GBz-OSUk?purpose=inline)

**Row**

Arranges items horizontally (left to right).

[Understanding Flutter Widgets: Column vs Row - DEV Community](https://images.openai.com/static-rsc-4/jvrLhJ74TyYH-rMAnMFcW0W-I17ELjYvH1hplhFzWsm7UmBtghZWX9ZoFukbB5L7GKnB5glXEdmeAkSVti-OZtq60moK1aj6HsLehVXWeN5F70lQlWxrksxf4ryZoR7GjPCrQykgsQWVBzwS8H1wIZeSaJmg3rS02LFTeE0WV-s?purpose=inline)

**Column**

Arranges items vertically (top to bottom).

Example:

```
Column(
  children: [
    Text("Name"),
    Text("Age"),
    Text("City"),
  ],
)
```

This displays three text widgets one below another.

## **10. Container**

Container is like a box that holds another widget.

You can give it:

- Height
- Width
- Background colour
- Padding
- Margin
- Border

Example:

```
Container(
  height: 100,
  width: 200,
  color: Colors.blue,
  child: Text("Hello"),
)
```

Think of it as a coloured box on your mobile screen.

## **11. Widget**

This is one of the MOST important Flutter concepts.

**Everything you see in Flutter is a Widget.**

Examples:

- Text
- Button
- Image
- Container
- Row
- Column
- Scaffold

Even the complete screen is built using widgets.

## **12. Navigation**

Navigation means moving from one screen to another.

Example:

You open an app:

1. Login Screen
2. Home Screen
3. Profile Screen

In Flutter, you can use `Navigator.push()` to open another screen and `Navigator.pop()` to return to the previous screen.

```
Navigator.push(
  context,
  MaterialPageRoute(
    builder: (context) => SecondScreen(),
  ),
);
```

Think of it like opening a new page in a book.

## **13. TextField and Form Validation**

**TextField** allows users to enter information.

Examples:

- Name
- Email
- Password
- Phone number

```
TextField(
  decoration: InputDecoration(
    labelText: "Enter Name",
  ),
)
```

**Form Validation** means checking whether the user entered correct information.

Example:

- Name should not be empty.
- Email should be valid.
- Password should not be empty.

```
if (email.isEmpty) {
  print("Email is required");
} else {
  print("Valid input");
}
```

## **14. MediaQuery (Responsive UI)**

Responsive UI means the application adjusts according to screen size.

For example:

- Your app runs on a small phone.
- Your app runs on a large phone.
- Your app runs on a tablet.

MediaQuery helps Flutter get information about the screen.

```
double width = MediaQuery.of(context).size.width;
```

This gets the screen width.

**Remember:** MediaQuery = Screen size information.

# **Part 3: State Management (Practical 5)**

This is probably the most important section to understand.

First, understand one thing:

**State means the current value or condition of something in your application.**

For example, imagine a counter application.

Initially:

```
Counter = 0
```

You press the + button:

```
Counter = 1
```

You press it again:

```
Counter = 2
```

The counter value changes. This changing value is called State.

## **15. setState()**

`setState()` tells Flutter that something has changed and the screen needs to update.

Example:

```
int count = 0;

void increase() {
  setState(() {
    count++;
  });
}
```

What happens?

1. Initially, count is 0.
2. User presses the button.
3. count increases by 1.
4. setState tells Flutter to rebuild the relevant UI.
5. New value appears on the screen.

[Flutter Bloc - Detailed Explanation - Scaler Topics](https://images.openai.com/static-rsc-4/Ejk4118HuQF2GtEGSiC8amQf-4_kvjlkAeD3mKqJrdU5xKVmp1Bwge5OR6bySRpFq00pZQwg2m1dbCg2RZJDVcVYv7bUnToRGsTiVoul_4TxpcaHzuVM6EckaOKS6pGASSJ5VKqT-gwm0s1TmCx6qfYJerF0T4kfShGhAVLO3mk?purpose=inline)

[scaler.com](https://www.scaler.com/topics/flutter-bloc/?utm_source=chatgpt.com)

**Remember:** setState = Update the screen when data changes.

## **16. Provider**

Provider is another way to manage state in Flutter.

You might ask: If setState already updates the screen, why do we need Provider?

Imagine a shopping application.

You have:

- Home Screen
- Product Screen
- Cart Screen
- Payment Screen

When you add a product to your cart, the cart information may need to update on multiple screens.

Using setState separately on every screen can become difficult.

Provider helps share data between different parts of your application.

[State Management in Flutter: Exploring Provider | by Ankit Ahuja | Medium](https://images.openai.com/static-rsc-4/OzsL1jqOe2twX4jiNzxLnziz3gKSooDwzwo9_I8iGdgplnWpuuoCzZWML1Q3Y8QPNAnW4hvvf-jc1sUZeoEEtztNsUd-phhGApKqu5t0XJlxtS-NPwMDacO65YUHp_lj7wcpWl5K3qnfy3j7YxPEnbHiActN5iunJ_xaoNIwbos?purpose=inline)

[medium.com](https://medium.com/%40ankitahuja007/state-management-in-flutter-exploring-provider-7b1a41d262c5?utm_source=chatgpt.com)

**Simple example:**

Imagine you have a shopping cart.

```
Cart Provider:
    cartCount = 0

When product is added:
    cartCount = cartCount + 1

Notify all listening screens

Update cart count everywhere
```

**Difference between setState and Provider:**

| setState                   | Provider                      |
| -------------------------- | ----------------------------- |
| Simple state management    | Shared state management       |
| Usually used in one widget | Can share data across widgets |
| Easy for small apps        | Useful for bigger apps        |

**Remember:**

- setState = Update local screen.
- Provider = Share and manage data across screens.

## **17. SharedPreferences**

This is another VERY important concept.

SharedPreferences is used to save small amounts of data locally on the device.

Imagine you open an app and set the counter to 10.

You close the app and open it again.

Without saving, the counter may return to 0.

With SharedPreferences, you can save the value 10 and load it when the app starts again.

[Shared Preferences in Flutter: Store and Retrieve data locally | by Raju Potharaju | GYTWorkz | Medium](https://images.openai.com/static-rsc-4/QWtjVdoltHq9KkgFyZ2cTqQpIQDBOHm8aD1mW6eHe0uiwYf9bTAZlDYS8ebK4nh44UKH0hIJFWZgzkjp3_izTDusyKW4WxggHCNOM6ukkLRu0-KUEQm9lvuhx8ug53A_AdpHb3RyrCbb0-Ox8NyihhTXBfoPnnhlkLJ55lSHluc?purpose=inline)

[medium.com](https://medium.com/gytworkz/shared-preferences-in-flutter-store-and-retrieve-data-locally-bbc937fabce4?utm_source=chatgpt.com)

Example:

```
// Save data
prefs.setInt("count", 10);

// Read data
int count = prefs.getInt("count") ?? 0;
```

Here:

- `"count"` is the key.
- `10` is the value.
- `getInt()` retrieves the saved value.
- `?? 0` means use 0 if no saved value exists.

It can store:

- Integer
- String
- Boolean
- Double
- List of Strings

**Real-life example:** Remembering your app's dark mode setting even after closing it.

### **setState vs Provider vs SharedPreferences**

| Concept           | Main purpose                              |
| ----------------- | ----------------------------------------- |
| setState          | Update the UI                             |
| Provider          | Share/manage changing data                |
| SharedPreferences | Save small data permanently on the device |

These three are different. Don't confuse them!

# **Part 4: REST API and JSON (Practical 6)**

## **18. API**

API stands for Application Programming Interface.

In simple words, an API allows two applications or systems to communicate with each other.

Example:

You open a weather application.

The application needs weather information from a server.

It sends a request to an API, and the API returns the weather data.

[REST APIs — Beginner Friendly Guide | by Swastik Sharma | Medium](https://images.openai.com/static-rsc-4/0N8vFfZhJwq3eFPXiJ8d_gIP83hhtgaFFEW2AzNXINWE7kEBJmExA4Q41RyAqOK3p0EwMocEr23EkgSdJEZgG48q-xmnKbGDaN-kD4Qyxs-JPpLYKYZrVpP01YYi8V7hkLVXXhvYAlm9_nrR6LVTUYLgvdRx95UoGZgF8hxQxl0?purpose=inline)

[medium.com](https://medium.com/%40swastik7sharma/rest-apis-beginner-friendly-guide-e2a4a65239f2?utm_source=chatgpt.com)

**Remember:** API = Communication between applications.

## **19. REST API**

REST API is a common way for applications to communicate with servers using HTTP.

Some important methods:

| Method | Purpose             |
| ------ | ------------------- |
| GET    | Get data            |
| POST   | Send or create data |
| PUT    | Update data         |
| DELETE | Delete data         |

For your practical, GET is especially important.

Example:

```
Send GET request
       ↓
Receive student data
       ↓
Display student data
```

## **20. JSON**

JSON stands for JavaScript Object Notation.

It is a format used to exchange data between applications and servers.

Example:

```
{
  "name": "Atharv",
  "age": 20,
  "city": "Ahmedabad"
}
```

This is JSON data.

You can understand it as information organised in key-value pairs.

## **21. JSON Parsing**

Parsing means converting JSON data into a format your application can understand and use.

For example:

```
String name = data["name"];
```

This retrieves the name from the JSON data.

**Remember:**

- JSON = Data format.
- Parsing = Reading and extracting JSON data.

## **22. HTTP GET Request**

GET is used to fetch data from a server.

Example:

```
final response = await http.get(
  Uri.parse("https://example.com/users")
);
```

This sends a request to the server.

If successful, the server sends back data.

## **23. ListView**

ListView displays multiple items in a scrollable list.

Example:

- List of students
- List of products
- List of contacts

[A complete guide to Flutter’s ListTile | by Suragch | Medium](https://images.openai.com/static-rsc-4/wYukdL-9HHj7Lrq6mJpz7il0DSwDc8PZVmR9Fh1mTZcOG-9bilWT8VXnjOIw2AU4PKzPPUNaXU1enqw9sORnzOxMnqkCLgmY5dWwuOrh5ZCGHdzjKFDqDpG_CxsemxuE50FmYPcwGEvc6IBB9BttpBrLB4G-74dJFVizGSmtqEk?purpose=inline)

[suragch.medium.com](https://suragch.medium.com/a-complete-guide-to-flutters-listtile-597a20a3d449?utm_source=chatgpt.com)

**Remember:** ListView = Display multiple items in a scrollable list.

# **Part 5: Firebase (Practical 7)**

## **24. Firebase**

&#x20;Firebase

Firebase is a Google platform that provides services for mobile and web applications.

It provides:

- User authentication
- Database
- File storage
- Notifications
- Analytics

Think of Firebase as a ready-made backend for your application.

[Backend with Firebase: A Production-Ready Flutter Guide](https://images.openai.com/static-rsc-4/hiyY6aWg_HVi2MeZ5fHo77156kqbXveNj0UUUazY8q1yahkMCkQm00qZkas5CLfAZiICmYviaK6fz6hsLN3VpGnLhyUrJFkUOLZAB0EVzqdvw8yIAFoeBQtamaDtmRoZDJegbhDqfa_SldXFx_vHy9Rggzzqw44954w0FhLQW9g?purpose=inline)

[fluttergeekhub.com](https://fluttergeekhub.com/uncategorized/backend-with-firebase/?utm_source=chatgpt.com)

## **25. Authentication**

Authentication means checking who a user is.

Example:

You open an app and enter:

- Email
- Password

Firebase checks whether the login details are correct.

If correct, the user can log in.

If incorrect, it displays an error.

**Remember:** Authentication = Checking user identity.

## **26. Firestore**

Firestore is a cloud database provided by Firebase.

It stores application data online.

Example:

```
Students
   |
   |--- Student 1
   |       Name: Rahul
   |       Age: 20
   |
   |--- Student 2
           Name: Amit
           Age: 21
```

You can access this data through your application.

## **27. CRUD Operations**

CRUD represents four basic database operations.

| Letter | Full form | Meaning              |
| ------ | --------- | -------------------- |
| C      | Create    | Add new data         |
| R      | Read      | View data            |
| U      | Update    | Change existing data |
| D      | Delete    | Remove data          |

For example, imagine a student management application:

- Create: Add a new student.
- Read: Display student details.
- Update: Change student's age.
- Delete: Remove a student.

**Remember:** CRUD = Create, Read, Update, Delete.

# **Part 6: SwiftUI Basics (Practical 8 and 9)**

Now let's move to iOS development.

SwiftUI is Apple's framework used to create application interfaces using Swift.

## **28. SwiftUI**

SwiftUI is similar to Flutter because both are used to build application screens.

The difference is that SwiftUI is Apple's UI framework.

## **29. VStack**

VStack arranges elements vertically.

```
VStack {
    Text("Hello")
    Text("World")
}
```

Output:

```
Hello
World
```

Think of VStack as Flutter's Column.

## **30. HStack**

HStack arranges elements horizontally.

```
HStack {
    Text("Hello")
    Text("World")
}
```

Output:

```
Hello    World
```

Think of HStack as Flutter's Row.

## **31. ZStack**

ZStack arranges elements on top of each other.

Example:

```
ZStack {
    Color.blue
    Text("Hello")
}
```

Here, the text appears on top of the blue background.

[SwiftUI VStack - Syntax and Basic Examples \[3\]](https://images.openai.com/static-rsc-4/yRreeQ3aXpqgyBUF0XIT4LdxU076YVNUbrL5B8FtWCMygFb0aCrP6MTQE6DGV4WfN2ySDhth81OlqFySI_T4kRPRq3yxa5TRePj224S1I8YZQ0WzZAM1f_jYWvkvL2Qz5reQuzUXt-bpQzW4B-ygrpKYtodFQoJYKC2kqWyBC-A?purpose=inline)

VStack

Vertical

[Stacks and Spacer - SwiftUI Handbook - Design+Code](https://images.openai.com/static-rsc-4/Uu1379sYiCBdY_WZfuT_JlB-i7Heva_DUcd4E1M-iq6UzpbErD9uTtBpCXFAgv_VES6gFOiMzYym4890rXlR36T5SF1LeQ0roJCoANUAhlPdIzRIiBIJ0W85mm3DZ8dL_hz4ix855hjg5vvhrVV9OotXrst2UWFF8sFpcwcZUpg?purpose=inline)

HStack

Horizontal

[SwiftUI - Stack](https://images.openai.com/static-rsc-4/gNVXK_SdMS8_8jN1Wnlyl40BLd5R4FnT40tXKqoYrogDlQWI786I3JIH7I3EZAAHYq5hIkZg51M4u9gT2hqvJls9xJa9LRAaxTnjcXkdUXCrJHuvph8LPhuTvWNm0WcgSwUDIs0W3bNnibBiMzECxfOB6sLIFl4_AUaUyoSPdxk?purpose=inline)

ZStack

Overlapping

## **32. @State**

In SwiftUI, `@State` stores a value that can change.

Example:

```
@State var count = 0
```

When the value changes, SwiftUI automatically updates the interface that depends on it.

Think of it as Flutter's setState concept, although their implementations are different.

## **33. @Binding**

This is a very important concept.

Binding allows one view to access and change a value owned by another view.

Imagine:

- Parent screen has a counter.
- Child screen has a button.
- When the child button is clicked, the parent's counter changes.

This is what `@Binding` helps achieve.

Example:

Parent:

```
@State var count = 0

ChildView(count: $count)
```

Child:

```
@Binding var count: Int
```

The `$count` passes a binding to the child.

**Remember:**

- @State = Own and store the value.
- @Binding = Receive and modify a value owned by another view.

## **34. NavigationStack**

NavigationStack is used to move between different screens in SwiftUI.

Example:

```
First Screen
     |
     | Click Button
     ↓
Second Screen
     |
     | Click Button
     ↓
Third Screen
```

Think of it as Flutter's navigation system.

## **35. JSON Decoding in Swift**

JSON decoding means converting JSON data into Swift objects.

For example, a server sends:

```
{
  "name": "Rahul",
  "age": 20
}
```

Swift converts this data into a usable structure.

Usually, Swift uses:

- `Codable`
- `Decodable`
- `JSONDecoder`

**Remember:** JSON decoding = Convert JSON into Swift data.

# **Part 7: Testing, Debugging & Deployment (Practical 10)**

## **36. Testing**

Testing means checking whether your application works correctly.

For example:

- Does the login button work?
- Does the counter increase?
- Does registration work?
- Does the app crash?

There are two important types:

**A. Unit Testing**

Tests a small piece of code, such as a function.

Example:

```
int add(int a, int b) {
  return a + b;
}
```

You test whether:

```
add(5, 5) = 10
```

**B. Widget Testing**

Tests a particular Flutter widget or UI component.

Example:

- Check whether a button appears.
- Check whether text is displayed.
- Check whether clicking a button changes something.

## **37. Debugging**

Debugging means finding and fixing errors in your application.

Example:

You write:

```
int age = "20";
```

This produces an error because an integer cannot directly store a String.

You fix it:

```
int age = 20;
```

**Remember:** Debugging = Finding and fixing errors.

## **38. Flutter DevTools**

Flutter DevTools is a collection of tools used to inspect and debug Flutter applications.

It helps you:

- Find errors.
- Check performance.
- Monitor memory.
- Inspect widgets.
- Analyse application behaviour.

Think of it as a health-check tool for your application.

## **39. APK and IPA**

These are application package formats.

[Downloading and Installing APK Files Could Put Your Business at Risk - Directive Blogs | Directive Technology, Inc. | Otsego County, NY](https://images.openai.com/static-rsc-4/6veKEK1X50Tj2xeeU9Xbqhssgx4drvfkv31r4RdMIDpMDOl7Jxil3W1GXGSaWB-KYOmjFOT3KVnzYvjGFjPCOkK8jd1DPOTwRD1Ob45aMX-8xm1VfnpY7CXluQeIWj-Ec8kcLqNl8pH5wnggmAHjuzjbsZrit3g0OvtGLnRXmFw?purpose=inline)

**APK**

Android application package. Used to install Android apps.

[File IPA là gì? Chi tiết định dạng cài đặt ứng dụng trên iPhone](https://images.openai.com/static-rsc-4/zuS6k7QXZGRj-Vu-K0k6uz_aNsRHdvZKBk7_lN98waYyYIowgA58NtajRt3LMbO7XJb7goPhd-ecVqxuZQDIvtcnF3ImwpwrW-VXZy5EU7hiOg5i67J3hJdrrOThagouFZu6fN-j0hkrHr90VzJTLoCDXAPrTfihbhfnBDN0NaM?purpose=inline)

**IPA**

iOS application archive. Used for iOS app distribution.

**Remember:**

- APK = Android.
- IPA = iOS.

## **40. Deployment**

Deployment means making your application available to users.

For example:

- Uploading an Android app to Google Play Store.
- Publishing an iOS app on Apple App Store.

# **Part 8: Important Differences – Exam Revision**

These are the differences I recommend learning for your viva.

| Concepts                      | Difference                                                          |
| ----------------------------- | ------------------------------------------------------------------- |
| List vs Set                   | List allows duplicates; Set stores unique values                    |
| List vs Map                   | List uses indexes; Map uses keys                                    |
| Row vs Column                 | Row is horizontal; Column is vertical                               |
| Widget vs Scaffold            | Widget is a UI building block; Scaffold provides a screen structure |
| setState vs Provider          | Local state update vs shared state management                       |
| Provider vs SharedPreferences | Manage shared app state vs save data locally                        |
| API vs JSON                   | API communicates; JSON represents data                              |
| GET vs POST                   | GET fetches data; POST sends/creates data                           |
| Firebase Auth vs Firestore    | User authentication vs cloud database                               |
| Create vs Update              | Add new data vs modify existing data                                |
| VStack vs HStack              | Vertical vs horizontal                                              |
| @State vs @Binding            | Own a value vs access a value owned by another view                 |
| Unit vs Widget Testing        | Test functions vs test UI components                                |

# **Part 9: Test Your Understanding**

Let's see if you have understood these concepts. Try answering these 10 questions without looking above.

**Mini Viva Quiz**

0/10 answered

**1. Which Flutter function updates the UI when a local state changes?**

SharedPreferences

setState()

Scaffold

ListView

**2. Which collection stores only unique values?**

List

Map

Set

String

**3. Which Flutter widget provides the basic screen structure?**

Scaffold

TextField

Container

Row

**4. What is SharedPreferences used for?**

Creating buttons

Saving small data locally

Connecting to Firebase

Displaying images

**5. What is Provider mainly used for?**

Changing colours

Sharing and managing app state

Creating images

Installing Flutter

**6. Which HTTP method fetches data?**

POST

DELETE

GET

UPDATE

**7. What does CRUD stand for?**

Create, Read, Update, Delete

Copy, Run, Upload, Download

Create, Remove, Use, Display

Code, Read, Update, Design

**8. Which SwiftUI property wrapper owns a changing value?**

@Binding

@State

@View

@List

**9. What does @Binding do?**

Deletes data

Stores permanent data

Shares access to a value owned by another view

Creates a database

**10. Which file format is used for Android application packages?**

IPA

JSON

APK

PDF

Submit Answers

# **My recommendation for your practical exam**

Don't try to memorise all 40 definitions at once. Learn them in this order:

1. **First:** Dart basics – variables, conditions, loops, functions and collections.
2. **Second:** Flutter UI – Scaffold, Row, Column, Container and navigation.
3. **Third:** State management – setState, Provider and SharedPreferences.
4. **Fourth:** API, JSON and Firebase.
5. **Fifth:** SwiftUI – VStack, HStack, @State and @Binding.
6. **Finally:** Testing, debugging and deployment.

The most important thing is to understand **what each concept does, why we use it, and one real-life example**. That will help you answer both practical questions and viva questions confidently.
