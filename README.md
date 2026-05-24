# IF Investment Fortune - Astra Oracle

Source snapshot for the Netlify site:

https://sparkly-shortbread-34a8b0.netlify.app/

## Files

- `index.html` - the deployed single-page application source
- `netlify.toml` - Netlify static publish configuration
- `package.json` - minimal project metadata and local preview command

## Local Preview

```bash
npm run dev
```

Then open the printed local URL in a browser.

## Auth Setup

`index.html` uses Supabase Auth with the bundled `supabase.js` browser client.

- Supabase project: `IF (INVESTMENT FORTUNE)` / `srccoltrdxdgstlkkaux`.
- Site URL: `https://sparkly-shortbread-34a8b0.netlify.app`.
- Redirect URLs: add `https://sparkly-shortbread-34a8b0.netlify.app/**`.
- OAuth callback URL for Google/Kakao/Naver developer consoles: `https://srccoltrdxdgstlkkaux.supabase.co/auth/v1/callback`.
- Google: enable Authentication > Providers > Google and save the Google Client ID/Secret.
- Kakao: enable Authentication > Providers > Kakao and save the Kakao REST API Key/Client Secret.
- Naver: create a Supabase custom OAuth/OIDC provider with provider id `naver`, then save the Naver Client ID/Secret. The app calls it as `custom:naver`.
