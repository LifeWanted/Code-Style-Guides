
# JavaScript #

## Spacing ##

### Use Spaces (Soft Tab), Not Tabs (Hard Tab) ###
```js
// Good
var aVar        = 123;
var otherVar    = “another”;

// Bad
var aVar		= 123; // Note hard tabs.
var otherVar	= “another”;
```

### Align at 4-character ###
```js
// Good
var aVar        = 123; // Note aligned at 16th column.
var otherVar    = “another”;

// Bad
var aVar      = 123; // Note aligned at 14th column.
var otherVar  = “another”;
```

## Variables ##

### One Variable Per `var` ###
```js
// Good
var foo = 123;
var bar = “another”;

// Bad
var foo = 123,
    bar = “another”;

// Bad
var foo = 123
  , bar = “another”
  ;
```

### Align at the Equal Sign Using Tab-Stops ###
```js
// Good
var aVariable       = 123;
var otherVariable   = “another”;

// Bad
var aVariable = 123;
var otherVariable = “another”;

// Bad
var aVariable     = 123;
var otherVariable = “another”;

// Bad
var aVariable =     123;
var otherVariable = “another”;
```

## Operators ##

### At Least One Space Either Side of Operator ###
```js
// Good
foo = “value”;

// Bad
foo=”value”;

// Bad
foo= ”value”;

// Bad
foo =”value”;
```

## Conditionals and Loops ##

### Always Wrap Body in Braces ###
```js
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
```js
// Good
while( condition ){
    doSomething();
}

// Bad
while( condition ){ doSomething(); }
```

### Open Brace On Keyword Line ###
```js
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
```js
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
```js
// Good
if( someVar == true ){
    // Do something.
}
aFunc( param );

// Bad
if(someVar == true){
    // Do something.
}
aFunc(param);
```

### No Space Outside Next To Keywords ###
```js
```

## Object Literals ##

### Opening Brace On Line With Variable or Function ###
```js
// Good
var foo = {
    field1 : 123,
    field2 : “another”
};
someFunction({
    field1 : 123,
    field2 : “another”
});

// Okay
var foo = { field1 : 123 }; // Note only 1 field in object.
someFunction( { field : 123 } );

// Bad
var foo = { field1 : 123, field2 : “another” };
someFunction( { field1 : 123, field2 : “another” } );

// Bad
var foo =
    {
        field1 : 123,
        field2 : “another”
    };
someFunction(
    {
        field1 : 123,
        field2 : “another”
    }
);
```

### Align on the Colon Using Tab-Stops ###
```js
// Good
var obj = {
    aField          : 123,
    anotherField    : “another”
};

// Bad
var obj = {
    aField : 123,
    anotherField : “another”
};

// Bad
var obj = {
    aField       : 123,
    anotherField : “another”
};

// Bad
var obj = {
    aField :        123,
    anotherField :  “another”
};
```

## Functions ##

### Align Consecutive Calls ###
```js
// Good
var foo         = require( “foo”        );
var other       = require( “other”      );
var something   = require( “something”  );

// Good
var foo         = fooFunc(      “foo”       );
var other       = otherFunc(    “other”     );
var something   = someFunc(     “something” );

// Okay
var foo         = require( “foo” );
var other       = require( “other” );
var something   = require( “something” );

// Bad
var foo         = fooFunc( “foo” );
var other       = otherFunc( “other” );
var something   = someFunc( “something” );
```

### Separate Definitions With A Horizontal Line ###
```js
// Good
function foo(){
    doSomeStuff();
}

// ---------------------------------------------------------------------------------------------- //

function bar(){
    doOtherStuff();
}

// Good
var AClass = (function(){
    function AClass(){
    }
    
    // ------------------------------------------------------------------------------------------ //

    AClass.prototype.aMethod = function(){
        doStuff();
    };
    
    // ------------------------------------------------------------------------------------------ //
    
    return AClass;
})();

// Bad
function foo(){
    doSomeStuff();
}

function bar(){
    doOtherStuff();
}
```

## Classes ##

## Documentation and Comments ##

### Use JSDoc-Style Documentation ###
```js
```

### Use C++-Style Comments ###
```js
```

### Put a Comment Every 4-8 Lines ###
```js
```

## Miscellany ##

### Always End Lines With Semicolon ###
```js
```

### Use CamelCase Naming ###
```js
```
