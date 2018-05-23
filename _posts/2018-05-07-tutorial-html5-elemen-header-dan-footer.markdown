---
layout: post
title: Tutorial HTML5 - Elemen &lt;header&gt; dan &lt;footer&gt;
date: 2018-05-07 10:54:20 +0700
description: Mengenal Elemen header dan footer Beserta Atribut dan Fungsinya
img: header.jpg
tags: [HTML5]
---
Elemen <code>header</code> berfungsi sebagai konten pengantar halaman web yang terdiri dari logo, form pencarian dan deretan hyperlink untuk navigasi. Elemen <code>header</code> juga berfungsi sebagai konten pengantar artikel yang berisi judul, tanggal, pembuat artikel, waktu dibuat dll. Dalam satu dokumen dapat terdapat beberapa elemen <code>header</code>.

<pre>
<code data-language="html">&lt;header&gt;
   &lt;div id="logo"&gt;Rocking Stone&lt;/div&gt;
   &lt;nav&gt;...&lt;/nav&gt;
 &lt;/header&gt;</code>
</pre>

<pre>
<code data-language="html">&lt;article&gt;
 &lt;header&gt;
   &lt;h1&gt;Google Buys Nest&lt;/h1&gt;
   &lt;p&gt;Posted at 11:34am 13th January 2014&lt;/p&gt;
 &lt;/header&gt;
 &lt;p&gt;...&lt;/p&gt;
 &lt;p&gt;...&lt;/p&gt;</code>
</pre>

Elemen <code>footer</code> biasanya berisi nama penulis dokumen, informasi hak cipta, tautan ke ketentuan penggunaan, informasi kontak, dll.

<pre>
<code data-language="html">&lt;article class="film_review"&gt;
  &lt;header&gt;
    &lt;h2&gt;Jurassic Park&lt;/h2&gt;
  &lt;/header&gt;
  &lt;section class="main_review"&gt;
    &lt;p&gt;Dinos were great!&lt;/p&gt;
  &lt;/section&gt;
  &lt;footer&gt;
    &lt;p&gt;
      Posted on
      &lt;time datetime="2015-05-15 19:00"&gt;May 15&lt;/time&gt;
      by Staff.
    &lt;/p&gt;
  &lt;/footer&gt;
&lt;/article&gt;</code>
</pre>