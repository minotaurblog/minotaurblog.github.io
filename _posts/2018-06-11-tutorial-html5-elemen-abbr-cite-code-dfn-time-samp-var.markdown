---
layout: post
title: Tutorial HTML5 - Elemen &lt;abbr&gt;, &lt;cite&gt;, &lt;code&gt;, &lt;dfn&gt;, &lt;time&gt, &lt;samp&gt;, &lt;var&gt;
date: 2018-06-11 15:52:12 +0700
description: Mengenal Elemen &lt;abbr&gt;, &lt;cite&gt;, &lt;code&gt;, &lt;dfn&gt;, &lt;time&gt;, &lt;samp&gt;, &lt;var&gt; Beserta Atribut dan Fungsinya
img: abbr.jpg
tags: [HTML5]
---
Elemen <code>abbr</code> digunakan untuk menampilkan singkatan dari suatu kata. Elemen <code>abbr</code> menggunakan
atribut <code>title</code> yang berisi kepanjangan kata tersebut.

<pre>
<code data-language="html">&lt;p&gt;Organisasi &lt;abbr title="World Health Organization"&gt;WHO&lt;/abbr&gt; didirikan pada tahun 1948.&lt;/p&gt;</code>
</pre>

Elemen <code>cite</code> digunakan untuk mengutip suatu karya (judul artikel, buku, nama lukisan dll).

<pre>
<code data-language="html">&lt;p&gt;&lt;cite&gt;The Scream&lt;/cite&gt; by Edward Munch. Painted in 1893.&lt;/p&gt;</code>
</pre>

Elemen <code>code</code> digunakan untuk menandai kode program.

<pre>
<code data-language="html">&lt;p&gt;To create a new array, type the following: &lt;code&gt;var faq = new Array(3)&lt;/code&gt;&lt;/p&gt;</code>
</pre>

Elemen <code>dfn</code> digunakan untuk menandai defenisi dari suatu istilah.

<pre>
<code data-language="html">&lt;p&gt;&lt;dfn&gt;HTML&lt;/dfn&gt; is the standard markup language for creating web pages.&lt;/p&gt;</code>
</pre>

Elemen <code>time</code> digunakan untuk menandai waktu. Elemen <code>time</code> memiliki satu atribut <code>datetime</code> berisi format tanggal dan waktu yang dapat dibaca mesin.

<ul>Format tanggal dan waktu yang valid:
<li>format tahun yang valid: <code>2011</code></li>
<li>format bulan yang valid: <code>2011-08</code></li>
<li>format tanggal yang valid: <code>2011-08-23</code></li>
<li>format tanggal tanpa tahun yang valid: <code>11-16</code></li>
<li>format minggu yang valid: <code>2011-W47</code></li>
<li>format waktu yang valid: <code>13:16</code>, <code>14:54:19</code>, <code>14:54:37.789</code></li>
<li>format tanggal dan waktu lokal yang valid: <code>2011-11-18T14:54:39.929</code>, <code>2011-11-18 14:54:39.929</code></li>
<li>format tanggal dan waktu global yang valid: <code>2011-11-18T14:54:39.929Z</code>, <code>2011-11-18T14:54:39.929-0400</code>, <code>2011-11-18T14:54:39.929-04:00</code>, <code>2011-11-18 14:54:39.929Z</code>, <code>2011-11-18 14:54:39.929-0400</code>, <code>2011-11-18 14:54:39.929-04:00</code></li>
</ul>

<pre>
<code data-language="html">&lt;p&gt;We open at &lt;time&gt;10:00&lt;/time&gt; every morning.&lt;/p&gt;

&lt;p&gt;I have a date on &lt;time datetime="2008-02-14 20:00"&gt;Valentines day&lt;/time&gt;.&lt;/p&gt;</code>
</pre>

Elemen <code>samp</code> digunakan untuk menandai ouput dari kode program.

<pre>
<code data-language="html">&lt;p&gt;I entered &lt;code&gt;git push&lt;/code&gt; and the terminal printed out &lt;samp&gt;Everything up-to-date&lt;/samp&gt;&lt;/p&gt;</code>
</pre>

Elemen <code>var</code> digunakan untuk menandai nama variabel dalam matematika atau programming.

<pre>
<code data-language="html">&lt;p&gt;The variables &lt;var&gt;minSpeed&lt;/var&gt; and &lt;var&gt;maxSpeed&lt;/var&gt; control the minimum and maximum speed of the apparatus in revolutions per minute (RPM).&lt;/p&gt;</code>
</pre>
