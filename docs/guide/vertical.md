<h1 class="bd-title" id="content">Vertical alignment</h1>

<p class="bd-lead">Easily change the vertical alignment of inline, inline-block, inline-table, and table cell elements.</p>

<p>Change the alignment of elements with the <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align"><code class="highlighter-rouge">vertical-alignment</code></a> utilities. Please note that vertical-align only affects inline, inline-block, inline-table, and table cell elements.</p>

<p>Choose from <code class="highlighter-rouge">.align-baseline</code>, <code class="highlighter-rouge">.align-top</code>, <code class="highlighter-rouge">.align-middle</code>, <code class="highlighter-rouge">.align-bottom</code>, <code class="highlighter-rouge">.align-text-bottom</code>, and <code class="highlighter-rouge">.align-text-top</code> as needed.</p>

<p>With inline elements:</p>

<div class="zc-example">
  <span class="align-baseline">baseline</span>
  <span class="align-top">top</span>
  <span class="align-middle">middle</span>
  <span class="align-bottom">bottom</span>
  <span class="align-text-top">text-top</span>
  <span class="align-text-bottom">text-bottom</span>
</div>

<figure class="zc-highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"align-baseline"</span><span class="nt">&gt;</span>baseline<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"align-top"</span><span class="nt">&gt;</span>top<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"align-middle"</span><span class="nt">&gt;</span>middle<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"align-bottom"</span><span class="nt">&gt;</span>bottom<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"align-text-top"</span><span class="nt">&gt;</span>text-top<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"align-text-bottom"</span><span class="nt">&gt;</span>text-bottom<span class="nt">&lt;/span&gt;</span></code></pre></figure>

<p>With table cells:</p>

<div class="zc-example">
<table style="height: 100px;">
<tbody>
  <tr>
    <td class="align-baseline">baseline</td>
    <td class="align-top">top</td>
    <td class="align-middle">middle</td>
    <td class="align-bottom">bottom</td>
    <td class="align-text-top">text-top</td>
    <td class="align-text-bottom">text-bottom</td>
  </tr>
</tbody>
</table>
</div>
<figure class="zc-highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;table</span> <span class="na">style=</span><span class="s">"height: 100px;"</span><span class="nt">&gt;</span>
<span class="nt">&lt;tbody&gt;</span>
  <span class="nt">&lt;tr&gt;</span>
    <span class="nt">&lt;td</span> <span class="na">class=</span><span class="s">"align-baseline"</span><span class="nt">&gt;</span>baseline<span class="nt">&lt;/td&gt;</span>
    <span class="nt">&lt;td</span> <span class="na">class=</span><span class="s">"align-top"</span><span class="nt">&gt;</span>top<span class="nt">&lt;/td&gt;</span>
    <span class="nt">&lt;td</span> <span class="na">class=</span><span class="s">"align-middle"</span><span class="nt">&gt;</span>middle<span class="nt">&lt;/td&gt;</span>
    <span class="nt">&lt;td</span> <span class="na">class=</span><span class="s">"align-bottom"</span><span class="nt">&gt;</span>bottom<span class="nt">&lt;/td&gt;</span>
    <span class="nt">&lt;td</span> <span class="na">class=</span><span class="s">"align-text-top"</span><span class="nt">&gt;</span>text-top<span class="nt">&lt;/td&gt;</span>
    <span class="nt">&lt;td</span> <span class="na">class=</span><span class="s">"align-text-bottom"</span><span class="nt">&gt;</span>text-bottom<span class="nt">&lt;/td&gt;</span>
  <span class="nt">&lt;/tr&gt;</span>
<span class="nt">&lt;/tbody&gt;</span>
<span class="nt">&lt;/table&gt;</span></code></pre></figure>
