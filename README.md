# Android-Stopwatch

##Description
Android doesn't have a built in stopwatch, it only has the CountDownTimer. So I built a stopwatch class that can be easily used.

##Usage

The interface is easy to use:

1. To start the stopwatch you call start() method.
2. To start the stopwatch with a given offset pass in the offset as a parameter to start. (Ex: If you want to start the
time from 00:00:10 not 00:00:00)

3. To get the current time there are multiple convienece methods to get each component. An easier approach is to call the toString() that will return the time in the form of HH:MM:SS

```java
Stopwatch stopWatch = new Stopwatch();
stopwatch.start();
long minutes = stopwatch.getElapsedTimeMin();
Log.d("Time", stopwatch.toString());
```

4. You can add a listener to listen for tick events every second by calling the Stopwatch(StopwatchListener listener) or stopwatch.addListener(StopwatchListener listener)



##TODO
- [ ] Make the listining period dynamic and provided by the client.
- [ ] Add more convience methods to print the time in different formats
- [ ] Add different views for the class to display the time on.
- [ ] Add a gradle plugin.

##License

The logic was inspired by [this answer on StackOverflow](http://stackoverflow.com/a/22357730/4504604).
