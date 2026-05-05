---
title: "Why your API infrastructure isn’t ready for AI (and what to do about it)"
url: "https://tyk.io/blog/why-your-api-infrastructure-isnt-ready-for-ai-and-what-to-do-about-it/"
date: "Thu, 02 Apr 2026 13:38:27 +0000"
author: "Laura Heritage"
feed_url: "https://tyk.io/feed/"
---
<p>Most financial institutions have spent years building API infrastructure. Few have built it to support what comes next.</p>



<p>At LEAP 2026, Mark Boyd, founder of Platformable, laid out the problem clearly: the adoption gap in Open Banking and AI isn&#8217;t a technology problem. It&#8217;s a context problem.&nbsp;</p>



<p>Banks are deploying APIs without a structured understanding of:</p>



<ul class="wp-block-list">
<li>Who they serve</li>



<li>What markets they operate in, or </li>



<li>What their organizations are actually capable of delivering. </li>
</ul>



<p></p>



<p>When AI enters that environment, the cracks become craters.</p>



<p>Boyd&#8217;s solution is a context-first approach to digital infrastructure, one that gives humans a governing role over AI outcomes and enables intelligent agents to navigate uncertainty without breaking down.&nbsp;</p>



<p>The results, when done well, are significant.&nbsp;</p>



<ul class="wp-block-list">
<li>ABN AMRO used this approach to spin up a digital bank for teenagers in under a year. </li>



<li>Klarna built an agentic product protocol API that creates value across its entire client ecosystem.<br /></li>
</ul>



<p></p>



<p><a href="https://www.youtube.com/watch?v=8Wn1crJ3e1A">Watch Boyd&#8217;s full session here</a>, or read on for the key takeaways.</p>



<h2 class="wp-block-heading" id="h-the-problem-ai-needs-more-than-apis">The problem: AI needs more than APIs</h2>



<p>Smart finance today spans Open Banking, Open Finance, stablecoins, embedded finance, and agentic commerce. All of it runs on API infrastructure. But for agentic AI to function on that foundation, it needs to understand intent, not just execute instructions.</p>



<p>Without that understanding, organizations run into two compounding problems.&nbsp;</p>



<ul class="wp-block-list">
<li>API drift, where what gets built no longer matches what was intended. </li>



<li>API sprawl, where APIs multiply faster than anyone can track or govern them.</li>
</ul>



<p></p>



<p>Context engineering is Boyd&#8217;s answer. It&#8217;s the practice of describing intent in enough depth that AI systems can act on it reliably, even when things go wrong. That means documenting use cases, operational environments, and organizational capabilities in a structured way that both humans and agents can navigate.</p>



<h2 class="wp-block-heading" id="h-five-types-of-context-that-matter">Five types of context that matter</h2>



<p>Boyd breaks context into five layers, each one essential to building infrastructure that actually delivers value.</p>



<p><strong>User context</strong> is about deeply understanding who you&#8217;re building for.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7612" height="572" src="https://tyk.io/wp-content/uploads/2026/04/closing-the-adoption-gap-1024x572.png" width="1024" /></figure>



<p>Boyd uses Gen Z as an example: ages 13 to 28, entering banking for the first time, with strong fintech preferences, a rent-not-own mindset, and expectations around instant payments and round-up savings. ABN AMRO&#8217;s teenage digital bank succeeded because the institution had already done this work at the infrastructure level.&nbsp;</p>



<p>Corporate banking has its own user context: enterprises increasingly want direct integration between their bank accounts and ERP systems, enabling real-time cash flow visibility, optimized payments, and cross-border transaction management.</p>



<p><strong>Global context</strong> covers the macro forces shaping where and how banks can operate.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7613" height="572" src="https://tyk.io/wp-content/uploads/2026/04/blog-building-content-first-LEAP-2-1024x572.png" width="1024" /></figure>



<p>Data sovereignty regulations in France and Germany now require consumer and business finance data to be stored on in-country servers. AI regulation is converging with Open Banking compliance across markets from the UK to Australia to Singapore.&nbsp;</p>



<p>Meanwhile, the way customers find and engage with financial services is shifting, as search traffic drops and online communities fragment across WhatsApp, Discord, and Signal. Ecosystem-led growth and partnership strategies are becoming a primary customer acquisition model.</p>



<p><strong>Local and regional context</strong> means staying current on the regulatory milestones specific to each market you operate in.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7614" height="572" src="https://tyk.io/wp-content/uploads/2026/04/blog-building-content-first-LEAP-3-1024x572.png" width="1024" /></figure>



<p>Sixty-eight countries now have Open Banking regulations in place, with 21 more moving in that direction. Cross-border players are managing a constantly shifting set of local requirements alongside AI regulation, instant payment rules, and regional standards like the <a href="https://www.berlin-group.org/">Berlin Group</a> framework and <a href="https://financialdataexchange.org/">Financial Data Exchange (FDX)</a>. Interoperability is not optional in this environment, and API aggregators are filling standards gaps in the meantime.</p>



<p><strong>Organizational context</strong> is where many adoption efforts quietly fail.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7615" height="351" src="https://tyk.io/wp-content/uploads/2026/04/blog-building-content-first-LEAP-4-1024x351.png" width="1024" /></figure>



<p>A top-down mandate for API governance doesn&#8217;t work in a federated organization where business lines operate independently. Boyd recommends mapping accountability gaps using RACI frameworks to surface where API and AI workflows fall through the cracks. He also suggests framing adoption conversations around what each department actually cares about: revenue, cost savings, equity, or operational efficiency. The <a href="https://bian.org/">Banking Industry Architecture Network (BIAN)&#8217;</a>s capabilities model is a useful tool for mapping business capabilities to value streams, making it easier to track intent across the organization.</p>



<p><strong>Digital and infrastructure context</strong> ties it all together.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7616" height="572" src="https://tyk.io/wp-content/uploads/2026/04/blog-building-content-first-LEAP-5-1024x572.png" width="1024" /></figure>



<p>Boyd recommends using Arazzo workflows to document how APIs combine to serve specific use cases, and notes these are also useful for MCP descriptions and AI-readable documentation like Agents.MD and llm.txt. ABN AMRO&#8217;s 2028 corporate roadmap offers a concrete example of this vision: decommissioning legacy applications, increasing API coverage, and moving toward modular, composable instances that spin up for a task and retire when done.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7617" height="572" src="https://tyk.io/wp-content/uploads/2026/04/blog-building-content-first-LEAP-6-1024x572.png" width="1024" /></figure>



<p>Klarna offers the clearest commercial example of this in action. It used AI to build an agentic product protocol API, a deliberately low-risk, high-value starting point. Rather than pointing AI at customers first, Klarna built product catalogs that allow its clients to surface relevant products and services for their own customers. The result creates value at every layer of the ecosystem: Klarna&#8217;s business model strengthens, clients get a better toolset, and end users get a more relevant experience. Klarna reinforced this with ecosystem-specific documentation and tailored customer journeys for each partner, effectively turning its API into an interoperability toolkit. It&#8217;s a useful model for any institution thinking about where to start with agentic AI.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-7618" height="572" src="https://tyk.io/wp-content/uploads/2026/04/blog-building-content-first-LEAP-7-1024x572.png" width="1024" /></figure>



<h2 class="wp-block-heading" id="h-finops-where-infrastructure-meets-business-value">FinOps: Where infrastructure meets business value</h2>



<p>Boyd&#8217;s framework doesn&#8217;t stop at architecture. It connects directly to cost management through FinOps modelling, using the FinOps Foundation&#8217;s AI frameworks as a starting point.</p>



<p>There are three components.&nbsp;</p>



<ul class="wp-block-list">
<li>Infrastructure capital expenditure, which is often ring-fenced separately for AI workloads right now. </li>



<li>Operational cost, where API metrics become a direct input to quantifying business savings. </li>



<li>Value realization, where AI usage is mapped to revenue outcomes and business goals. </li>
</ul>



<p></p>



<p>Getting this right turns infrastructure decisions into business cases, which is what earns cross-functional buy-in.</p>



<h2 class="wp-block-heading" id="h-three-steps-to-get-started">Three steps to get started</h2>



<p>Boyd closes with practical guidance for organizations ready to move:</p>



<ol class="wp-block-list">
<li>Map your context first. Use an ecosystem model to build a complete picture before making infrastructure decisions.</li>



<li>Don&#8217;t skip business capabilities mapping and API governance. They might <a href="https://tyk.io/blog/is-the-best-api-governance-strategy-a-boring-one/">feel boring</a> but these are important foundations that will enable acceleration and scalability. </li>



<li>Start AI with low-risk, high-value use cases rather than customer-facing initiatives. FinOps is the right first target. Build a catalog of AI use cases from there, and use sandboxes and synthetic data wherever possible</li>
</ol>



<p></p>



<p>Want further tips? Then <a href="https://tyk.io/contact/">speak to Tyk</a> for tailored insights and advice.</p>



<h4 class="wp-block-heading" id="h-frequently-asked-questions">Frequently asked questions</h4>



<p><strong>What is context-first API infrastructure in Open Banking?</strong> Context-first API infrastructure is an approach where banks document the intent behind their APIs before building them. That means mapping user needs, regulatory environments, organizational capabilities, and technical workflows so that both humans and AI agents can act on them reliably. Without this foundation, banks end up with API drift (what gets built no longer matches what was intended) and API sprawl (more APIs than anyone can govern).</p>



<p><strong>What is context engineering and why does it matter for agentic AI?</strong> Context engineering is the practice of describing intent in enough depth that AI systems can execute tasks reliably, even when they encounter errors or unexpected inputs. As financial services move toward agentic AI, where systems act autonomously on behalf of users, AI needs to understand not just instructions but the business environment those instructions operate within. Context engineering provides that foundation.</p>



<p><strong>How should banks get started with agentic AI?</strong> Boyd recommends starting with low-risk, high-value internal use cases rather than customer-facing applications. FinOps is the most practical first target: using API metrics to quantify infrastructure costs and identify savings. From there, banks can build a catalog of AI use cases, test in sandboxes with synthetic data, and scale from a position of documented intent rather than reactive deployment.</p>



<p><strong>What is API drift and how do banks avoid it?</strong> API drift happens when the APIs an organization builds no longer match the original business intent behind them. It&#8217;s common in fast-moving environments where development outpaces governance. The solution is context-first API governance: documenting use cases, mapping business capabilities, and using frameworks like Arazzo workflows to track how APIs serve specific outcomes over time.</p>



<p><strong>What Open Banking standards should financial institutions be building with?</strong> It depends on the market. In the US, FDX is the primary standard. In Europe, the Berlin Group framework applies. Sixty-eight countries now have Open Banking regulations in place, with 21 more moving in that direction. For cross-border institutions, API aggregators are currently filling interoperability gaps while global standards continue to develop. Regardless of region, Boyd&#8217;s core recommendation is the same: build with interoperability as a requirement, not an afterthought.</p>
<p>The post <a href="https://tyk.io/blog/why-your-api-infrastructure-isnt-ready-for-ai-and-what-to-do-about-it/">Why your API infrastructure isn&#8217;t ready for AI (and what to do about it)</a> appeared first on <a href="https://tyk.io">Tyk API Management</a>.</p>
