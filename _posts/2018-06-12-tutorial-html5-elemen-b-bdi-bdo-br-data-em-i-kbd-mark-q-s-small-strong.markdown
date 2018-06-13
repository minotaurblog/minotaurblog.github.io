---
layout: post
title: Tutorial HTML5 - Elemen &lt;b&gt;, &lt;bdi&gt;, &lt;bdo&gt;, &lt;br&gt;, &lt;data&gt, &lt;em&gt;, &lt;i&gt;, &lt;kbd&gt;, &lt;mark&gt;, &lt;q&gt;, &lt;s&gt;, &lt;small&gt;, &lt;strong&gt;
date: 2018-06-12 10:32:12 +0700
description: Mengenal Elemen &lt;b&gt;, &lt;bdi&gt;, &lt;bdo&gt;, &lt;br&gt;, &lt;data&gt, &lt;em&gt;, &lt;i&gt;, &lt;kbd&gt;, &lt;mark&gt;, &lt;q&gt;, &lt;s&gt;, &lt;small&gt;, &lt;strong&gt; Beserta Atribut dan Fungsinya
img: b.jpg
tags: [HTML5]
---
Elemen <code>b</code> digunakan untuk menandai kata yang perlu diperhatikan dengan membuat teks tebal.

<pre>
<code data-language="html">&lt;p&gt;This article describes several &lt;b class="keywords"&gt;text-level&lt;/b&gt; elements. It explains their usage in an &lt;b class="keywords"&gt;HTML&lt;/b&gt; document.&lt;/p&gt;</code>
</pre>

Elemen <code>bdi</code> digunakan untuk mengisolasi kata dari bahasa yang arah tulisannya berbeda dari kata-kata lain di sekitarnya. BDI adalah singkatan dari Bi-directional Isolation.

<pre>
<code data-language="html">&lt;ul&gt;
  &lt;li&gt;User &lt;bdi&gt;hrefs&lt;/bdi&gt;: 60 points&lt;/li&gt;
  &lt;li&gt;User &lt;bdi&gt;jdoe&lt;/bdi&gt;: 80 points&lt;/li&gt;
  &lt;li&gt;User &lt;bdi&gt;إيان&lt;/bdi&gt;: 90 points&lt;/li&gt;
&lt;/ul&gt;</code>
</pre>

Hasil output:

<ul>
 <li>User <bdi>hrefs</bdi>: 60 points</li>
 <li>User <bdi>jdoe</bdi>: 80 points</li>
 <li>User <bdi>إيان</bdi>: 90 points</li>
</ul>

Bagaimana jika tanpa elemen <code>bdi</code>?

<pre>
<code data-language="html">&lt;ul&gt;
  &lt;li&gt;User hrefs: 60 points&lt;/li&gt;
  &lt;li&gt;User jdoe: 80 points&lt;/li&gt;
  &lt;li&gt;User إيان: 90 points&lt;/li&gt;
&lt;/ul&gt;</code>
</pre>

Hasil output:

<ul>
 <li>User hrefs: 60 points</li>
 <li>User jdoe: 80 points</li>
 <li>User إيان: 90 points</li>
</ul>

Elemen <code>bdo</code> digunakan untuk mengganti arah teks.

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
      <td><code>dir</code></td>
      <td>
        <code>ltr</code><br>
        <code>rtl</code>
      </td>
      <td><code>ltr</code>: teks ditampilkan dari kiri ke kanan<br>
      <code>rtl</code>: teks ditampilkan dari kanan ke kiri
      </td>
    </tr>
  </tbody>
</table>

<pre>
<code data-language="html">&lt;p&gt;&lt;bdo dir="rtl"&gt;This text will go right to left.&lt;/bdo&gt;&lt;/p&gt;</code>
</pre>

Elemen <code>br</code> digunakan untuk membuat baris baru.

<pre>
<code data-language="html">Mozilla Foundation&lt;br&gt;
1981 Landings Drive&lt;br&gt;
Building K&lt;br&gt;
Mountain View, CA 94043-0801&lt;br&gt;
USA</code>
</pre>

Elemen <code>data</code> digunakan untuk membuat daftar data yang disertai id untuk keperluan pemrosesan data menggunakan javascript.

<pre>
<code data-language="html">&lt;ul&gt;HTML5 Books
&lt;li&gt;&lt;data value="1118012526"&gt;HTML5 For Dummies&lt;/data&gt;&lt;/li&gt;
&lt;li&gt;&lt;data value="1615640843"&gt;HTML5 For Complete Idiots&lt;/data>&lt;/li&gt;
&lt;li&gt;&lt;data value="8390492029"&gt;HTML5 For Stark Raving Mad Lunatics Who Couldn't Tie A Shoelace If They Tried&lt;/data>&lt;/li&gt;
&lt;/ul&gt;</code>
</pre>

Elemen <code>em</code> digunakan untuk menandai kata yang perlu ditekankan.

<pre>
<code data-language="html">&lt;p&gt;In HTML 5, what was previously called &lt;em&gt;block-level&lt;/em&gt; content is now called &lt;em&gt;flow&lt;/em&gt; content.&lt;/p&gt;</code>
</pre>

Elemen <code>i</code> membuat teks cetak miring yang digunakan untuk menandai kata-kata asing.

<pre>
<code data-language="html">&lt;p&gt;The Latin phrase &lt;i class="latin"&gt;Veni, vidi, vici&lt;/i&gt; is often mentioned in music, art, and literature.&lt;/p&gt;</code>
</pre>

Elemen <code>kbd</code> digunakan untuk menulis perintah masukkan dari keyboard.

<pre>
<code data-language="html">&lt;p&gt;Three keys you really need to familiarize yourself with are &lt;kbd&gt;CTRL&lt;/kbd&gt;, &lt;kbd&gt;ALT&lt;/kbd&gt; and &lt;kbd&gt;DEL&lt;/kbd&gt;.&lt;/p&gt;</code>
</pre>

Elemen <code>mark</code> digunakan untuk merepresentasikan teks yang disorot atau ditandai karena memiliki peran penting, biasanya dimaksudkan untuk mereferensi (merujuk) atau mengingatkan akan hal penting yang berkaitan dengan konteks khusus sebuah kalimat.

<pre>
<code data-language="html">&lt;p&gt;Despite the stockmarket crash in 2008, the value of my share portfolio &lt;mark&gt;increased by 100 percent&lt;/mark&gt;. I must be doing something right.&lt;/p&gt;
&lt;p&gt;I should point out that the value only increased because I kept pumping more money in!&lt;/p&gt;</code>
</pre>

Elemen <code>q</code> digunakan untuk menandai kutipan singkat dalam sebuah kalimat. Elemen <code>q</code> menggunakan atribut <code>cite</code> digunakan untuk mengetahui sumber kutipan diambil.

<pre>
<code data-language="html">&lt;p&gt;According to Mozilla's website, &lt;q cite="https://www.mozilla.org/en-US/about/history/details/"&gt;Firefox 1.0 was released in 2004 and became a big success.&lt;/q&gt;&lt;/p&gt;</code>
</pre>

Elemen <code>s</code> digunakan untuk menunjukkan konten atau teks yang sudah tidak lagi akurat atau relevan.

<pre>
<code data-language="html">&lt;s&gt;Today's Special: Salmon&lt;/s&gt; SOLD OUT&lt;br&gt;
&lt;!-- Using CSS --&gt;
&lt;span style="text-decoration:line-through;"&gt;Today's Special: Salmon&lt;/span&gt; SOLD OUT</code>
</pre>

Elemen <code>small</code> digunakan untuk konten yang kurang penting.

<pre>
<code data-language="html">&lt;p&gt;Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis.&lt;/p&gt;
&lt;small&gt;Posted on &lt;time datetime="2017-04-29T19:00"&gt;Apr 29&lt;/time&gt; in &lt;a href="/category/code"&gt;Code&lt;/a&gt;&lt;/small&gt;</code>
</pre>

Elemen <code>strong</code> digunakan untuk menunjukkan yang penting untuk diperhatikan.

<pre>
<code data-language="html">&lt;p&gt;Chapter 1: &lt;strong&gt;Proper Use of the Strong Element&lt;/strong&gt;&lt;/p&gt;</code>
</pre>