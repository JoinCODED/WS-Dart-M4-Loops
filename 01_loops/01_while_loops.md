We can use a loop to execute a block of code multiple times. There are many types of loops. We're gonna get into the first type, which is a `while` loop:

The syntax of a `while` loop looks like the following:

```dart
void main() {
    while (condition) {
        // do something
    }
}
```

It looks similar to an `if statement`. Let's write our first loop:

```dart
var i = 1;

while (i < 5) {
    print(i);
}
```

Don't run your code! As you can see, our condition will resolve to true, and as we told Dart, `while` this is `true`, `print` the value of `i`.

Once you run your code, Dart will print `i` non stop, and may crash your IDE or even your computer. That's called an `infinite loop`, because it runs forever!

Always, before you write your loop, think about how it's going to end. Let's fix our loop:

```dart
var i = 1;

while (i < 5) {
    print(i);
    i++;
}
```

Here, we told Dart to increment the value of `i` by one with each iteration.

What is an iteration?
Let's get again into the brain of Dart and see how it thinks and evaluates our code:

We have an integer called `i` with the value of `1`. `while` 1 is less than `5`, Dart will execute the print statement for the value of `i` and then increment it by `1` till it reaches the value 2, then the iteration will stop.

The condition will be checked again to see if it should keep going or stop and exit the loop.

The second iteration starts: Is `2` less than `5`? If so, `print` `i` and go for another iteration...

Last iteration: `i` is now equal to `5`, and it's not less than `5`, so the result will evaluate to `false`, and Dart will stop and exit the loop.

Output:

```
1
2
3
4
```

Let's make this more interesting:

```dart
var i = 1;

while (i <= 5) {
    print("x" * i);
    i++;
}
```

Output:

```
x
xx
xxx
xxxx
xxxxx
```

Cool we have a stair...
