<svelte:head>
	<title>Technical documentation</title>
</svelte:head>

<h1 id="corona-info">Technical documentation</h1>
<h2 id="simple-integration">Simple Integration</h2>
<p>It&#39;s as easy as adding </p>
<pre><code class="lang-html"><span class="hljs-tag">&lt;<span class="hljs-name">script</span> <span class="hljs-attr">async</span> <span class="hljs-attr">src</span>=<span class="hljs-string">'https://webinfowidget-webcomponent.netlify.com/build/embed.js'</span>&gt;</span><span class="undefined"></span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
<p>to your website. This will load our widget and place it on your website.</p>
<p>We&#39;ll take care of updating the information with new, important and verified Data. 100% Fake-News free.</p>
<h3 id="fast-secure-and-accessible">Fast, secure and accessible</h3>
<ul>
	<li>Fast: We made sure that our script is as small as possible - it&#39;s only 7.2kb</li>
	<li>Secure: No data is collected - we value your privacy</li>
	<li>Accessible: We&#39;ve optimized the widget for screenreaders and keyboard users</li>
</ul>
<h3 id="customizable">Customizable</h3>
<p>Position it where you want like so:</p>
<pre><code class="lang-css">{`web-info-widget {
\tleft: 5rem;
\ttop: 5rem;
\tright: auto;
\tbottom: auto;
}`}</code></pre>
