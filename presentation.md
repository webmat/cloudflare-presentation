Cloudflare

    Make the web faster

What is Cloudflare?

    - At its simplest: DNS for your service
    - When you "enable Cloudflare" the magic starts
      - Speed optimizations
      - Security
      - Downtime mitigation
      - Cloudflare apps

How it works:
Reverse proxy

    All traffic goes through them.
    Lets them do a bunch of stuff for you, while you keep your backend simple.
    But let's not get ahead of ourselves.

Per hostname

<pre><img src="cf-on.png"/> www.mysite.com
<img src="cf-off.png"/> sub.mysite.com</pre>

    All features enabled for www
    Only used as a DNS service for sub

What can they do?

  - Security: SSL, WAF, DDoS protection, Email obfuscation, server side exclude,
    Captcha, Hotlink protection
  - Speed optimizations: CDN, Web Content Optimization, SPDY, Railgun
  - Traffic analytics: real vs bots vs attackers, detailed logs
  - Other smart stuff: Always On, Geolocation header, Cloudflare apps, IPV6 support

How expensive?<br>
<pre><p style="text-align:center">0$+<p></pre>

  - DNS
  - Speed: CDN, some WCO (Rocket Loader)
  - Security: basic threat protection
  - Analytics: last 30 days, starting yesterday
  - Smart stuff: Always On, Geolocation header, Cloudflare apps

I'm serious

<pre><li>Pro: 20$, then +5$</li>
<li>Biz: 200$</li>
<li>Ent: Call us (3000$+)</li></pre>

Serious uses

  Let's talk about some of the interesting things

Geolocation<br>
![Country Header](country-header.png)

  Geolocation is IP based and give you the country of the originating request







Setting it up

  Nothing to do for DNS only
  Restore original IP if Cloudflare enabled (optional), since it's a reverse proxy

