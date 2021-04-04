# Blue-Topaz_Obsidian-css

蓝色托帕石不是贵重的宝石，以契合“黑曜石”😜。另外蓝色托帕石一般由无色或浅色黄玉经过人工处理后得到——这个主题不是我从零开始做出来的，而是大量借鉴了他人的主题后，修改而成的，就像蓝色托帕石一样，是后天人造的。在此，感谢所有共享了css文件的人。另外，“无色或浅色黄玉”没有任何暗喻的意思，也没有和别人的主题做比较的意思。如果你能喜欢这个主题，那就很好！

A blue theme for **Obsidian**. Blue Topaz is not a precious gem, like obsidian😜. Generally, Blue Topaz is obtained by artificially treating colourless topaz. Likewise，I did not make this theme from scratch, but modified it after borrowing others' themes. It is like Blue Topaz, which is a modified product. Thus, thanks for the all shared themes, which inspired me indeed! BTW, For the word "colourless topaz", there is no offence and no comparison. And it is not a metaphor. I will be glad if you enjoy the theme, *Blue Topaz*.

# Preview
![](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css/blob/master/preview_Blue%20Topaz.png)

```
===========================    TIPS   ===============================
====================================================================
===========主题中的一些特别样式 Special parts in this theme===========
=====================================================================
```
```
==========================
=====标签 Special tags=====
==========================
#dailynote
#weeklynote
#important
#重要
#inprogress
#进行中
#complete
#完成
#questions
#ideas
```
```


==========================
========图片 images========
==========================
用法

在图片末尾加上 “|left” 或 “|right” 可以让图片左或右对齐
xxx.jpg|left

-------------------
可用变体：
left/Left/LEFT/L
right/Right/RIGHT/R

如：xxx.png|L
-------------------


如果同时调整图片大小，需要把调整大小的数值放在最后
xxx.png|right|200

使用 “|inlineL” 或 “|inlineR” 可以将图片嵌入在文字中,L左，R右
xxx.png|inlineL

-------------------
可用变体：
inlineL/InlineL/INLINEL/inlL
inlineR/InlineR/INLINER/inlR

如：xxx.png|inlR
-------------------

Usage

Typing "|left" or "|right" at the end of the image file can make the image shown on left or right.
For example,
xxx.jpg|left

---------------------------
The variants you can use：
left/Left/LEFT/L
right/Right/RIGHT/R

e.g. xxx.png|L
---------------------------

You can also change the image size with the position. You should put the "|number" at the end.
For example,
xxx.png|right|200 


Use "inlineL" or "inlineR" to embed the image on the left or right.
xxx.png|inlineL

-----------------------------
The variants you can use：
inlineL/InlineL/INLINEL/inlL
inlineR/InlineR/INLINER/inlR

e.g. xxx.png|InlL
-----------------------------

===========================
=====笔记框 Note blocks=====
===========================

----------------------------------------------------------------------
---------------不同颜色背景 Colourful note backgrounds-----------------
----------------------------------------------------------------------
语法：```note-xxx-bg 或```note-xxx-background
---------------------------------------------

```note-orange-bg

```note-yellow-bg

```note-green-bg

```note-blue-bg

```note-purple-bg

```note-pink-bg

```note-red-bg

```note-gray-bg

```note-brown-bg

-----------------------------------------------------
----------不同笔记颜色 Colourful note texts------------
-----------------------------------------------------

```note-orange

```note-yellow

```note-green

```note-blue

```note-purple

```note-pink

```note-red

```note-gray

```note-brown

-----------------------------------------------------------
------------记忆笔记框 Recall/cloze note blocks-------------
-----------------------------------------------------------
可鼠标点击显示笔记内容 To show text by clicking
-----------------------------------------------------------

```note-cloze

--------------------------------------------------------
------------重要笔记框 important note blocks-------------
--------------------------------------------------------
有笔记外框 Different block style
--------------------------------------------------------

```note-imp

```



```
=========================
=======列表 list=========
=========================


=========================================
================stickies=================
=========================================
手动输入以下格式，可以得到不同的样式
```
<p class="stickies"\> 你自己的文字 </p>
<p class="stickies2"\> 你自己的文字 </p>
<p class="to-recall"\> 你自己的文字 </p>
```

USAGE
Typing the following formats, you can obtain some special styles.
```
<p class="stickies"\> Your words </p>
<p class="stickies2"\> Your words </p>
<p class="to-recall"\> Your words </p>
```


```
=============================
==== <aside> </aside> =======
=============================
```

thanks to dcoales from obsidian member group on discord  
https://discord.com/channels/686053708261228577/702656734631821413/794236352857374764

Use 
```
<aside><h1> Your words </h1></aside>
<aside><h2> Your words </h2></aside>
```
to get a right-side note block


---

## BTW
```css
/* Blockquote header */
.markdown-preview-view blockquote {
  position: relative; /* for pseudos */
  color: var(--theme-color);
  font-size: 1rem;
  font-weight: normal;
  line-height: 1.5;
  margin: 0;
  border: 3px solid;
  border-radius:20px;
  padding: 10px 15px;
  background: var(--background-primary);
}

.theme-dark .markdown-preview-view blockquote {
  background-color: var(--background-primary) !important;
}

.markdown-preview-view blockquote p{
 color: var(--text-normal);
 font-size: 16px;
}

.markdown-preview-view blockquote:after {
  content:"";
  position: absolute;
  border: 3px solid var(--theme-color);
  border-radius: 35px 0 0 0;
  width: 50px;
  height: 55px;
  bottom: -58px;
  left: 25px;
  border-bottom: none;
  border-left: none;
  border-right: none;
  z-index: 3; 
}

.markdown-preview-view blockquote:before {
  content:"";
  position: absolute;
  width: 25px;
  border: 10px solid var(--background-primary);
  bottom: -7px;
  left: 20px;
  z-index: 2;
}
```
![](https://github.com/whyt-byte/Blue-Topaz_Obsidian-css/blob/master/blockquote.jpg?raw=true)

---

By Klaas from Discord group
```css
div:not(.CodeMirror-activeline)>.HyperMD-quote>span:first-of-type::before {
  content: '“' !important;
  font: 14px/20px italic Times, serif;
  font-weight: 700;
  font-size: 3em; /* PB changed from 18px */
  color: var(--text-accent);
  left: 3px;
  top: 15px;
  position: relative;
}
```
