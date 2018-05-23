---
layout: post
title: Pengenalan WAI ARIA
date: 2018-05-06 16:53:20 +0700
description: Mengenal apa itu WAI ARIA
img: aria.jpg
tags: [ARIA, HTML5, Javascript]
---
WAI-ARIA ( Web Accessibility Initiative - Accessible Rich Internet Applications ) adalah suatu cara agar konten web dan aplikasi web lebih dapat diakses oleh assistive technology (teknologi pendamping) seperti perangkat-perangkat yang digunakan orang cacat untuk mengakses web. Saat ini HTML masih belum ramah untuk assistive technology karena terbatasnya kemampuan HTML. Untuk membuat web benar-benar interaktif dengan pengguna, kita pasti harus banyak menggunakan javascript. Empat masalah yang menghalangi assistive technology untuk bekerja dengan aplikasi javascript:
1. Fungsi komponen yang tidak jelas
2. State dan properti komponen tidak jelas
3. Perubahan konten tidak terdeteksi
4. Aksesibilitas keyboard yang buruk

Cara menggunakan ARIA pada HTML dengan menambahkan atribut tambahan ke tag HTML. Tambahan atribut tersebut membuat perangkat assistive technology dapat mengenali properti, relationship dan state dari user interface.

Bagaimana ARIA dapat membuat HTML lebih ramah untuk perangkat AT?
###### 1. Fungsi komponen yang jelas dengan atribut role
ARIA menyediakan banyak jenis role untuk digunakan.

Pada Bootstrap menggunakan daftar tidak terurut (unordered list) untuk membuat tab navigasi. Agar komponen unordered list berperan sebagai tab navigasi, digunakan atribut <code>role="tablist"</code>, <code>role="tab"</code> dan <code>role="tabpanel"</code>.
<pre>
<code data-language="html">&lt;ul class="nav nav-tabs" id="myTab" role="tablist"&gt;
 &lt;li class="nav-item"&gt;
  &lt;a class="nav-link active" id="home-tab" data-toggle="tab" href="#home" role="tab" aria-controls="home" aria-selected="true"&gt;Home&lt;/a&gt;
 &lt;/li&gt;
 &lt;li class="nav-item"&gt;
  &lt;a class="nav-link" id="profile-tab" data-toggle="tab" href="#profile" role="tab" aria-controls="profile" aria-selected="false"&gt;Profile&lt;/a&gt;
 &lt;/li&gt;
 &lt;li class="nav-item"&gt;
  &lt;a class="nav-link" id="contact-tab" data-toggle="tab" href="#contact" role="tab" aria-controls="contact" aria-selected="false"&gt;Contact&lt;/a&gt;
 &lt;/li&gt;
&lt;/ul&gt;
&lt;div class="tab-content" id="myTabContent"&gt;
 &lt;div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab"&gt;
  &lt;p&gt;Welcome!&lt;/p&gt;
 &lt;/div&gt;
 &lt;div class="tab-pane fade" id="profile" role="tabpanel" aria-labelledby="profile-tab"&gt;
  &lt;p&gt;My Profile&lt;/p&gt;
 &lt;/div&gt;
 &lt;div class="tab-pane fade" id="contact" role="tabpanel" aria-labelledby="contact-tab"&gt;
  &lt;p&gt;Contact me&lt;/p&gt;
 &lt;/div&gt;
&lt;/div&gt;</code>
</pre>

###### 2. State dan properti komponen
Untuk membuat koneksi antara <code>role="tab"</code> dengan <code>role="tabpanel"</code> digunakan properti <code>aria-controls</code> dan <code>aria-labelledby</code>. Properti <code>aria-controls</code> digunakan untuk mengetahui elemen yang dikontrol dan properti <code>aria-labelledby</code> untuk mengetahui elemen yang bertindak sebagai label untuk elemen tersebut. Perlu diperhatikan bahwa nilai properti <code>aria-labelledby</code> dan <code>aria-labelledby</code> adalah nilai atribut <code>id</code> elemen tujuan.

Untuk mengetahui tab mana yang aktif atau tidak aktif (state komponen), digunakan properti <code>aria-selected</code>. Jika tab aktif maka properti <code>aria-selected</code> bernilai <code>true</code>. Jika tab tidak aktif maka properti <code>aria-selected</code> bernilai <code>false</code>.

<pre>
<code data-language="html">&lt;ul class="nav nav-tabs" id="myTab" role="tablist"&gt;
 &lt;li class="nav-item"&gt;
  &lt;a class="nav-link active" id="home-tab" data-toggle="tab" href="#home" role="tab" aria-controls="home" aria-selected="true"&gt;Home&lt;/a&gt;
 &lt;/li&gt;
 &lt;li class="nav-item"&gt;
  &lt;a class="nav-link" id="profile-tab" data-toggle="tab" href="#profile" role="tab" aria-controls="profile" aria-selected="false"&gt;Profile&lt;/a&gt;
 &lt;/li&gt;
 &lt;li class="nav-item"&gt;
  &lt;a class="nav-link" id="contact-tab" data-toggle="tab" href="#contact" role="tab" aria-controls="contact" aria-selected="false"&gt;Contact&lt;/a&gt;
 &lt;/li&gt;
&lt;/ul&gt;
&lt;div class="tab-content" id="myTabContent"&gt;
 &lt;div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab"&gt;
  &lt;p&gt;Welcome!&lt;/p&gt;
 &lt;/div&gt;
 &lt;div class="tab-pane fade" id="profile" role="tabpanel" aria-labelledby="profile-tab"&gt;
  &lt;p&gt;My Profile&lt;/p&gt;
 &lt;/div&gt;
 &lt;div class="tab-pane fade" id="contact" role="tabpanel" aria-labelledby="contact-tab"&gt;
  &lt;p&gt;Contact me&lt;/p&gt;
 &lt;/div&gt;
&lt;/div&gt;</code>
</pre>

###### 3. Mendeteksi perubahan konten
Dengan menggunakan properti <code>aria-live</code>, <code>aria-atomic</code> dan <code>aria-relevant</code>, perangkat AT dapat mendeteksi perubahan pada konten yang terjadi.

Terdapat 3 nilai untuk properti <code>aria-live</code>:
1. <code>aria-live="off"</code> merupakan nilai default jika properti <code>aria-live</code> tidak dibuat. Perubahan yang terjadi pada konten tidak akan diberitahu
2. <code>aria-live="polite"</code>, perubahan konten akan diberitahu setelah pengguna tidak melakukan aktivitas terhadap konten lagi.
3. <code>aria-live="assertive"</code>, perubahan konten langsung diberitahu.

Nilai properti <code>aria-atomic</code>:
1. <code>aria-atomic="true"</code>, jika pada elemen &lt;p&gt; terdapat properti tersebut maka jika pada paragraf terjadi perubahan satu atau lebih kata, perangkat AT akan memberitahu lagi mulai dari awal paragraf
2. <code>aria-atomic="false"</code>, jika pada elemen &lt;p&gt; terdapat properti tersebut maka jika pada paragraf terjadi perubahan satu atau lebih kata, perangkat AT tidak akan memberitahu dari awal paragraf tapi hanya kata yang berubah saja

Nilai properti <code>aria-relevant</code>:
1. <code>aria-relevant="additions"</code>, perangkat AT akan memberitahu pengguna jika terjadi penambahan elemen pada daerah elemen yang memiliki properti tersebut
2. <code>aria-relevant="removals"</code>, perangkat AT akan memberitahu pengguna jika terjadi penghapusan elemen pada daerah elemen yang memiliki properti tersebut
3. <code>aria-relevant="text"</code>, perangkat AT akan memberitahu pengguna jika terjadi perubahan teks pada daerah elemen yang memiliki properti tersebut
4. <code>aria-relevant="all"</code>, perangkat AT akan memberitahu pengguna jika terjadi penambahan elemen, penghapusan elemen dan perubahan teks pada daerah elemen yang memiliki properti tersebut

Secara default properti <code>aria-relevant</code> bernilai <code>aria-relevant="text additions"</code>.

###### 4. Meningkatkan aksesibitas keyboard
Pada HTML4, elemen-elemen yang bisa mendapat fokus dari tombol tab keyboard hanya elemen untuk hyperlink dan untuk form.

Pada HTML5, tiap elemen bisa mendapat fokus dari tombol tab keyboard dengan mendeklarasikan atribut <code>tabindex</code>. Jika atribut <code>tabindex</code> bernilai lebih kecil dari 0 maka tidak akan mendapat fokus dari tab keyboard.

