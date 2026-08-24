# Instructions

### Adding a New Redirect

To add a new redirect:

1. In `src/middleware.ts`, add a new entry to `hostRedirectMap`.
2. In **Cloudflare DNS**, create a **CNAME record** for the desired subdomain pointing to `redirect-things.vercel.app`.
3. In the **Vercel project**, add the subdomain as a **Project Domain** so Vercel recognizes and accepts requests for it.

After the DNS record has propagated and the domain is configured in Vercel, the subdomain will redirect to the destination configured in `hostRedirectMap`.
