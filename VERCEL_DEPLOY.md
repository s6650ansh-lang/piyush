# Deploy with GitHub and Vercel

This is a static website. The project needs no build command or backend.

## Files to put in the GitHub repository

Put these three files together at the repository root:

- `chiku_love_single_file.html`
- `background-song.mp3`
- `vercel.json`

The repository root contains unrelated photos and other files. Do not upload those files for this site.

## Deploy

1. Create a GitHub repository containing only the three files listed above.
2. In Vercel, choose **Add New → Project**, then import that GitHub repository.
3. Set **Framework Preset** to **Other**. Leave the build command and output directory empty.
4. Select **Deploy**. Vercel serves the site at `/`; `vercel.json` routes that URL to the HTML page.
5. Future pushes to the connected GitHub branch will trigger new deployments.

Keep the MP3 beside the HTML file so the background song can load. Browser autoplay restrictions may require visitors to interact with the page before audio starts.
