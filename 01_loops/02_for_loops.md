We are going to write the same code but using another way of creating loops, which is a `for` loop.

```dart
var i = 1;

while (i =< 5) {
    print("x" * i);
    i++;
}
```

```dart
for (var i = 1; i <= 5; i++){
    print("x" * i);
}
```

Syntax:

```dart
for (initialization; condition; increament) {
   //what to do in each iteration
}
```

We write the initialization, condition and increament code all in one line, so when to use a `while` loop and when to use a `for` loop? it's up to you, pick whatever you like.
