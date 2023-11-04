# Demo CSS Tutorial
This tutorial will introduce you to some fun animations you can do with HTML and CSS.

1) Lets start by opening [codepen](https://codepen.io/) and creating a login with your google account.
2) Now add some text to a paragraph tag
```html
<p>
  The Caterpillar and Alice looked at each other for some time in silence: at
  last the Caterpillar took the hookah out of its mouth, and addressed her in a
  languid, sleepy voice.
</p>
```
3) You can change the color of the text by putting in some CSS to change the color for all p tags
```
p {
  color:red;
}
```
4) But there is a lot more you can do.  Lets get the text to move inside the p styling in the CSS file.  We will define an animation called slidein that scales the margins, width and font-size.
```
p {
  color:red;
  animation-duration: 3s;
  animation-name: slidein;
  animation-iteration-count: infinite;
}

@keyframes slidein {
  from {
    margin-left: 100%;
    width: 300%;
  }

  75% {
    font-size: 300%;
    margin-left: 25%;
    width: 150%;
  }

  to {
    margin-left: 0%;
    width: 100%;
  }
}
```
