---
title: "Two ways to deal with NGINX killing its Ingress Controller"
url: "https://tyk.io/blog/two-ways-to-deal-with-nginx-killing-its-ingress-controller/"
date: "Tue, 03 Feb 2026 17:36:05 +0000"
author: "Jennifer Craig"
feed_url: "https://tyk.io/feed/"
---
<p><span style="font-weight: 400;">NGINX has decided you’ll be migrating in the near future. From March 2026, it will deprecate its Ingress Controller. While existing deployments will continue to function, and installation artifacts will remain available, it’s a slippery downhill slope from March onwards. As NGINX puts it: </span></p>
<p><em><span style="font-weight: 400;">“There will be no further releases, no bugfixes, and no updates to resolve any security vulnerabilities that may be discovered.”</span></em></p>
<p><span style="font-weight: 400;">Ouch. If your cluster depends on NGINX’s Ingress Controller, you’re on borrowed time.</span></p>
<p><span style="font-weight: 400;">Thankfully, you have two ways forward with Tyk, both of which deliver clear benefits. </span></p>
<ol>
<li><b> Replace it fast</b></li>
</ol>
<p><span style="font-weight: 400;">If you’re after a low-risk, fast migration, we’ve got you. You can swap the NGINX Ingress Controller for Tyk’s Ingress mode. Doing this means you can:</span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Keep your Ingress YAML</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Change the Ingress class </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Deploy Tyk Gateway and Tyk Operator</span></li>
</ul>
<p><span style="font-weight: 400;">Speedy, simple, secure. Learn how to use Tyk Operator as an Ingress Controller to manage your API traffic in Kubernetes </span><a href="https://tyk.io/docs/product-stack/tyk-operator/tyk-ingress-controller"><span style="font-weight: 400;">here</span></a><span style="font-weight: 400;">.</span></p>
<p><span style="font-weight: 400;">This’ll carry over your basic proxy routing – you’ll need to map any additional gateway rules stored via annotations, such as mTLS, to Tyk via API definition.  </span></p>
<ol start="2">
<li><b> Upgrade your architecture</b></li>
</ol>
<p><span style="font-weight: 400;">You have to migrate anyway, so why not use this as an opportunity to lay stronger foundations for a better future? You can stop using Ingress to define APIs and use Custom Resource Definitions (CRD) to do so instead. </span></p>
<p><span style="font-weight: 400;">When you migrate to using Tyk Gateway to define API Proxies with Tyk CRDs/OpenAPI, you don’t just replace routing – you gain a whole heap of benefits: </span></p>
<ul>
<li style="font-weight: 400;"><span style="font-weight: 400;">Store your proxies in the API best practice standard &#8211; </span><b>OpenAPI Specification</b></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Authorisation and authentication options that make robust security simple (JWT, OIDC, mTLS, API keys)</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Flexible rate limit and quota options to help you safeguard against abuse, overload, and denial-of-service attacks</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Powerful security and governance policies for efficient, consistent management at scale</span></li>
<li style="font-weight: 400;"><a href="https://tyk.io/pricing/"><span style="font-weight: 400;">Pricing plans</span></a><span style="font-weight: 400;"> that fit your API journey and don’t penalize your business for growth</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Detailed analytics that enable you to log, measure and trace efficiently for faster troubleshooting, slowdown prevention, improved end-user experiences and better business decisions</span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">API versioning that delivers flexibility and stability, for superior transition management </span></li>
<li style="font-weight: 400;"><span style="font-weight: 400;">Secure, flexible API governance designed to support innovation at scale while helping you streamline compliance </span></li>
</ul>
<p><span style="font-weight: 400;">By upgrading your architecture with Tyk Gateway, you move from just routing traffic with the NGINX Ingress Controller to building a real API platform that’s future-ready in every sense. </span></p>
<p><span style="font-weight: 400;">We have a quick-start repo to help you migrate from Ingress to CRD </span><a href="https://github.com/TykTechnologies/ingress2tyk/tree/main"><span style="font-weight: 400;">here</span></a><span style="font-weight: 400;">.</span></p>
<h2><b>Your NGINX Ingress Controller retirement solution </b></h2>
<p><span style="font-weight: 400;">NGINX is forcing your hand – but that doesn’t have to be a negative. Whether you go for the speedy route of replacing the dead Ingress Controller with Tyk’s Ingress mode or take the chance to build a powerful API platform, your business stands to gain. </span></p>
<p><a href="https://tyk.io/contact/"><span style="font-weight: 400;">Chat with our team</span></a><span style="font-weight: 400;"> to find out more or dive in and </span><a href="https://tyk.io/sign-up/"><span style="font-weight: 400;">enjoy a free trial</span></a><span style="font-weight: 400;"> to see for yourself how easy things can be.</span></p>
<p>&nbsp;</p>
<p>The post <a href="https://tyk.io/blog/two-ways-to-deal-with-nginx-killing-its-ingress-controller/">Two ways to deal with NGINX killing its Ingress Controller</a> appeared first on <a href="https://tyk.io">Tyk API Management</a>.</p>
