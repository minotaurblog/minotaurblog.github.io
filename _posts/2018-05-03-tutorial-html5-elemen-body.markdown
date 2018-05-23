---
layout: post
title: Tutorial HTML5 - Elemen &lt;body&gt;
date: 2018-05-03 20:26:20 +0700
description: Mengenal Elemen body Beserta Atribut dan Fungsinya
img: body.jpg
tags: [HTML5]
---
Elemen <code>body</code> sebagai tempat isi dokumen berada.

##### Atribut <code>onafterprint</code>
Eksekusi script javascript setelah klik tombol print pada Print Dialogue Box Browser

<pre>
<code data-language="html">&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body onafterprint="myFunction()"&gt;

&lt;h1&gt;Coba print dokumen tersebut&lt;/h1&gt;
&lt;p&gt;&lt;b&gt;Tip:&lt;/b&gt; Shortcut keyboard, Ctrl+P.&lt;/p&gt;
&lt;p&gt;&lt;b&gt;Note:&lt;/b&gt; Browser Safari dan Opera tidak mendukung atribut tersebut.&lt;/p&gt;

&lt;script&gt;
function myFunction() {
   alert("This document is now being printed");
}
&lt;/script&gt;

&lt;/body&gt;
&lt;/html&gt;</code>
</pre>

##### Atribut <code>onbeforeprint</code>
Eksekusi script javascript sebelum Print Dialogue Box Browser muncul.

<pre>
<code data-language="html">&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;body onafterprint="myFunction()"&gt;

&lt;h1&gt;Coba print dokumen tersebut&lt;/h1&gt;
&lt;p&gt;&lt;b&gt;Tip:&lt;/b&gt; Shortcut keyboard, Ctrl+P.&lt;/p&gt;
&lt;p&gt;&lt;b&gt;Note:&lt;/b&gt; Browser Safari dan Opera tidak mendukung atribut tersebut.&lt;/p&gt;

&lt;script&gt;
function myFunction() {
   alert("This document is now being printed");
}
&lt;/script&gt;

&lt;/body&gt;
&lt;/html&gt;</code>
</pre>

##### Atribut <code>onbeforeunload</code>
Eksekusi javascript saat dokumen akan direload atau direfresh atau ditutup.

##### Atribut <code>onresize</code>
Eksekusi javascript saat browser diminimize atau dimaximize.
