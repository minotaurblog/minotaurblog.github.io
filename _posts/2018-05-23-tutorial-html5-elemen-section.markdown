---
layout: post
title: Tutorial HTML5 - Elemen &lt;section&gt;
date: 2018-05-23 16:20:32 +0700
description: Mengenal Elemen section Beserta Atribut dan Fungsinya
img: section.jpg
tags: [HTML5]
---
Elemen <code>section</code> digunakan untuk mengelompokkan bagian-bagian dari dokumen atau apliksi. Tiap bagian biasanya disertai dengan sebuah heading.

Contoh dimana digunakan elemen <code>section</code> yaitu bab buku dan tab halaman HTML. Sebuah halaman depan Web dapat dibagi menjadi beberapa bagian seperti pengenalan, elemen-elemen berita, dan informasi kontak.

Di dalam elemen <code>section</code> dapat mengandung beberapa elemen <code>section</code>.

<pre>
<code data-language="html">&lt;div class="tabbed"&gt;
 &lt;!-- first panel --&gt;
 &lt;input name="tabbed" id="tabbed1" type="radio" checked&gt;
 &lt;section&gt;
   &lt;h1&gt;
     &lt;label for="tabbed1">&lt;!-- heading --&gt;&lt;/label&gt;
   &lt;/h1&gt;
   &lt;div&gt;
   &lt;!-- content --&gt;
   &lt;/div&gt;
 &lt;/section&gt;

 &lt;!-- second panel --&gt;
 &lt;input name="tabbed" id="tabbed2" type="radio"&gt;
 &lt;section&gt;
   &lt;h1&gt;
     &lt;label for="tabbed2"&gt;&lt;!-- heading --&gt;&lt;/label&gt;
   &lt;/h1&gt;
   &lt;div&gt;
   &lt;!-- content --&gt;
   &lt;/div&gt;
 &lt;/section&gt;

 &lt;!-- and so on -->
&lt;/div&gt;</code>
</pre>