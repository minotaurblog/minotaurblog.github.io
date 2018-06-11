---
layout: post
title: Tutorial HTML5 - Tipe Link
date: 2018-06-09 10:32:12 +0700
description: Mengenal Tipe-tipe Link
img: linktypes.jpg
tags: [HTML5]
---
Dalam HTML, tipe link menunjukkan hubungan antara dua dokumen. Elemen yang digunakan untuk me-link satu sama yang lain seperti <code>&lt;a&gt;</code>, <code>&lt;area&gt;</code>, dan <code>&lt;link&gt;</code>.

<table class="table">
  <thead>
    <tr>
      <th scope="col">Tipe Link</th>
      <th scope="col">Keterangan</th>
      <th scope="col">Boleh di gunakan untuk elemen</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>alternate</code></td>
      <td>
        <ul>
            <li>Untuk elemen <code>&lt;link&gt;</code> dimana atribut <code>rel</code> juga berisi nilai <code>stylesheet</code> dan disertai atribut <code>title</code> digunakan untuk menunjukkan stylesheet alternatif</li>
            <li>Jika atribut <code>type</code> bernilai <code>application/rss+xml</code> or <code>application/atom+xml</code> digunakan untuk RSS feed</li>
            <li>Jika atribut <code>media</code> bernilai, maka digunakan untuk menunjukkan media (perangkat) tujuan</li>
            <li>Jika atribut <code>hreflang</code> bernilai, maka digunakan untuk menunjukkan bahasa alternatif</li>
            <li>Jika atribut <code>type</code> bernilai, maka digunakan untuk menunjukkan format alternatif</li>
        </ul>
      </td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>author</code></td>
      <td>digunakan untuk menyediakan URL ke halaman yang menjelaskan siapa penulis/pengarang atau kontak penulis/pengarang</td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>bookmark</code></td>
      <td>menyediakan hyperlink ke halaman untuk di bookmark</td>
      <td><code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>external</code></td>
      <td>menyediakan hyperlink ke halaman bantuan</td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>license</code></td>
      <td>menyediakan hyperlink ke halaman yang berisi informasi lisensi web kita</td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>next</code></td>
      <td>menyediakan hyperlink ke halaman selanjutnya</td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>nofollow</code></td>
      <td>memberitahu mesin pencari agar tidak merayapi (crawling) tautan tersebut</td>
      <td><code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>noreferrer</code></td>
      <td>mencegah browser mengirim alamat halaman pada header HTTP ketika mengklik tautan tersebut</td>
      <td><code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>noopener</code></td>
      <td>membuat nilai <code>window.opener=null</code> ketika kita klik tautan yang memiliki atribut <code>target="_blank"</code></td>
      <td><code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>prev</code></td>
      <td>menyediakan hyperlink ke halaman sebelumnya</td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>search</code></td>
      <td>menyediakan hyperlink ke halaman pencaarian untuk website kita</td>
      <td><code>link</code>, <code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>icon</code></td>
      <td>menyediakan tautan ke file icon yang berfungsi sebagai logo website kita</td>
      <td><code>a</code> dan <code>area</code></td>
    </tr>
    <tr>
      <td><code>tag</code></td>
      <td>menyediakan tautan ke halaman yang berisi penjelasan dari label tag yang kita buat</td>
      <td><code>link</code></td>
    </tr>
    <tr>
      <td><code>canonical</code></td>
      <td>Jika Anda memiliki 1 halaman yang dapat diakses dengan beberapa URL, atau beberapa halaman dengan konten yang serupa (misalnya, halaman dengan versi seluler dan desktop), halamanmu harus menjelaskan kepada Google, URL mana yang valid (kanonis) untuk halaman tersebut.</td>
      <td><code>link</code></td>
    </tr>
    <tr>
      <td><code>manifest</code></td>
      <td>untuk membuat halaman web kita menjadi sebuah aplikasi web pada smartphone</td>
      <td><code>link</code></td>
    </tr>
  </tbody>
</table>