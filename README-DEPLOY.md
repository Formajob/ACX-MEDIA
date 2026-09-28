# ACX Media — temporary Vercel deployment

## Option A — Vercel dashboard

1. Open https://vercel.com/new
2. Import or upload the `acx-media-site` folder.
3. Keep the project as a static site.
4. Do not add a build command.
5. Set the output directory to `.` if Vercel asks for one.
6. Deploy.

Vercel will provide a temporary URL such as:

`https://acx-media-site.vercel.app`

## Option B — Vercel CLI

From this folder:

```bash
npx vercel
```

Follow the login and project prompts. For a production deployment:

```bash
npx vercel --prod
```

The site is a static HTML/CSS/JavaScript website and does not require a build step.

## Contact form note

The current form is a front-end prototype. It displays a confirmation message but does not send email yet. The public contact address shown on the site is:

`media@acx.ma`

To make the form send real messages, connect it later to a form provider or a serverless function.

## Custom domain later

Once `acx.ma` or another domain is purchased:

1. Open the Vercel project.
2. Go to **Settings → Domains**.
3. Add the domain.
4. Copy the DNS records shown by Vercel to the domain registrar.
5. Keep the temporary Vercel URL active as a fallback.
