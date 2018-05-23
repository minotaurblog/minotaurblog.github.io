---
layout: post
title: Tutorial HTML5 - Elemen &lt;base&gt;
date: 2018-05-02 21:31:20 +0700
description: Mengenal Elemen base Beserta Atribut dan Fungsinya
img: base.jpg
tags: [HTML5]
---
Elemen <code>base</code> berfungsi untuk menentukan base url dokumen HTML.

<table class="table">
  <thead>
    <tr>
      <th scope="col">Atribut</th>
      <th scope="col">Nilai</th>
      <th scope="col">Deskripsi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>href</code></td>
      <td>url</td>
      <td>Menentukan base url dari url relatif dalam dokumen HTML</td>
    </tr>
    <tr>
      <td rowspan="3"><code>target</code></td>
      <td><code>_blank</code></td>
      <td>Membuka hyperlink di jendela atau tab baru</td>
    </tr>
    <tr>
      <td><code>_self</code></td>
      <td>Membuka hyperlink di jendela yang sama dengan hyperlink</td>
    </tr>
    <tr>
      <td>frame name</td>
      <td>Membuka hyperlink di frame dengan atribut name</td>
    </tr>
  </tbody>
</table>

<pre>
<code data-language="html">&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
&lt;title&lt;This is an example for the &lt;base&gt; element&lt;/title&gt;
&lt;base href="https://www.example.com/news/index.html"&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;p&gt;Visit the &lt;a href="archives.html">archives&lt;/a&gt;.&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;</code>
</pre>

Link archives akan mengarahkan ke https://www.example.com/news/archives.html.