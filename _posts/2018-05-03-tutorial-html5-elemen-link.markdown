---
layout: post
title: Tutorial HTML5 - Elemen &lt;link&gt;
date: 2018-05-03 14:21:20 +0700
description: Mengenal Elemen link Beserta Atribut dan Fungsinya
img: link.jpg
tags: [HTML5]
---
Elemen <code>link</code> menentukan hubungan antara dokumen HTML dengan resource luar.

Atribut elemen <code>link</code>
##### Atribut <code>href</code>
Atribut <code>href</code> berisi alamat url resource luar.

Ada 2 tipe alamat url:
1. URL absolut - URL absolut menyebutkan protokol serta domain dan path ke file (http://yourwebsite.com/images/logo.png)
2. URL relatif - URL relatif tidak menyebutkan protokol (http:// atau https://) dan domain (www.example.com) hanya berisi path folder/direktori

<pre>
<code data-language="html">&lt;link rel="stylesheet" type="text/css" href="theme.css"&gt;</code>
</pre>

##### Atribut <code>hreflang</code>
Atribut <code>hreflang</code> menginformasikan bahasa yang dipakai oleh dokumen link tujuan.

<pre>
<code data-language="html">&lt;link rel="alternate" href="http://www.example.com/ca/fr/" hreflang="fr-ca"&gt;</code>
</pre>

##### Atribut <code>media</code>
Atribut <code>media</code> menentukan media atau device tujuan yang dipakai oleh resource.

<pre>
<code data-language="html">&lt;link rel="stylesheet" type="text/css" href="theme.css"&gt;
&lt;link rel="stylesheet" type="text/css" href="print.css" media="print"&gt;</code>
</pre>

Nilai yang mungkin untuk atribut <code>media</code>
<table class="table">
  <thead>
    <tr>
      <th scope="col">Nilai</th>
      <th scope="col">Deskripsi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>all</code></td>
      <td>Untuk semua media atau device</td>
    </tr>
    <tr>
      <td><code>print</code></td>
      <td>Digunakan untuk mode print preview atau page yang akan diprint</td>
    </tr>
    <tr>
      <td><code>screen</code></td>
      <td>Digunakan untuk layar komputer, tablet, smartphone dll</td>
    </tr>
    <tr>
      <td><code>speech</code></td>
      <td>Digunakan untuk screen readers</td>
    </tr>
    <tr>
      <td>aspect-ratio</td>
      <td>Menentukan rasio pada tampilan. Menggunakan prefix "max-" dan "min-". Contoh media="screen and (max-aspect-ratio:16/9)"</td>
    </tr>
    <tr>
      <td>color</td>
      <td>Menentukan banyak bit per warna pada tampilan. Menggunakan prefix "max-" dan "min-". Contoh media="screen and (min-color:3)"</td>
    </tr>
    <tr>
      <td>color-index</td>
      <td>Menentukan banyak warna yang dapat digunakan oleh tampilan. Menggunakan prefix "max-" dan "min-". Contoh media="screen and (min-color-index:256)"</td>
    </tr>
    <tr>
      <td>grid</td>
      <td>Menentukan jenis grafik yang dipakai tampilan. Nilai yang mungkin adalah "1" atau "0". Contoh media="handheld and (grid:1)"</td>
    </tr>
    <tr>
      <td>height</td>
      <td>Menentukan panjang tampilan. Menggunakan prefix "max-" dan "min-". Contoh media="screen and (max-height:700px)"</td>
    </tr>
    <tr>
      <td>width</td>
      <td>Menentukan lebar tampilan. Menggunakan prefix "max-" dan "min-". Contoh media="screen and (min-width:500px)"</td>
    </tr>
    <tr>
      <td>monochrome</td>
      <td>Menentukan bit per pixel pada monochrome frame buffer. Menggunakan prefix "max-" dan "min-". Contoh media="screen and (min-monochrome:2)"</td>
    </tr>
    <tr>
      <td>orientation</td>
      <td>Menentukan orientasi tampilan atau kertas. Nilai yang mungkin "portrait" atau "landscape". Contoh media="all and (orientation: landscape)"</td>
    </tr>
    <tr>
      <td>resolution</td>
      <td>Menentukan kepadatan pixel pada tampilan atau kertas. Menggunakan prefix "max-" dan "min-". Contoh media="print and (min-resolution:300dpi)"</td>
    </tr>
    <tr>
      <td>scan</td>
      <td>Menentukan metode scan pada tampilan TV. Nilai yang mungkin "progressive" atau "interlace". Contoh media="tv and (scan:interlace)"</td>
    </tr>
  </tbody>
</table>

##### Atribut <code>rel</code>
Atribut <code>rel</code> menentukan hubungan antara dokumen HTML dengan dokumen tujuan link atau resource.

Nilai yang mungkin untuk atribut <code>rel</code>
<table class="table">
  <thead>
    <tr>
      <th scope="col">Nilai</th>
      <th scope="col">Deskripsi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>alternate</code></td>
      <td>Menyediakan link ke dokumen alternatif</td>
    </tr>
    <tr>
      <td><code>author</code></td>
      <td>Menyediakan link ke halaman tentang pembuat dokumen</td>
    </tr>
    <tr>
      <td><code>dns-prefetch</code></td>
      <td>Meresolve DNS tujuan sebelum digunakan</td>
    </tr>
    <tr>
      <td><code>help</code></td>
      <td>Menyediakan link ke halaman bantuan</td>
    </tr>
    <tr>
      <td><code>icon</code></td>
      <td>Import icon untuk dokumen</td>
    </tr>
    <tr>
      <td><code>licence</code></td>
      <td>Menyediakan link ke halaman informasi tentang licence</td>
    </tr>
    <tr>
      <td><code>next</code></td>
      <td>Menyediakan link ke dokumen selanjutnya jika dokumen tersebut berseri</td>
    </tr>
    <tr>
      <td><code>prev</code></td>
      <td>Menyediakan link ke dokumen sebelumnya jika dokumen tersebut berseri</td>
    </tr>
    <tr>
      <td><code>search</code></td>
      <td>Menyediakan link ke halaman pencarian dokumen berkaitan</td>
    </tr>
    <tr>
      <td><code>stylesheet</code></td>
      <td>Import style sheet atau file css</td>
    </tr>
  </tbody>
</table>

##### Atribut <code>sizes</code>
Atribut <code>sizes</code> menentukan ukuran icon resource untuk <code>rel="icon"</code>.

<pre>
<code data-language="html">&lt;link rel="icon" href="demo_icon.gif" type="image/gif" sizes="16x16"&gt;</code>
</pre>
