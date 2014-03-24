# C++ #

## Spacing ##

### Use Spaces (Soft Tab), Not Tabs (Hard Tab) ###
```cpp
```

### Align at 4-character ###
```cpp
```

## Variables ##

### One Variable Per Definition ###
```cpp
```

### Align at the Equal Sign Using Tab-Stops ###
```cpp
```

## Operators ##

### At Least One Space Either Side of Operator ###
```cpp
```

## Conditionals and Loops ##

### Always Wrap Body in Braces ###
```cpp
// Good
if( condition ){
    doSomething();
}

// Bad
if( condition )
    doSomething();

// Bad
if( condition ) doSomething();
```

### Body Gets Own Lines ###
```cpp
// Good
while( condition ){
    doSomething();
}

// Bad
while( condition ){ doSomething(); }
```

### Open Brace On Keyword Line ###
```cpp
// Good
for( condition ){
    doSomething();
}

// Bad
for( condition )
{
    doSomething();
}
```

### Closing Brace Gets Own Line ###
```cpp
// Good
if( condition ){
    doSomething();
}
else {
    doSomethingElse();
}

// Bad
if( condition ){
    doSomething();
} else {
    doSomethingElse();
}

// Bad
if( condition )
{
    doSomething();
} else
{
    doSomethingElse();
}
```

## Parentheticals ##

### At Least One Space Inside ###
```cpp
```

### No Space Outside Next To Keywords ###
```cpp
```

## Functions ##

### Align Consecutive Calls ###
```cpp
```

### Separate Definitions With A Horizontal Line ###
```cpp
```

## Classes ##

## Documentation and Comments ##

### Use Doxygen Documentation ###
```cpp
```

### Use C++-Style Comments ###
```cpp
```

### Put a Comment Every 4-8 Lines ###
```cpp
```

## Miscellany ##

### Use CamelCase Naming ###
```cpp
```
