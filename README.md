# ДЪГА — Спомените, които остават

Интерактивно, mobile-first Memory Experience за бивши възпитаници на „Дъга“.

## Local development

```bash
npm install
npm run dev
```

## Environment variables

Copy `.env.example` to `.env.local` and set:

`VITE_WEB3FORMS_ACCESS_KEY=...`

The access key is never committed to the repository.

## Web3Forms setup

The experience submits responses to `https://api.web3forms.com/submit` with the seven memory fields, optional anonymous-quote consent, timestamp and source.

## Vercel deployment

Import the repository into Vercel, use the default Vite build settings (`npm run build`, output `dist`), and add `VITE_WEB3FORMS_ACCESS_KEY` under Project Settings → Environment Variables.

## Custom domain

After deployment, add the desired domain in Vercel's Domains settings and point DNS as instructed by Vercel.

## Notes

- Replace the temporary text logo with the real „Дъга“ logo when available.
- Add a real `public/og-image.jpg` before launch if a custom social preview is desired.
- Keep the Web3Forms key in Vercel/environment configuration, not source control.
