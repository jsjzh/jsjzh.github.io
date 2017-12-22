---
title: sublime-emmet
date: 2017-12-22 14:54:20
tags:
categories:
---

<div class="blockquote-center">TODO一句话概括</div>

<!-- more -->

## 目录 ##

## 前言 ##

## 内容 ##

### 基础 ###

#### 后代: > ####
`div>ul>li`
```
<div>
    <ul>
        <li></li>
    </ul>
</div>
```

#### 兄弟: + ####
`div+p+bq`
```
<div></div>
<p></p>
<blockquote></blockquote>
```

#### 上级: ^ ####
`div+div>p>span+em^bq`
```
<div></div>
<div>
    <p><span></span><em></em></p>
    <blockquote></blockquote>
</div>
```

`div+div>p>span+em^^bq`
```
<div></div>
<div>
    <p><span></span><em></em></p>
</div>
<blockquote></blockquote>
```

#### 分组: () ####
`div>(header>ul>li*2>a)+footer>p`
```
<div>
    <header>
        <ul>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
        </ul>
    </header>
    <footer>
        <p></p>
    </footer>
</div>
```

`(div>dl>(dt+dd)*3)+footer>p`
```
<div>
    <dl>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
    </dl>
</div>
<footer>
    <p></p>
</footer>
```

#### 乘法: * ####
`ul>li*5`
```
<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

#### 自增符号: $ ####
`ul>li.item$*5`
```
<ul>
    <li class="item1"></li>
    <li class="item2"></li>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
</ul>
```

`h$[title=item$]{Header $}*3`
```
<h1 title="item1">Header 1</h1>
<h2 title="item2">Header 2</h2>
<h3 title="item3">Header 3</h3>
```

`ul>li.item$$$*5`
```
<ul>
    <li class="item001"></li>
    <li class="item002"></li>
    <li class="item003"></li>
    <li class="item004"></li>
    <li class="item005"></li>
</ul>
```

`ul>li.item$@-*5`
```
<ul>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
    <li class="item2"></li>
    <li class="item1"></li>
</ul>
```

`ul>li.item$@3*5`
```
<ul>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
    <li class="item6"></li>
    <li class="item7"></li>
</ul>
```
