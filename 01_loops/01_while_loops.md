We can use a loop to execute a block of code multiple times, and our first type of loops is a `while` loop.

The syntax of a while loop looks like this:

```dart
void main() {
    while (condition) {
        // do something
    }
}
```

Looks similar to an if statement, let's write our first loop:

```dart
var i = 1;

while (i < 5) {
    print(i);
}
```

Don't run your code!, as you see, our condition will resolve to true, and as we told dart, `while` this is `true` `print` the value of `i`.

So once you run your code, dart will print `i` non stop, and may crash your ide or even your computer, and that's whats called an `infinite loop`, because it runs forever!

Always before you right your loop, think about how it's gonna end, so let's fix our loop:

```dart
var i = 1;

while (i < 5) {
    print(i);
    i++;
}
```

So here we told dart to increament the value of `i` by one with each iteration, what is an iteration?

let's get again into the brain of dart and see how it thinks and evaluates our code:

We have an integer called `i` with the value of `1`, `while` 1 is less than `5`, and that's `true`, excute a print statement for the value of `i` and then increament it by `1`.

So `i` is now equal to `2`, and we finished an `iteration`.

The condition will be checked again to see if It should keep going or It should stop and exit the loop.

The second iteration starts: Is `2` less than `5`? that's `true` so `print` `i` and go for another iteration...

[later]

Last iteration: `i` is now equal to `5`, is `5` less than `5`? `false`, so dart will stop and exit the loop.

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

while (i =< 5) {
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
