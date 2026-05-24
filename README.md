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

- Google: enable Authentication > Providers > Google.
- Kakao: enable Authentication > Providers > Kakao.
- Naver: create a Supabase custom OAuth/OIDC provider with provider id `naver`, then add Naver client credentials. The app calls it as `custom:naver`.
- Add the deployed Netlify URL to Supabase Authentication > URL Configuration > Site URL and Redirect URLs.
