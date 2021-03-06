# $last projection

> Returns the last element of a list inside of a structure addressed by `path`

## Signature

**path** *(String/Array)* - Path to the list

**subject** *(Object)* - The object that contains the requested value

**TYPE SIGNATURES**
```
String -> Object -> *
(String, Object) -> *
Array -> Object -> *
(Array, Object) -> *
```

**EXAMPLE**
```js
const myObject = {
	rooms: {
		kitchen: {
			refrigerator: [
				'eggs',
				'beer',
				'milk'
			]
		}
	}
};

$last('rooms.kitchen.refrigerator', myObject); // returns 'milk'
```

**IMMUTABLE JS SUPPORT**
*the following types are supported for values targeted by `path`*:
```
Iterable.Indexed
Iterable.Keyed
Iterable.Set
```
