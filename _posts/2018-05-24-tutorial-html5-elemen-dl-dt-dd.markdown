---
layout: post
title: Tutorial HTML5 - Elemen &lt;dl&gt;, &lt;dt&gt;, &lt;dd&gt
date: 2018-05-24 14:05:12 +0700
description: Mengenal Elemen dl, dt, dd Beserta Atribut dan Fungsinya
img: description.jpg
tags: [HTML5]
---
Elemen <code>dl</code>, <code>dt</code>, <code>dd</code> digunakan untuk list yang bersifat menjelaskan.

###### Satu istilah dan penjelasan
<pre>
<code data-language="html">&lt;dl&gt;
 &lt;dt&gt;Firefox&lt;/dt&gt;
 &lt;dd&gt;
   A free, open source, cross-platform, graphical web browser developed by the Mozilla Corporation and hundreds of volunteers.
 &lt;/dd&gt;

 &lt;!-- Other terms and descriptions --&gt;
&lt;/dl&gt;</code>
</pre>

Hasil output:

<dl>
  <dt>Firefox</dt>
  <dd>
    A free, open source, cross-platform, graphical web browser developed by the Mozilla Corporation and hundreds of volunteers.
  </dd>

  <!-- Other terms and descriptions -->
</dl>


###### Banyak istilah dan satu penjelasan
<pre>
<code data-language="html">&lt;dl&gt;
 &lt;dt&gt;Firefox&lt;/dt&gt;
 &lt;dt&gt;Mozilla Firefox&lt;/dt&gt;
 &lt;dt&gt;Fx&lt;/dt&gt;
 &lt;dd&gt;
   A free, open source, cross-platform, graphical web browser developed by the Mozilla Corporation and hundreds of volunteers.
 &lt;/dd&gt;

 &lt;!-- Other terms and descriptions --&gt;
&lt;/dl&gt;</code>
</pre>

Hasil output:

<dl>
  <dt>Firefox</dt>
  <dt>Mozilla Firefox</dt>
  <dt>Fx</dt>
  <dd>
    A free, open source, cross-platform, graphical web browser developed by the Mozilla Corporation and hundreds of volunteers.
  </dd>

  <!-- Other terms and descriptions -->
</dl>

###### Satu istilah dan banyak penjelasan
<pre>
<code data-language="html">&lt;dl&gt;
 &lt;dt&gt;Firefox&lt;/dt&gt;
 &lt;dd&gt;
   A free, open source, cross-platform, graphical web browser developed by the Mozilla Corporation and hundreds of volunteers.
 &lt;/dd&gt;
 &lt;dd&gt;
   The Red Panda also known as the Lesser Panda, Wah, Bear Cat or Firefox, is a mostly herbivorous mammal, slightly larger than a domestic cat (60 cm long).
 &lt;/dd&gt;

 &lt;!-- Other terms and descriptions --&gt;
&lt;/dl&gt;</code>
</pre>

Hasil output:

<dl>
  <dt>Firefox</dt>
  <dd>
    A free, open source, cross-platform, graphical web browser developed by the Mozilla Corporation and hundreds of volunteers.
  </dd>
  <dd>
    The Red Panda also known as the Lesser Panda, Wah, Bear Cat or Firefox, is a mostly herbivorous mammal, slightly larger than a domestic cat (60 cm long).
  </dd>

  <!-- Other terms and descriptions -->
</dl>
