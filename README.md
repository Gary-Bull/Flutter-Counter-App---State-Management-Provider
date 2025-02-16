# Using a State Management Provider

Using the default counter app provided when creating a new Flutter project. I added the `provider` pub package to manage and share state in a clean and efficient manner.

I created the below files - 

- counter_model.dart
- home_page.dart

In the `counter_model.dart` file i created the `CounterModel` class that extends the `ChangeNotifier` class. In the `CounterModel` class, I created a variable to hold the count number, and 3 methods, one to increment the count, one to decrement the count and the last one to reset the count to 0, each of the methods also notifies the listeners.

The `home_page.dart` file contains the `MyHomePage` stateful widget, that has one required parameter to be passed to it, which is call `title`, this parameter is then passed to the Text widget so you're able to dynamically change the title of the AppBar widget, if you wish.

There are 3 FloatingActionButton's which contain Icon widgets and when they are pressed the BuildContext reads the <CounterModel> to find the current count value, then calls one of the 3 methods. 

![image](https://github.com/user-attachments/assets/84c61345-c72d-45d7-ac70-4567ee156168)
