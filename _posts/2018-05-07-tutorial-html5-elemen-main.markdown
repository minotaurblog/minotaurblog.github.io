---
layout: post
title: Tutorial HTML5 - Elemen &lt;main&gt;
date: 2018-05-07 10:14:20 +0700
description: Mengenal Elemen main Beserta Atribut dan Fungsinya
img: main.jpg
tags: [HTML5]
---
Elemen <code>main</code> mewakili konten utama dari tubuh dokumen atau aplikasi. Dalam sebuah dokumen tidak boleh mengandung lebih dari satu elemen <code>main</code> kecuali memiliki atribut <code>hidden</code> untuk elemen <code>main</code> lainnya. Elemen <code>main</code> hanya dapat memiliki induk elemen seperti <code>html</code>, <code>body</code>, <code>div</code> dan <code>form</code>. Elemen <code>main</code> tidak boleh merupakan anak elemen dari <code>article</code>, <code>aside</code>, <code>header</code>, <code>footer</code> atau <code>nav</code>.

<pre>
<code data-language="html">&lt;main&gt;
 &lt;h1&gt;Web Browsers&lt;/h1&gt;
 &lt;p&gt;Google Chrome, Firefox, and Internet Explorer are the most used browsers today.&lt;/p&gt;

 &lt;article&gt;
   &lt;h1&gt;Google Chrome&lt;/h1&gt;
   &lt;p&gt;Google Chrome is a free, open-source web browser developed by Google,
   released in 2008.&lt;/p&gt;
 &lt;/article&gt;

 &lt;article&gt;
   &lt;h1&gt;Internet Explorer&lt;/h1&gt;
   &lt;p&gt;Internet Explorer is a free web browser from Microsoft, released in 1995.&lt;/p&gt;
 &lt;/article&gt;

 &lt;article&gt;
   &lt;h1&gt;Mozilla Firefox&lt;/h1&gt;
   &lt;p&gt;Firefox is a free, open-source web browser from Mozilla, released in 2004.&lt;/p&gt;
 &lt;/article&gt;
&lt;/main&gt;</code>
</pre>