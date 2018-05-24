---
layout: post
title: Tutorial HTML5 - list
date: 2018-05-24 14:42:12 +0700
description: Mengenal Elemen ul, ol, li Beserta Atribut dan Fungsinya
img: list.jpg
tags: [HTML5]
---
#### Daftar tidak terurut
Elemen <code>ul</code> digunakan untuk membuat daftar tidak terurut.

<pre>
<code data-language="html">&lt;ul&gt;
 &lt;li&gt;first item&lt;/li&gt;
 &lt;li&gt;second item&lt;/li&gt;
 &lt;li&gt;third item&lt;/li&gt;
&lt;/ul&gt;</code>
</pre>

#### Daftar terurut
Elemen <code>ol</code> digunakan untuk membuat daftar terurut.

##### Atribut <code>reversed</code>
Atribut <code>reversed</code> berfungsi untuk membuat daftar dibalikkan urutannya.

<pre>
<code data-language="html">&lt;ol reversed&gt;
 &lt;li&gt;first item&lt;/li&gt;
 &lt;li&gt;second item&lt;/li&gt;
 &lt;li&gt;third item&lt;/li&gt;
&lt;/ol&gt;</code>
</pre>

Hasil output:

<ol reversed>
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ol>

##### Atribut <code>start</code>
Atribut <code>start</code> berfungsi untuk menentukan awal penomoran daftar.

<pre>
<code data-language="html">&lt;ol start="6"&gt;
 &lt;li&gt;first item&lt;/li&gt;
 &lt;li&gt;second item&lt;/li&gt;
 &lt;li&gt;third item&lt;/li&gt;
&lt;/ol&gt;</code>
</pre>

Hasil output:

<ol start="6">
  <li>first item</li>
  <li>second item</li>
  <li>third item</li>
</ol>

##### Atribut <code>type</code>
Atribut <code>type</code> berfungsi untuk menentukan tipe penomoran.

Nilai atribut <code>type</code> yang mungkin:
* <code>1</code>, penomoran menggunakan nomor (default)
* <code>a</code>, penomoran menggunakan huruf abjad kecil
* <code>A</code>, penomoran menggunakan huruf abjad besar
* <code>i</code>, penomoran menggunakan angka romawi kecil
* <code>I</ocde>, penomoran menggunakan angka romawi besar

#### Daftar bersarang
<pre>
<code data-language="html">&lt;ol&gt;
 &lt;li&gt;first item&lt;/li&gt;
 &lt;li&gt;second item
   &lt;ul&gt;
     &lt;li&gt;second item first subitem&lt;/li&gt;
     &lt;li&gt;second item second subitem&lt;/li&gt;
     &lt;li&gt;second item third subitem&lt;/li&gt;
   &lt;/ul&gt;
 &lt;/li&gt;
 &lt;li&gt;third item&lt;/li&gt;
&lt;/ol&gt;</code>
</pre>