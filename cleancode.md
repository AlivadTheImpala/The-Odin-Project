# summary
To summarize, writing clean code is important because it allows you and others to understand your code at a future date. This means that your code is more easily maintainable and understandable, leading to less time trying to understand what's happening at any given line. 

## naming conventions
1. variables and functions should be descriptive
2. names should use consistent vocabulary
3. names should be immediately understandable
		ex: ONE_HOUR vs. 3600000 (time in milliseconds)
```javascript
setTimeout(stopTimer, ONE_HOUR) //immediately clear how long the for the function to run. 

setTimeout(stopTimer, 3600000) //while valid, this will require you to search how long 3600000 milliseconds are. 

```

## comments
comments should explain the why for you code. If you follow clean code practices, descriptive names, consistent vocabulary, etc, your code will explain whats going on pretty clearly. comments can act as a way to explain why its happening to provide context. Even so, there might be instances where an action written in code, may not be intuitive to everybody, so writing a comment would be a non-issue to add to provide the needed context. 