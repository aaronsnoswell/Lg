# Lg - Simple(r) Android logging

This is a simple drop-in wrapper around the android Log class - it takes an
arbitrary number of Objects and calls `.toString()` on each of them. NULL is
also handled.

## Example

```java

// Logging example - no need to pass a logging tag
Lg.d("This is a log message");

// Accepts any number of objects
Lg.e("Oh noes! That was an error!", someException, status_code);

// Supports the Android d (Debug), i (Information), v (Verbose), e (Error) and w (Warn) tags
Lg.w("I'm warning you!, that was the last straw!");

```
