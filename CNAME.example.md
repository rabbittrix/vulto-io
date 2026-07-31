# Custom domain setup for Vulto.io

GitHub Pages is live at:
https://rabbittrix.github.io/vulto-io/

`vulto.io` will not resolve until DNS exists at your registrar.

## DNS records (apex)

| Type | Name | Value |
|---|---|---|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| AAAA | `@` | `2606:50c0:8000::153` |
| AAAA | `@` | `2606:50c0:8001::153` |
| AAAA | `@` | `2606:50c0:8002::153` |
| AAAA | `@` | `2606:50c0:8003::153` |
| CNAME | `www` | `rabbittrix.github.io` |

## After DNS propagates

1. Create `dist-web/CNAME` with a single line: `vulto.io`
2. In GitHub → `rabbittrix/vulto-io` → Settings → Pages → Custom domain: `vulto.io` → Enforce HTTPS
3. Push `dist-web/CNAME` so deploys keep the domain
