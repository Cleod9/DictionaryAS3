# Dictionary Util for AS3 #

This is a simple typed Dictionary Class for AS3. It maps strings to objects of a given type. (To allow any type to be mapped, pass "Object" as the class type instead)

### Minimum required classes for using this utility: ###

- com.mcleodgaming.util.Dictionary

## Instructions ##

Copy the included **com** folder to your project's root code directory, and add the import to the top of your classes that will be using it:

```as3
import com.mcleodgaming.util.Dictionary;
```

Then create a new Dictionary Object like so:


```as3
//Creates a Dictionary of type int
var myDict:Dictionary = new Dictionary(int);
```

Once initiated, following the above example you are then able to use the following functions through `myDict`:

`length` - Property that returns an `int` indicating the number of items inside of the Dictionary.

`Keys` - Property that returns an Array of keys used in the Dictionary. Keys will always be of type `String`

`Values` - Property that returns an Array of the values inside of the Dictionary. The values will have the same type as the one that was provided on initialization of the Dictionary. (in the above example, that would be `int`)

`push(key:String, obj:*):Boolean` - Adds `obj` to the Dictionary associated with the provided `key` String. If the provided `obj` does not match the declared Dictionary type, the object will not be added and an error will be traced.

`pop():*` - Pops the last object from the end of the dictionary.

`remove(key:String):*` - Removes an object from the array associated with the specified `key`

`getValue(value:*):String` - Returns a key specified by a given `value`

`getKey(key:String):*` - Returns a value specified by a given `key`

`renameKey(key:String, newKey:String):Boolean` - Renames a `key` to `newKey` while maintaining the association with its object.

`setKey(key:String, obj:*):void` - Sets `key` to a new value, or adds the key if it does not exist.

`containsKey(key:String):Boolean` - Returns `true` if the specified `key` exists in the Dictionary, `false` otherwise.

`containsValue(value:*):Boolean` - Returns `true` if the specified `value` exists in the Dictionary, `false` otherwise. 

`clear():void` - * Removes all values and keys from the dictionary

See the included `Main.as` file for a more specific example of the code in action.

## Terms of Use ##

Free to use in any projects without notifying me, nor is credit needed (though it'd be much appreciated!). Just do not re-distribute it under anyone else's name and be sure to retain the copyright notice in the source!

----------

Copyrighted © 2013 by Greg McLeod

GitHub: [https://github.com/cleod9](https://github.com/cleod9)