---
layout: blankdemo
title: Escetic
permalink: /hljs/escetic/
---

<style>
@font-face {
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 700;
  font-display: swap;
  src: url(https://fonts.gstatic.com/s/roboto/v27/KFOlCnqEu92Fr1MmWUlfBBc4.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
body {font-family:Roboto, sans-serif}
pre {user-select:all}

.hljs{display:block;overflow-x:auto;padding:0.5em;background:white;color:black}
.hljs-string,.hljs-variable,.hljs-template-variable,.hljs-symbol,.hljs-bullet,.hljs-section,.hljs-addition,.hljs-attribute,.hljs-link{color:#888}
.hljs-comment,.hljs-quote,.hljs-meta,.hljs-deletion{color:#ccc}
.hljs-keyword,.hljs-selector-tag,.hljs-section,.hljs-name,.hljs-type,.hljs-strong{font-weight:bold}
.hljs-emphasis{font-style:italic}
</style>

<h2>Sample dan CSS yang digunakan</h2>

<h3>CSS (Copy CSS ini ke Template)</h3>

<pre><code class="hljs"><span class="hljs-selector-class">.hljs</span>{<span class="hljs-attribute">display</span>:block;<span class="hljs-attribute">overflow-x</span>:auto;<span class="hljs-attribute">padding</span>:<span class="hljs-number">0.5em</span>;<span class="hljs-attribute">background</span>:white;<span class="hljs-attribute">color</span>:black}
<span class="hljs-selector-class">.hljs-string</span>,<span class="hljs-selector-class">.hljs-variable</span>,<span class="hljs-selector-class">.hljs-template-variable</span>,<span class="hljs-selector-class">.hljs-symbol</span>,<span class="hljs-selector-class">.hljs-bullet</span>,<span class="hljs-selector-class">.hljs-section</span>,<span class="hljs-selector-class">.hljs-addition</span>,<span class="hljs-selector-class">.hljs-attribute</span>,<span class="hljs-selector-class">.hljs-link</span>{<span class="hljs-attribute">color</span>:<span class="hljs-number">#888</span>}
<span class="hljs-selector-class">.hljs-comment</span>,<span class="hljs-selector-class">.hljs-quote</span>,<span class="hljs-selector-class">.hljs-meta</span>,<span class="hljs-selector-class">.hljs-deletion</span>{<span class="hljs-attribute">color</span>:<span class="hljs-number">#ccc</span>}
<span class="hljs-selector-class">.hljs-keyword</span>,<span class="hljs-selector-class">.hljs-selector-tag</span>,<span class="hljs-selector-class">.hljs-section</span>,<span class="hljs-selector-class">.hljs-name</span>,<span class="hljs-selector-class">.hljs-type</span>,<span class="hljs-selector-class">.hljs-strong</span>{<span class="hljs-attribute">font-weight</span>:bold}
<span class="hljs-selector-class">.hljs-emphasis</span>{<span class="hljs-attribute">font-style</span>:italic}</code></pre>

<h3>Contoh HTML, XML</h3>

<pre><code class="hljs"><span class="hljs-meta">&lt;!DOCTYPE html&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">title</span>&gt;</span>Title<span class="hljs-tag">&lt;/<span class="hljs-name">title</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">style</span>&gt;</span><span class="css"><span class="hljs-selector-tag">body</span> {<span class="hljs-attribute">width</span>: <span class="hljs-number">500px</span>;}</span><span class="hljs-tag">&lt;/<span class="hljs-name">style</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"application/javascript"</span>&gt;</span><span class="javascript">
  <span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">$init</span>(<span class="hljs-params"></span>) </span>{<span class="hljs-keyword">return</span> <span class="hljs-literal">true</span>;}
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">body</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">checked</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"title"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">'title'</span>&gt;</span>Title<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-comment">&lt;!-- here goes the rest of the page --&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">body</span>&gt;</span></code></pre>

<h3>Contoh JavaScript</h3>

<pre><code class="hljs"><span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">$initHighlight</span>(<span class="hljs-params">block, cls</span>) </span>{
  <span class="hljs-keyword">try</span> {
    <span class="hljs-keyword">if</span> (cls.search(<span class="hljs-regexp">/\bno\-highlight\b/</span>) != <span class="hljs-number">-1</span>)
      <span class="hljs-keyword">return</span> process(block, <span class="hljs-literal">true</span>, <span class="hljs-number">0x0F</span>) +
             <span class="hljs-string">` class="<span class="hljs-subst">${cls}</span>"`</span>;
  } <span class="hljs-keyword">catch</span> (e) {
    <span class="hljs-comment">/* handle exception */</span>
  }
  <span class="hljs-keyword">for</span> (<span class="hljs-keyword">var</span> i = <span class="hljs-number">0</span> / <span class="hljs-number">2</span>; i &lt; classes.length; i++) {
    <span class="hljs-keyword">if</span> (checkCondition(classes[i]) === <span class="hljs-literal">undefined</span>)
      <span class="hljs-built_in">console</span>.log(<span class="hljs-string">'undefined'</span>);
  }

  <span class="hljs-keyword">return</span> (
    <span class="xml"><span class="hljs-tag">&lt;<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">web-component</span>&gt;</span>{block}<span class="hljs-tag">&lt;/<span class="hljs-name">web-component</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  )
}

export  $initHighlight;</span></code></pre>
