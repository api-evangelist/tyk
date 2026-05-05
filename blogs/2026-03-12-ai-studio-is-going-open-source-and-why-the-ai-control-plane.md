---
title: "AI Studio is going Open Source (and why the AI Control Plane must be extensible)"
url: "https://tyk.io/blog/ai-studio-is-going-open-source-and-why-the-ai-control-plane-must-be-extensible/"
date: "Thu, 12 Mar 2026 11:30:00 +0000"
author: "Martin Buhr"
feed_url: "https://tyk.io/feed/"
---
<p><span style="font-weight: 400;">Over the last year, something subtle but important has happened in the AI industry. The conversation has shifted from “Which model should we use?” to “How do we control what we’ve built?”</span></p>
<p><span style="font-weight: 400;">That shift matters, because the hard problem was never the model.</span></p>
<p><span style="font-weight: 400;">The hard problem is what happens when models become infrastructure, when they are embedded into workflows, connected to internal systems, calling APIs, invoking tools, moving data across boundaries, and increasingly operating with partial autonomy. At that point, the LLM is no longer a novelty. It becomes part of your value chain.</span></p>
<p><span style="font-weight: 400;">And value chains, if left ungoverned, become liabilities.</span></p>
<p><span style="font-weight: 400;">Today, I’m very pleased to announce that </span><b>Tyk AI Studio is going open source</b><span style="font-weight: 400;">.</span></p>
<p><span style="font-weight: 400;">Tyk is an Open Source company, we are strong advocates of open standards, and open formats. I am personally a big believer that in order to continue to foster innovation, open source must thrive (and yes, in the age of AI even open source projects are coming under strain). </span></p>
<p><span style="font-weight: 400;">Taking AI Studio open source is a deliberate architectural decision about how AI infrastructure should evolve.</span></p>
<p><img alt="" class="alignnone wp-image-7522 size-large" height="563" src="https://tyk.io/wp-content/uploads/2026/03/Tyk-AI-studio-analytics--1024x721.png" width="800" /></p>
<h2>The AI value chain is fragmenting</h2>
<p><span style="font-weight: 400;">If you’ve read my previous writing, you’ll know I tend to frame AI as a value chain rather than a product. That framing becomes more useful every month.</span></p>
<p><span style="font-weight: 400;">We have model vendors competing aggressively and evolving rapidly. We have orchestration layers and emerging standards such as MCP and A2A attempting to normalise interaction patterns. We have internal data sources being wired into RAG pipelines. We have agents that can trigger APIs and external tools. And we have compliance teams trying to keep up with all of this.</span></p>
<p><span style="font-weight: 400;">Each of these layers moves independently. Each introduces its own risk surface. And very few organisations have a unifying control plane across them.</span></p>
<p><span style="font-weight: 400;">What many enterprises currently have is not an AI architecture, but a growing collection of integrations that work… until they don’t.</span></p>
<p><span style="font-weight: 400;">AI Studio exists to address that structural gap. It acts as the AI Gateway layer of what we call the AI Control Stack: a policy-driven, observable, extensible layer that sits between your organisation and the evolving AI value chain.</span></p>
<h2>Open source is structural, not ideological (ok maybe it’s a bit ideological)</h2>
<p><span style="font-weight: 400;">The obvious question is: </span><i><span style="font-weight: 400;">but why open source?</span></i></p>
<p><span style="font-weight: 400;">The answer is pretty mundane…</span></p>
<p><span style="font-weight: 400;">We cannot build a durable governance layer for a system that is changing this quickly if that governance layer itself is closed and fixed. New vendors appear, pricing models shift, standards evolve, internal use cases change, and regulation tightens. If your control plane can only adapt at the speed of a vendor roadmap, you are permanently behind.</span></p>
<p><span style="font-weight: 400;">Open source flips that dynamic: it enables a community to respond to change faster than any single team could. </span></p>
<p><span style="font-weight: 400;">We’ve seen this play out in API infrastructure over the last decade. The organisations that retained control of their APIs were the ones that owned their control plane. AI will be no different.</span></p>
<p><img alt="" class="alignnone wp-image-7525 size-large" height="562" src="https://tyk.io/wp-content/uploads/2026/03/Tyk-AI-studio-complince-1024x719.png" width="800" /></p>
<h2>Extensibility is the point</h2>
<p><span style="font-weight: 400;">One of the first conclusions we reached while building AI Studio is that there is no “standard” AI architecture in the enterprise. Some organisations are embedding copilots into internal tooling. Others are exposing AI-powered features in customer-facing products. Many are experimenting with autonomous agents.</span></p>
<p><span style="font-weight: 400;">Any platform that assumes a fixed pattern of use will eventually constrain its users.</span></p>
<p><span style="font-weight: 400;">So instead of hardcoding assumptions, we built AI Studio around extensibility. The AI Gateway provides the core capabilities (routing, governance, observability, cost control), but the real power lies in the plugin ecosystem and developer environment that surrounds it.</span></p>
<p><span style="font-weight: 400;">If you need custom model selection logic, you can build it.</span></p>
<p><span style="font-weight: 400;">If you need proprietary guardrails, you can implement them.</span></p>
<p><span style="font-weight: 400;">If you need specialised pre- or post-processing, you can inject it.</span></p>
<p><span style="font-weight: 400;">If you want to integrate internal systems, MCP servers, or domain-specific tooling, you can extend the gateway rather than working around it.</span></p>
<p><span style="font-weight: 400;">If you need a new, completely custom UI &#8211; you can add it.</span></p>
<p><span style="font-weight: 400;">This is not about shipping features faster than competitors. It’s about ensuring that your AI control plane can evolve at the same pace as your AI usage.</span></p>
<h2>This was fun…</h2>
<p><span style="font-weight: 400;">On a more personal level, building AI Studio has been energising in a way that feels familiar. It reminds me of the early days of Tyk, when I was hacking away in my living room with a bottle of wine hiding under a blanket (yes, there is a photo… unfortunately).</span></p>
<p><span style="font-weight: 400;">The difference now is that we’re not building in isolation. We have an exceptional team, and we have customers deploying serious AI systems in production. Their feedback has shaped this platform in very concrete ways. The direction of AI Studio is informed by real deployment constraints, real governance requirements, and real operational complexity.</span></p>
<p><span style="font-weight: 400;">There’s something uniquely motivating about working in a space that is moving quickly while also having the benefit of experience and community behind you. It creates a kind of disciplined experimentation, which is rare.</span></p>
<h2>Democratizing AI Means Owning the Control Plane</h2>
<p><span style="font-weight: 400;">“Democratizing AI” is a phrase that gets used loosely. Often, it implies simplification — hiding complexity behind abstraction. That’s not what we mean.</span></p>
<p><span style="font-weight: 400;">AI is inherently complex because it is embedded in systems that are complex. Democratization, in this context, means giving enterprises the ability to participate in that complexity without surrendering control to it. It means enabling vendor independence. It means making policy enforceable. It means giving teams visibility into cost, risk, and behaviour, and it means allowing organisations to extend their systems safely rather than relying on opaque black boxes.</span></p>
<p><span style="font-weight: 400;">Open source is how we make that credible.</span></p>
<p><span style="font-weight: 400;">By open sourcing AI Studio, we are inviting architects, developers, and platform teams to help shape the control plane that will underpin the agentic era. The Community Edition provides the foundation. Enterprise capabilities build on top for organisations that require deeper operational and governance tooling.</span></p>
<p><span style="font-weight: 400;">But the core — the AI Gateway, the UI control plane, and its extensibility model — is open.</span></p>
<p><span style="font-weight: 400;">Because the AI value chain is not stabilising any time soon. If anything, it is accelerating. The only sustainable response is to build infrastructure that is transparent, adaptable, and extensible by design.</span></p>
<p><span style="font-weight: 400;">We’re excited to take that step.</span></p>
<p><span style="font-weight: 400;">And we’re even more excited to build it in the open.</span></p>
<p><span style="font-weight: 400;">— Martin</span></p>
<p>The post <a href="https://tyk.io/blog/ai-studio-is-going-open-source-and-why-the-ai-control-plane-must-be-extensible/">AI Studio is going Open Source (and why the AI Control Plane must be extensible)</a> appeared first on <a href="https://tyk.io">Tyk API Management</a>.</p>
