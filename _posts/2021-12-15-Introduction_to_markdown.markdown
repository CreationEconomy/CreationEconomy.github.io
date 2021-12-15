---
layout: post
title:  "Markdown 소개"
date:   2021-12-14 14:34:25
categories: IT
tags: introduction
image: /assets/article_images/2014-11-30-mediator_features/night-track.JPG
image2: /assets/article_images/2014-11-30-mediator_features/night-track-mobile.JPG
comments: true
---

# 마크다운(Markdown) 이란
<br>
마크다운은 일반 텍스트로 서식을 가지는 문서를 작성하는 방법이다.
이 블로그도 마크다운 문서를 기반으로 빌드 되었다.

# 마크다운 문법

## 1. Header
제목을 작성할 때 사용되며 #의 개수에 따라 H1~H6로 나뉜다. <br>
#이 많을수록 크기가 작아지는 것을 볼 수 있다.


>
\# H1 <br>
\## H2 <br>
\### H3 <br>
\#### H4 <br> 
\##### H5 <br>
\###### H6 <br>

>
# H1
## H2
<br>
### H3
<br>
#### H4
<br>
##### H5
<br>
###### H6

---
## 2. Italic
텍스트를 강조하고자 할 때 사용된다.
>
\*italic* <br>
\_italic_ <br>
\**bold** <br>
\__bold__ <br>
\~~StrikeThrough~~ <br>

>
*italic* <br>
_italic_ <br>
**bold** <br>
__bold__ <br>
~~StrikeThrough~~

## 3. Link
외부 사이트의 링크를 표시하고자 할 때 사용된다. <br>
>
\[Links](https://creationeconomy.github.io/) <br>
\[Links with title](https://creationeconomy.github.io/ "link title") <br>
\`\<link>` : <https://creationeconomy.github.io/> <br>

>
[Links](https://creationeconomy.github.io/) <br>
[Links with title](https://creationeconomy.github.io/ "link title") <br>
`<link>` : <https://creationeconomy.github.io/> <br>

## 4. Code Block
글에 코드를 삽입할 때 사용된다.

>
\`\`\`python <br>
def test(a, b): <br>
&nbsp;&nbsp;&nbsp;&nbsp; print("hello World!") <br>
&nbsp;&nbsp;&nbsp;&nbsp; return a+b <br>
\`\`\`

```python
def test(a, b):
    print("hello World!")
    return a+b
```
>
\`\`\`html <br>
\<!DOCTYPE html> <br>
\<html> <br>
&nbsp;&nbsp;&nbsp;&nbsp;\<head> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\<mate charest="utf-8" /> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\<title>Hello world!</title> <br>
&nbsp;&nbsp;&nbsp;&nbsp;\</head> <br>
&nbsp;&nbsp;&nbsp;&nbsp;\<body> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\<h1>Hello world!</h1> <br>
&nbsp;&nbsp;&nbsp;&nbsp;\</body> <br>
\</html> <br>
\`\`\`

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Hello world!</title>
    </head>
    <body>
        <h1>Hello world!</h1>
    </body>
</html>
```

## 4. Image
글에 이미지를 삽입할 때 사용된다.

>\!\[](이미지 URL)

<br>

>![](https://cdn.pixabay.com/photo/2021/12/10/19/17/prague-6861273_960_720.jpg)