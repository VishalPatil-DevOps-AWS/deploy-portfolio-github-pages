## Deploy Your Portfolio Free with GitHub Pages


<img width="1000" height="420" alt="cover" src="https://github.com/user-attachments/assets/a8c9684e-ee35-4f76-90ed-c0373ddfa76a" />



##A portfolio on your laptop helps no one. A live link on your resume helps everyone.

This guide shows how to put a static portfolio (HTML, CSS and JavaScript) online for free in about 30 minutes, with no command line. At the end, it shows how to take the same files to AWS.

**See it live:** https://vishalpatil-devops-aws.github.io/portfolio/

## What you need

- A free GitHub account
- GitHub Desktop (https://desktop.github.com)
- Your portfolio folder, with `index.html` in it

## Deploy in 6 steps

1. **Create a public repository** named exactly `<username>.github.io`, with a README.
2. **Clone it** in GitHub Desktop (File > Clone repository).
3. **Copy your files in.** Copy the *contents* of your portfolio folder, not the folder itself. `index.html` must sit at the top level.
4. **Commit and push.** Write a message like `Add portfolio website`, click **Commit to main**, then **Push origin**.
5. **Turn on Pages.** Go to Settings > Pages, choose **Deploy from a branch**, then `main` and `/ (root)`, and click Save.
6. **Wait 1 to 3 minutes.** Your site is live at `https://<username>.github.io/`.

> **Tip:** Your username becomes your web address, so pick a professional one.

## Something broke?

| Problem | Fix |
|---|---|
| 404 error | Move `index.html` to the repository root and check Settings > Pages |
| CSS or images missing | GitHub is case-sensitive. Match file names exactly and use paths like `css/style.css` |
| Site not updating | Push your changes, wait for the green tick in Actions, then press Ctrl + F5 |
| Push rejected | Pull origin, then push again |

## Updating later

Edit your files, commit, push. GitHub Pages redeploys automatically.

## Next: take it to AWS

The same HTML, CSS and JS files can run on AWS, which makes this a great first cloud project:

- **AWS Amplify:** connect your GitHub repo and it redeploys on every push.
- **Amazon S3:** host the files as a static website.
- **S3 + CloudFront + Route 53:** the production-style setup, with HTTPS and a custom domain.

> **Warning:** AWS can generate charges. Set a billing alarm
