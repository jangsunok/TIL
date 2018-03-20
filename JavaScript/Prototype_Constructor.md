# Prototype


All JavaScript objects inherit properties and methods from a prototype.



```js
function Person(first, last, age) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
}

Person.prototype.nationality = "Korean";
Person.prototype.name = function() {
    return this.firstName + " " + this.lastName;
};

var me  = new Person("SunOk", "Jang", 26);

console.log(me.firstName);  // => SunOk
console.log(me.nationality);  // => Korean
console.log(me.name());  // => SunOk Jang

me.nationality = "South Korean"
console.log(me.nationality);  // => South Korean

```



# Constructor

constructor 속성은 단순히 함수명을 나타내는 것이 아닌 **함수 객체에 대한 참조**


```js
var o = {};
o.constructor === Object; // true

var a = [];
a.constructor === Array; // true

var n = new Number(3);
n.constructor === Number; // true


console.log(me.constructor == Person.prototype.constructor); // true
console.log(me.constructor == Person); // true


```
