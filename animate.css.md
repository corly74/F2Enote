
<h1>Animate.css說明翻譯+WOW.js使用滑鼠移到該位置才開始動畫<h1>
  
   

  
  
  [Animate.css效果預覽](https://daneden.github.io/animate.css/)
  
 <h3>Animate Usage</h3>
<p>To use animate.css in your website, simply drop the stylesheet into your document's <head>, and add the class animated to an element, along with any of the animation names. That's it! You've got a CSS animated element. Super!</p>
  

```html
 <head>
  <link rel="stylesheet" href="animate.min.css">
</head> 
```

<p>
  or use a CDN hosted version by CDNJS </p>

```html
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.2/animate.min.css">
</head>
```

 <h3>WOW.js Usage</h3>
 
[WOW.js github](https://github.com/graingert/WOW)
<p<NPM</p>
```html

   npm install wow.js
```





<h3>Animations</h3>
<p>To animate an element, add the class animated to an element. You can include the class infinite for an infinite loop. Finally you need to add one of the following classes to the element:</p>


Class Name    |         |        |           |
------------  | ------- | ------ | ----------
`bounce`      | `flash` |`pulse` | `rubberBand`
 彈跳 | 閃爍    |放大再縮小原樣(上下)   | rubberBand:放大再縮小原樣(左右)
`wobble` | `jello` |`bounceIn`|`bounceInDown`
大力搖晃 | 果凍搖晃    |微彈跳   | 彈跳(從上往下跳)
