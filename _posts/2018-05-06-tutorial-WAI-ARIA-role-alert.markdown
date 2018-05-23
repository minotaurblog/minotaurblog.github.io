---
layout: post
title: Tutorial ARIA - Alert
date: 2018-05-08 19:13:20 +0700
description: Mengenal widget alert beserta properti dan kegunaannya
img: alert.jpg
tags: [ARIA, HTML5, Javascript]
---
Alert adalah sebuah widget yng berfungsi untuk menyampaikan pesan singkat dan penting yang menarik perhatian pengguna tanpa mengganggu kerjaan pengguna.

Alert tidak memerlukan interaksi dengan keyboard.

<table class="table">
  <tbody>
    <tr>
      <td>Superclass role (role induk)</td>
      <td><code>section</code> (role abstrak)</td>
    </tr>
    <tr>
      <td>Subclass role (role turunan)</td>
      <td><code>alertdialog</code></td>
    </tr>
    <tr>
      <td>Properti</td>
      <td><code>aria-atomic</code><br>
          <code>aria-busy (state)</code><br>
          <code>aria-controls</code><br>
          <code>aria-current (state)</code><br>
          <code>aria-describedby</code><br>
          <code>aria-details</code><br>
          <code>aria-disabled (state)</code><br>
          <code>aria-dropeffect</code><br>
          <code>aria-errormessage</code><br>
          <code>aria-expanded (state)</code><br>
          <code>aria-flowto</code><br>
          <code>aria-grabbed (state)</code><br>
          <code>aria-haspopup</code><br>
          <code>aria-hidden (state)</code><br>
          <code>aria-invalid (state)</code><br>
          <code>aria-keyshortcuts</code><br>
          <code>aria-label</code><br>
          <code>aria-labelledby</code><br>
          <code>aria-live</code><br>
          <code>aria-owns</code><br>
          <code>aria-relevant</code><br>
          <code>aria-roledescription</code>
      </td>
    </tr>
    <tr>
      <td>State</td>
      <td><code>aria-busy</code><br>
          <code>aria-current</code><br>
          <code>aria-disabled</code><br>
          <code>aria-expanded</code><br>
          <code>aria-grabbed</code><br>
          <code>aria-hidden</code><br>
          <code>aria-invalid</code>
      </td>
    </tr>
    <tr>
      <td>State atau Properti bawaan</td>
      <td><code>aria-live="assertive"</code><br>
          <code>aria-atomic="true"</code>
      </td>
    </tr>
  </tbody>
</table>

kode HTML
<pre>
<code data-language="html">&lt;div&gt;
 &lt;button id="alert-trigger"&gt;Trigger Alert&lt;/button&gt;

 &lt;div id="example" role="alert"&gt;&lt;/div&gt;

 <!--  The following script element contains the content that will be inserted into the alert element. -->
 &lt;script type="text/template" id="alert-template"&gt;
   &lt;p>&lt;span lang="da">Hej&lt;/span&gt;, hello, &lt;span lang="it"&gt;ciao&lt;/span&gt;, &lt;span lang="ja"&gt;?????&lt;/span&gt;, &lt;span lang="ko"&gt;??&lt;/span&gt;&lt;/p&gt;
 &lt;/script&gt;
&lt;/div&gt;</code>
</pre>

Kode CSS
<pre>
<code data-language="css">[role="alert"] {
 padding: 10px;
 border: 2px solid hsl(206, 74%, 54%);
 border-radius: 4px;
 background: hsl(206, 74%, 90%);
}

[role="alert"]:empty {
 display: none;
}</code>
</pre>

Kode Javascript
<pre>
<code data-language="css">window.addEventListener('load', function () {

    var button = document.getElementById('alert-trigger');

    button.addEventListener('click', addAlert);

  });

  function addAlert (event) {
    var example = document.getElementById('example');
    var template = document.getElementById('alert-template').innerHTML;

    example.innerHTML = template;
  }</code>
</pre>

<p data-height="265" data-theme-id="0" data-slug-hash="odpWLR" data-default-tab="html,result" data-user="minotaurblog" data-embed-version="2" data-pen-title="ARIA - alert" class="codepen">See the Pen <a href="https://codepen.io/minotaurblog/pen/odpWLR/">ARIA - alert</a> by minotaurblog (<a href="https://codepen.io/minotaurblog">@minotaurblog</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>