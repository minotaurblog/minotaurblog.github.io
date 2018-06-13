---
layout: post
title: Tutorial HTML5 - Elemen &lt;ruby&gt;, &lt;rb&gt;, &lt;rp&gt;, &lt;rt&gt;, &lt;rtc&gt;
date: 2018-06-13 12:32:12 +0700
description: Mengenal Elemen &lt;ruby&gt;, &lt;rb&gt;, &lt;rp&gt;, &lt;rt&gt;, &lt;rtc&gt; Beserta Atribut dan Fungsinya
img: ruby.jpg
tags: [HTML5]
---
Elemen <code>ruby</code> digunakan untuk menulis aksara cina dan jepang beserta cara pengucapan dari karakter tulisan cina/jepang dan cara pengucapan tersebut melekat di atas karakter cina/jepang.

Elemen <code>rb</code> digunakan untuk menandai aksara cina dan jepang.

Elemen <code>rt</code> digunakan untuk menulis cara pengucapan dari karakter tulisan cina/jepang dan cara pengucapan tersebut melekat di atas karakter cina/jepang.

Elemen <code>rp</code> berisi parenthesis (tanda kurung) untuk browser yang tidak mendukung elemen <code>ruby</code>.

Elemen <code>rtc</code> digunakan sebagai tempat teks elemen <code>ruby</code>.

<pre>
<code data-language="html">&lt;ruby&gt;
  &lt;rb&gt;旧&lt;/rb&gt;
  &lt;rt&gt;jiù&lt;/rt&gt;
  &lt;rb&gt;金&lt;/rb&gt;
  &lt;rt&gt;jīn&lt;/rt&gt;
  &lt;rb&gt;山&lt;/rb&gt;
  &lt;rt&gt;shān&lt;/rt&gt;
  &lt;rtc&gt;San Francisco&lt;/rtc&gt;
&lt;/ruby&gt;</code>
</pre>

Hasil output:

<ruby>
  <rb>旧</rb>
  <rt>jiù</rt>
  <rb>金</rb>
  <rt>jīn</rt>
  <rb>山</rb>
  <rt>shān</rt>
  <rtc>San Francisco</rtc>
</ruby>

