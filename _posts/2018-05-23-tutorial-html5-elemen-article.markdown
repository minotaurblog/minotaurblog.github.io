---
layout: post
title: Tutorial HTML5 - Elemen &lt;article&gt;
date: 2018-05-23 18:44:20 +0700
description: Mengenal Elemen article Beserta Atribut dan Fungsinya
img: article.jpg
tags: [HTML5]
---
Elemen <code>article</code> digunakan untuk menunjukkan bagian tulisan/karangan/artikel. Tiap tulisan/karangan/artikel pasti memiliki sebuah heading. Contoh digunakan elemen <code>article</code> adalah pada post forum, artikel majalah atau koran, dan entri blog.

Di dalam elemen <code>article</code> dapat mengandung elemen <code>article</code> dimana isi anak elemen <code>article</code> harus berkaitan dengan induknya. Contohnya pada blog yang menerima komentar pembaca dimana tiap komentar menggunakan elemen <code>article</code> yang berada di dalam elemen <code>article</code> tulisan/konten blog.

<pre>
<code data-language="html">&lt;article class="film_review"&gt;
 &lt;header&gt;
   &lt;h2&gt;Jurassic Park&lt;/h2&gt;
 &lt;/header&gt;
 &lt;section class="main_review"&gt;
   &lt;p&gt;Dinos were great!&lt;/p&gt;
 &lt;/section&gt;
 &lt;section class="user_reviews"&gt;
   &lt;article class="user_review"&gt;
     &lt;p&gt;Way too scary for me.&lt;/p&gt;
     &lt;footer&gt;
       &lt;p&gt;
         Posted on
         &lt;time datetime="2015-05-16 19:00"&gt;May 16&lt;/time&gt;
         by Lisa.
       &lt;/p&gt;
     &lt;/footer&gt;
   &lt;/article&gt;
   &lt;article class="user_review"&gt;
     &lt;p>I agree, dinos are my favorite.&lt;/p&gt;
     &lt;footer&gt;
       &lt;p&gt;
         Posted on
         &lt;time datetime="2015-05-17 19:00"&gt;May 17&lt;/time&gt;
         by Tom.
       &lt;/p&gt;
     &lt;/footer&gt;
   &lt;/article&gt;
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