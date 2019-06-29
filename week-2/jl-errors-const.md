> paste [this markdown](https://raw.githubusercontent.com/janke-learning/error-exercises/master/const.md) into this file and fix the errors!      
> references: [errors & life-cycle](https://github.com/janke-learning/errors-and-life-cycle), [exercise repo](https://github.com/janke-learning/errors)
# Variable Errors


### exercises
* [missing variable name](#missing-variable-name)
* [reassigning to constant](#reassigning-to-constant)
* [unassigned const declaration](#unassigned-const-declaration)

---

### missing variable name

broken code:
```js
const = 5;
```
error message:
```js
Uncaught SyntaxError: Unexpected token =
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
var five = 5;
```
your notes:

[TOP](#variable-errors)

---


## reassigning to constant

broken code:
```js
const a = 9;
a = 0;
```
error message:
```js
Uncaught SyntaxError: Identifier 'a' has already been declared
TypeError: Assignment to constant variable.
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
const a = 9;

```
your notes:The variable identifier cannot be reassigned.

[TOP](#variable-errors)

---


## unassigned const declaration

broken code:
```js
const a;
a = 0;
```
error message:
```js
Uncaught SyntaxError: Missing initializer in const declaration
```
classification:
* creation phase or execution phase ?
* syntax or semanitc ?

the fix:
```js
const a = 0;
```
your notes:An initializer for a constant is required. You must specify its value in the same statement in which it's declared (which makes sense, given that it can't be changed later).

[TOP](#variable-errors)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
