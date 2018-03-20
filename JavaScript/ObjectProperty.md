

# Object property


Object.defineProperty(object, propertyname, descriptor)



>**매개 변수**

>**object**  필수 요소.  속성을 추가 또는 수정할 개체입니다.  네이티브 JavaScript 개체(사용자 정의 개체 또는 기본 제공 개체) 또는 DOM 개체일 수 있습니다.  

>**propertyname** 필수 요소.  속성 이름을 포함하는 문자열입니다.  

>**descriptor** 필수 요소.  속성의 설명자입니다.  데이터 속성 또는 접근자 속성과 관련될 수 있습니다.  


## 데이터 속성 추가

```js
var newLine = "<br />";

// Create a user-defined object.
var obj = {};

// Add a data property to the object.
Object.defineProperty(obj, "newDataProperty", {
    value: 101,
    writable: true,
    enumerable: true,
    configurable: true
});

// Set the property value.
obj.newDataProperty = 102;
document.write("Property value: " + obj.newDataProperty + newLine);

// Output:
// Property value: 102
```


## 접근자 속성 추가

```js
var newLine = "<br />";

// Create a user-defined object.
var obj = {};

// Add an accessor property to the object.
Object.defineProperty(obj, "newAccessorProperty", {
    set: function (x) {
        document.write("in property set accessor" + newLine);
        this.newaccpropvalue = x;
    },
    get: function () {
        document.write("in property get accessor" + newLine);
        return this.newaccpropvalue;
    },
    enumerable: true,
    configurable: true
});

// Set the property value.
obj.newAccessorProperty = 30;
document.write("Property value: " + obj.newAccessorProperty + newLine);

// Output:
// in property set accessor
// in property get accessor
// Property value: 30

```
