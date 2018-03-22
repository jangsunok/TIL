
# DOM (Document Object Model)

DOM은 Html, Xml 등의 웹페이지 문서를 Object로 접근할수 있게 해주는 인터페이스(모델)

> With the object model, JavaScript gets all the power it needs to create dynamic HTML:

> - JavaScript can change all the HTML elements in the page
- JavaScript can change all the HTML attributes in the page
- JavaScript can change all the CSS styles in the page
- JavaScript can remove existing HTML elements and attributes
- JavaScript can add new HTML elements and attributes
- JavaScript can react to all existing HTML events in the page
- JavaScript can create new HTML events in the page

```html
<!DOCTYPE html>
<html>
<body>
    <input type="button" onclick="alert(window.location)" value="alert(window.location)" />
    <input type="button" onclick="window.open('bom.html')" value="window.open('bom.html')" />
</body>
</html>
```



# BOM (Browser Object Model)
BOM은 웹페이지의 내용을 제외한, 브라우져를 Object로 접근할수 있게 해주는 인터페이스(모델)


```html
<!DOCTYPE html>
<html>
<body>
    <img src="..." />
    <img src="..." />
    <script type="text/javascript">
        // body 객체
        console.log(document.getElementsByTagName('body')[0]);
        // 이미지 객체들의 리스트
        console.log(document.getElementsByTagName('body'));
    </script>
</body>
</html>
```



![Alt text](http://learn.javascript.ru/article/browser-environment/windowObjects@2x.png)

Window 최상위 객체를 통해 document, screen, location, history, navigator등을 제어가 가능하다.
