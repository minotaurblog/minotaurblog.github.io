---
layout: post
title: Tutorial HTML5 - Elemen &lt;a&gt;
date: 2018-06-09 10:32:12 +0700
description: Mengenal Elemen &lt;a&gt; Beserta Atribut dan Fungsinya
img: a.jpg
tags: [HTML5]
---
Elemen <code>a</code> digunakan untuk membuat hyperlink ke halaman web lain, file, alamat email, atau alamat URL lainnya.

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
      <td><code>download</code></td>
      <td>&nbsp;</td>
      <td>Menginstruksikan browser mengunduh file yang tertera pada atribut <code>href</code>. Atribut <code>href</code> yang tertera harus memiliki protokol (http atau https), domain (www.contoh.com) dan port (www.contoh.com:80) yang sama dengan protokol, domain dan port URL halaman web dimana hyperlink tersebut berada.</td>
    </tr>
    <tr>
      <td><code>href</code></td>
      <td>URL</td>
      <td>berisi alamat URL tujuan</td>
    </tr>
    <tr>
      <td><code>hreflang</code></td>
      <td>kode bahasa</td>
      <td>berisi kode bahasa yang digunakan alamat URL tujuan</td>
    </tr>
    <tr>
      <td><code>target</code></td>
      <td><code>_blank</code>, <code>_self</code>, dan frame name</td>
      <td>
        <code>_blank</code>: membuka hyperlink di jendela atau tab baru.<br>
        <code>_self</code>: membuka hyperlink di jendela atau tab yang sama dengan hyperlink.<br>
        frame name: membuka hyperlink di frame dengan atribut name
      </td>
    </tr>
    <tr>
      <td><code>rel</code></td>
      <td><a href="http://localhost:4000/tutorial-html5-tipe-link/">Tipe Link</a></td>
      <td>menjelaskan hubungan dokumen sekarang dengan dokumen yang dituju tautan</td>
    </tr>
    <tr>
      <td><code>type</code></td>
      <td><a href="http://localhost:4000/tutorial-html5-mime-types/">media type</a></td>
      <td>menentukan media type untuk dokumen di tautan tujuan</td>
    </tr>
  </tbody>
</table>

###### Membuat tautan ke website luar

<pre>
<code data-language="html">&lt;a href="https://www.mozilla.com/"&gt;Link eksternal&lt;/a&gt;</code>
</pre>

###### Membuat tautan ke seksi lain pada dokumen yang sama

<pre>
<code data-language="html">&lt;a href="#attr-href"&gt;Link ke seksi tujuan&lt;/a&gt;</code>
</pre>

###### Membuat gambar yang bisa diklik

<pre>
<code data-language="html">&lt;a href="https://developer.mozilla.org/en-US/" target="_blank"&gt;&lt;img src="https://mdn.mozillademos.org/files/6851/mdn_logo.png" alt="MDN logo" /&gt;&lt;/a&gt;</code>
</pre>

###### Membuat tautan email

<pre>
<code data-language="html">&lt;a href="mailto:nowhere@mozilla.org"&gt;Send email to nowhere&lt;/a&gt;</code>
</pre>

###### Membuat tautan telepon

<pre>
<code data-language="html">&lt;a href="tel:+491570156"&gt;+49 157 0156&lt;/a&gt;</code>
</pre>