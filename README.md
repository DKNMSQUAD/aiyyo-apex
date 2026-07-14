Apex redirect shim for aiyyo.in -> https://www.aiyyo.in (the real site, on Cloudflare Pages).

Why: aiyyo.in DNS is hosted on Wix, which supports no ALIAS/ANAME record, so the bare apex cannot CNAME to Cloudflare Pages. GitHub Pages publishes stable apex IPs, so the apex A records point here and this page forwards to www, preserving the path.

Temporary. The permanent fix is moving the aiyyo.in nameservers to Cloudflare and CNAME-flattening the apex to aiyyo-site.pages.dev.
