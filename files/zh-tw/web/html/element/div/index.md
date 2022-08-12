---
title: <div>
slug: Web/HTML/Element/div
translation_of: Web/HTML/Element/div
---
<p>{{HTMLRef}}</p>

<p><strong>HTML <code>&lt;div&gt;</code> 元素</strong>（或是<em> HTML 文件區塊元素</em>）是本質上不特別代表任何東西的通用内容流容器。它可以成為樣式化用途（使用 <strong>class</strong> 或 <strong>id</strong> 屬性）、或是共享如 <strong>lang</strong> 同一個屬性的元素集合。它應該在沒有其他適合的語義元素（例如{{HTMLElement("article")}} 或 {{HTMLElement("nav")}} ）可用時才用。</p>

<table class="properties">
 <tbody>
  <tr>
   <th scope="row"><a href="/zh-TW/docs/Web/HTML/Content_categories">內容類型</a></th>
   <td><a href="/zh-TW/docs/Web/HTML/Content_categories#Flow_content">流內容</a>、捫及內容。</td>
  </tr>
  <tr>
   <th scope="row">允許內容</th>
   <td><a href="/zh-TW/docs/Web/HTML/Content_categories#Flow_content">流內容</a></td>
  </tr>
  <tr>
   <th scope="row">Tag 省略</th>
   <td>{{no_tag_omission}}</td>
  </tr>
  <tr>
   <th scope="row">允許父元素</th>
   <td>任何允許<a href="/zh-TW/docs/Web/HTML/Content_categories#Flow_content">內容流</a>的元素。</td>
  </tr>
  <tr>
   <th scope="row">DOM 介面</th>
   <td>{{domxref("HTMLDivElement")}}</td>
  </tr>
 </tbody>
</table>

<h2 id="Attributes">屬性</h2>

<p>這個元素包含<a href="/zh-TW/docs/Web/HTML/Global_attributes">全域屬性</a>。</p>

<p><strong>align</strong> 元素已過時，不要使用它。</p>

<h2 id="Examples">範例</h2>

<pre class="brush: html">&lt;div&gt;
  &lt;p&gt;這裡可以是任何內容，例如 &amp;lt;p&amp;gt;、&amp;lt;table&amp;gt;。你說了算！&lt;/p&gt;
&lt;/div&gt;
</pre>

<h3 id="Result">結果</h3>

<p>這裡可以是任何內容，例如 &lt;p&gt;、&lt;table&gt;。你說了算！</p>

<h2 id="Specifications">規範</h2>

{{Specifications}}

<h2 id="Browser_compatibility">瀏覽器相容性</h2>


<div>{{Compat("html.elements.div")}}</div>



<h2 id="See_also">詳閱</h2>

<ul>
 <li>語義化的切片元素：{{HTMLElement("section")}}, {{HTMLElement("article")}}, {{HTMLElement("nav")}}, {{HTMLElement("header")}}, {{HTMLElement("footer")}}</li>
 <li>針對段落式內容樣式化的 {{HTMLElement("span")}} 元素</li>
</ul>