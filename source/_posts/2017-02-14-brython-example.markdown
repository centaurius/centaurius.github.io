---
layout: post
title: "Brython Example"
date: 2017-02-14 19:34:19 +0000
comments: true
categories: [python, coding]
published: true
---
<html>
<head>
<meta name="description" content="Hello world demo written in Brython www.brython.info">
<meta name="keywords" content="Python,Brython">
<meta name="author" content="Pierre Quentel">
<meta charset="iso-8859-1">
<script type="text/javascript" src="javascripts/brython.js"></script>
</head>

<body onload="brython()">
<script type="text/python">
from browser import document as doc
from browser import alert

def echo(*args):
    alert("Hello %s !" %doc["zone"].value)

doc["test"].bind("click", echo)
</script>
<p>Your name is: <input id="zone"><button id="test">click!</button>
</body>

</html>
