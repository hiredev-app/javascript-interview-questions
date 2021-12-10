![Image header](https://github.com/hiredev-app/javascript-interview-questions/blob/main/image-header.png?raw=true)

## Questions

<details>
<summary>What's a correct way to access a DOM element in JavaScript? | <i>Multi choice answer</i></summary>

- [x] getElementById(idName)
- [x] getElementsByClass(className)
- [ ] getElementByTagName(tagName)
- [x] querySelector()</details>

<details>
<summary>Which of the statements about "var" and "let" variables is correct? | <i>Single choice answer</i></summary>

- [ ] Variables of type "let" create a property on "global" object.
- [x] Variables of type "var" are hoisted, while "let" variables are not.
- [ ] Variables of type "var" are scoped to their immediate enclosing block.</details>

<details>
<summary>What's the difference between "===" and "==" equality operators? | <i>Multi choice answer</i></summary>

- [ ] Operator "===" performs deep equality check, while "==" performs shallow equality check.
- [ ] Both operators are the same.
- [x] Operator "==" performs type coercion before the equality check, while "===" does not.</details>

<details>
<summary>Which of these expressions return NaN? | <i>Multi choice answer</i></summary>

- [ ] Number("1")
- [x] Number("Number")
- [ ] 1 + "1"
- [x] parseInt("'1'")</details>

<details>
<summary>What's the difference between "null" and "undefined" in JavaScript? | <i>✎ Full text answer</i></summary>

</details>

<details>
<summary>What does the following snippet log into the console? | <i>Single choice answer</i></summary>

- [ ] one, two, three
- [ ] three, one, two
- [x] one, three, two
- [ ] two, one, three
~~~javascript 
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
~~~
</details>

<details>
<summary>What are the pros and cons of using Promises instead of callbacks? What other options do we have to handle async in JavaScript? | <i>✎ Full text answer</i></summary>

</details>

<details>
<summary>What is event bubbling in JavaScript? | <i>✎ Full text answer</i></summary>

</details>

<details>
<summary>What does nullish-coalescing operator do? | <i>Multi choice answer</i></summary>

- [x] It returns right-side operator in case left-side operator is undefined.
- [ ] It returns right-side operator in case left-side operator is falsy.
- [x] It returns right-side operator in case left-side operator is null.
- [ ] It returns left-side operator in case right-side operator in undefined.</details>

<details>
<summary>Is following code-snippet ES6 correct? If it is, what does it perform? | <i>Single choice answer</i></summary>

- [ ] The statement is correct. It creates a two-dimensional array.
- [ ] The statement is not correct.
- [x] The statement is correct. It swaps values of variables x and y.
- [ ] The statement is correct. It does nothing at all though.
~~~javascript
var x = "Foo";
var y = "Bar";
[x, y] = [y, x];
~~~
</details>
