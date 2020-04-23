
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

<p>NPM</p>

```html

   npm install wow.js
```
<p>在body前面貼上以下js<p/>

```js
var wow = new WOW(
  {
    boxClass:     'wow',      // 要套用WOW.js縮需要的動畫class(預設是wow)
    animateClass: 'animated', // 要"動起來"的動畫(預設是animated, 因此如果你有其他動畫library要使用也可以在這裡調整)
    offset:       0,          // 距離顯示多遠開始顯示動畫 (預設是0, 因此捲動到顯示時才出現動畫)
    mobile:       true,       // 手機上是否要套用動畫 (預設是true)
    live:         true,       // 非同步產生的內容是否也要套用 (預設是true, 非常適合搭配SPA)
    callback:     function(box) {
      // 當每個要開始時, 呼叫這裡面的內容, 參數是要開始進行動畫特效的element DOM
    },
    scrollContainer: null // 可以設定成只套用在某個container中捲動才呈現, 不設定就是整個視窗
  }
);
wow.init();
```
<h3>wow.js 進階設定</h3>
<p>
data-wow-duration: 突現秒數
data-wow-delay: 遲延秒數
data-wow-offset: 位移
data-wow-iteration: 重複次數(要一直重複的話可以用"infinite")</p>


<h3>Animations</h3>
<p>To animate an element, add the class animated to an element. You can include the class infinite for an infinite loop. Finally you need to add one of the following classes to the element:</p>


Class Name    |         |        |           |
------------  | ------- | ------ | ----------
`bounce`      | `flash` |`pulse` | `rubberBand`
 彈跳 | 閃爍    |放大再縮小原樣(上下)   | rubberBand:放大再縮小原樣(左右)
`wobble` | `jello` |`bounceIn`|`bounceInDown`
大力搖晃 | 果凍搖晃    |微彈跳   | 彈跳(從上往下跳)
>
