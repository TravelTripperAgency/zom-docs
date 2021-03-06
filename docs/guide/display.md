<h1 class="zc-title">Display property</h1>

<p class="zc-lead">Quickly and responsively toggle the display value of components and more with our display utilities. Includes support for some of the more common values, as well as some extras for controlling display when printing.</p>

<h2 id="how-it-works">How it works</h2>

<p>Change the value of the <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/display"><code class="highlighter-rouge">display</code> property</a> with our responsive display utility classes. We purposely support only a subset of all possible values for <code class="highlighter-rouge">display</code>. Classes can be combined for various effects as you need.</p>

<h2 id="notation">Notation</h2>

<p>Display utility classes that apply to all <a href="/docs/4.1/layout/overview/#responsive-breakpoints">breakpoints</a>, from <code class="highlighter-rouge">xs</code> to <code class="highlighter-rouge">xl</code>, have no breakpoint abbreviation in them. This is because those classes are applied from <code class="highlighter-rouge">min-width: 0;</code> and up, and thus are not bound by a media query. The remaining breakpoints, however, do include a breakpoint abbreviation.</p>

<p>As such, the classes are named using the format:</p>

<ul class="default">
<li><code class="highlighter-rouge">.d-{value}</code> for <code class="highlighter-rouge">xs</code></li>
<li><code class="highlighter-rouge">.d-{breakpoint}-{value}</code> for <code class="highlighter-rouge">sm</code>, <code class="highlighter-rouge">md</code>, <code class="highlighter-rouge">lg</code>, and <code class="highlighter-rouge">xl</code>.</li>
</ul>

<p>Where <em>value</em> is one of:</p>

<ul class="default">
<li><code class="highlighter-rouge">none</code></li>
<li><code class="highlighter-rouge">inline</code></li>
<li><code class="highlighter-rouge">inline-block</code></li>
<li><code class="highlighter-rouge">block</code></li>
<li><code class="highlighter-rouge">table</code></li>
<li><code class="highlighter-rouge">table-cell</code></li>
<li><code class="highlighter-rouge">table-row</code></li>
<li><code class="highlighter-rouge">flex</code></li>
<li><code class="highlighter-rouge">inline-flex</code></li>
</ul>

<p>The media queries effect screen widths with the given breakpoint <em>or larger</em>. For example, <code class="highlighter-rouge">.d-lg-none</code> sets <code class="highlighter-rouge">display: none;</code> on both <code class="highlighter-rouge">lg</code> and <code class="highlighter-rouge">xl</code> screens.</p>

<h2 id="examples">Examples</h2>

<div class="zc-example">
<div class="d-inline p-2 bg-primary text-white">d-inline</div>
<div class="d-inline p-2 bg-dark text-white">d-inline</div>
</div>
<figure class="zc-highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"d-inline p-2 bg-primary text-white"</span><span class="nt">&gt;</span>d-inline<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"d-inline p-2 bg-dark text-white"</span><span class="nt">&gt;</span>d-inline<span class="nt">&lt;/div&gt;</span></code></pre></figure>

<div class="zc-example">
<span class="d-block p-2 bg-primary text-white">d-block</span>
<span class="d-block p-2 bg-dark text-white">d-block</span>
</div>
<figure class="zc-highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"d-block p-2 bg-primary text-white"</span><span class="nt">&gt;</span>d-block<span class="nt">&lt;/span&gt;</span>
<span class="nt">&lt;span</span> <span class="na">class=</span><span class="s">"d-block p-2 bg-dark text-white"</span><span class="nt">&gt;</span>d-block<span class="nt">&lt;/span&gt;</span></code></pre></figure>

<h2 id="hiding-elements">Hiding elements</h2>

<p>For faster mobile-friendly development, use responsive display classes for showing and hiding elements by device. Avoid creating entirely different versions of the same site, instead hide element responsively for each screen size.</p>

<p>To hide elements simply use the <code class="highlighter-rouge">.d-none</code> class or one of the <code class="highlighter-rouge">.d-{sm,md,lg,xl}-none</code> classes for any responsive screen variation.</p>

<p>To show an element only on a given interval of screen sizes you can combine one <code class="highlighter-rouge">.d-*-none</code> class with a <code class="highlighter-rouge">.d-*-*</code> class, for example <code class="highlighter-rouge">.d-none .d-md-block .d-xl-none</code> will hide the element for all screen sizes except on medium and large devices.</p>

<table class="table">
<thead>
  <tr>
    <th>Screen Size</th>
    <th>Class</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Hidden on all</td>
    <td><code class="highlighter-rouge">.d-none</code></td>
  </tr>
  <tr>
    <td>Hidden only on xs</td>
    <td><code class="highlighter-rouge">.d-none .d-sm-block</code></td>
  </tr>
  <tr>
    <td>Hidden only on sm</td>
    <td><code class="highlighter-rouge">.d-sm-none .d-md-block</code></td>
  </tr>
  <tr>
    <td>Hidden only on md</td>
    <td><code class="highlighter-rouge">.d-md-none .d-lg-block</code></td>
  </tr>
  <tr>
    <td>Hidden only on lg</td>
    <td><code class="highlighter-rouge">.d-lg-none .d-xl-block</code></td>
  </tr>
  <tr>
    <td>Hidden only on xl</td>
    <td><code class="highlighter-rouge">.d-xl-none</code></td>
  </tr>
  <tr>
    <td>Visible on all</td>
    <td><code class="highlighter-rouge">.d-block</code></td>
  </tr>
  <tr>
    <td>Visible only on xs</td>
    <td><code class="highlighter-rouge">.d-block .d-sm-none</code></td>
  </tr>
  <tr>
    <td>Visible only on sm</td>
    <td><code class="highlighter-rouge">.d-none .d-sm-block .d-md-none</code></td>
  </tr>
  <tr>
    <td>Visible only on md</td>
    <td><code class="highlighter-rouge">.d-none .d-md-block .d-lg-none</code></td>
  </tr>
  <tr>
    <td>Visible only on lg</td>
    <td><code class="highlighter-rouge">.d-none .d-lg-block .d-xl-none</code></td>
  </tr>
  <tr>
    <td>Visible only on xl</td>
    <td><code class="highlighter-rouge">.d-none .d-xl-block</code></td>
  </tr>
</tbody>
</table>

<div class="zc-example">
<div class="d-lg-none">hide on screens wider than lg</div>
<div class="d-none d-lg-block">hide on screens smaller than lg</div>
</div>
<figure class="zc-highlight"><pre><code class="language-html" data-lang="html"><span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"d-lg-none"</span><span class="nt">&gt;</span>hide on screens wider than lg<span class="nt">&lt;/div&gt;</span>
<span class="nt">&lt;div</span> <span class="na">class=</span><span class="s">"d-none d-lg-block"</span><span class="nt">&gt;</span>hide on screens smaller than lg<span class="nt">&lt;/div&gt;</span></code></pre></figure>
