# cppingale.me

This site is configured for the custom domain `cppingale.me`, and the CNAME
file has been removed so GitHub Pages will serve from `chinmay-92.github.io`
in the meantime.

The domain is registered and active but has **no DNS records**, so it resolves
nowhere — and while the CNAME file was present, GitHub redirected every request
to it, which made the whole site unreachable rather than just the domain.

To restore it, add four A records for the apex at the registrar:

    185.199.108.153
    185.199.109.153
    185.199.110.153
    185.199.111.153

optionally a CNAME for `www` pointing at `chinmay-92.github.io`, then put the
CNAME file back:

    echo cppingale.me > CNAME

Anything pointing at this site (the Simmer email confirmation page, app-ads.txt
for AdMob) has to name whichever host is live at the time.
