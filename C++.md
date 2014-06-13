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
// Good
int foo;
int bar;
int* biz;

// Bad (two variables listed on one line)
int foo, bar;
int* biz;

// Really bad (type of foo and bar hidden)
int* biz, foo, bar;
```

### Define Pointer Types with Asterisk by the Type ###
```cpp
// Good
int* somePtr;

// Bad (asterisk next to variable name)
int *somePtr;

// Bad (asterisk floating in the middle)
int * somePtr;
```

### Align at the Equal Sign Using Tab-Stops ###
```cpp
// Good
int some    = 2;
int var     = 234;
int anothr  = 16;

// Bad (not aligned)
int some = 2;
int var = 234;
int anothr = 16;

// Bad (not at a tab-stop)
int some   = 2;
int var    = 234;
int anothr = 16;
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

// Bad (no braces)
if( condition )
    doSomething();

// Bad (no brances, and on one line)
if( condition ) doSomething();
```

### Body Gets Own Lines ###
```cpp
// Good
while( condition ){
    doSomething();
}

// Bad (body on same line as condition)
while( condition ){ doSomething(); }
```

### Open Brace On Keyword Line ###
```cpp
// Good
for( condition ){
    doSomething();
}

// Bad (opening brace given own line, pushing the body away)
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
else if( otherCondition ){
    doSomethingElse();
}

// Bad (else-if crowding the if's body, hard to read)
if( condition ){
    doSomething();
} else if( otherCondition ){
    doSomethingElse();
}

// Bad (now you're just trying to piss me off)
if( condition )
{
    doSomething();
} else if( otherCondition )
{
    doSomethingElse();
}
```

## Parentheticals ##

### At Least One Space Inside, Unless Casting ###
```cpp
// Good
someFun( var, foo, bar );

// Good (casts are easier to read compressed)
int bar = 2;
double foo = (double)bar;

// Bad (function parameters crowded in, harder to read)
someFun(var, foo, bar);
```

### No Space Outside Next To Keywords ###
```cpp
// Good
while( condition ){
    doStuff();
}

// Bad (condition is distanced from the operation)
while ( condition ) {
    doStuff();
}
```

## Functions ##

### Align Consecutive Calls ###
```cpp
// Good
someFunc(   param   );
otherFunc(  param2  );

// Bad (mis-aligned parameters are harder to read)
someFunc( param );
otherFunc( param2 );

// Bad (not aligned on a tab-stop );
someFunc(  param  );
otherFunc( param2 );
```

### Separate Definitions With A Horizontal Line ###
```cpp
// Good
int foo( void ){
    return doStuff();
}

// ---------------------------------------------------------------------------------------------- //

void bar( int a ){
    doOtherStuff();
}
```

## Classes ##

## Documentation and Comments ##

### Use Doxygen Documentation ###
```cpp
// Good
/// @brief Does some awesome magical things.
///
/// @param parm     A variable acted upon.
/// @param parm2    Other variable acted upon.
///
/// @return Some stuff about the result.
int magicStuff( int parm, double parm2 ){
    return parm * parm2;
}
```

### Use C++-Style Comments ###
```cpp
// Good
// Only reject blue users.
if( user.color == "blue" ){
    reject( user );
}

// Bad (using C-style comment, annoying when trying to disable blocks of code for debugging.)
/* Only reject blue users. */
if( user.color == "blue" ){
    reject( user );
}
```

### Put a Comment Every 4-8 Lines ###
```cpp
```

## Miscellany ##

### Use CamelCase Naming ###
```cpp
// Good
class MyType {};
MyType myInstance;

// Bad (uses underscores instead of camel casing, harder to type)
class my_type {};
my_type my_instance;
```
