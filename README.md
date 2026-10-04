# Yidong Zhang

Personal academic homepage for GitHub Pages:

**https://dongdongjun-destiny.github.io**

The site uses [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io), the same Academic Pages / Minimal Mistakes–family Jekyll theme as [Chi Kit Ng’s homepage](https://ngchikit.github.io/). Content is taken from the English CV in `files/Yidong_Zhang_CV.pdf`.

## Enable GitHub Pages

After this branch is merged into `main`:

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.
3. The workflow in `.github/workflows/pages.yml` builds Jekyll and deploys to `https://dongdongjun-destiny.github.io`.

Alternative (no Actions): set **Source** to **Deploy from a branch**, branch `main`, folder `/ (root)`. The `Gemfile` uses the `github-pages` gem and only GitHub Pages–supported plugins, so the built-in Jekyll builder also works. Use one method or the other, not both.

`url` is `https://dongdongjun-destiny.github.io` and `baseurl` is empty in `_config.yml` (correct for a user site).

## Replace the photo

The sidebar currently uses a neutral initials placeholder.

1. Add a square photo (about 512×512 px works well), for example `images/yidong.jpg`.
2. In `_config.yml`, set:

   ```yaml
   author:
     avatar: "images/yidong.jpg"
   ```

3. Optional: regenerate favicons from the same photo and replace the files in `images/` (`favicon.ico`, `favicon-32x32.png`, `apple-touch-icon.png`, `android-chrome-512x512.png`, …).

## Edit content

| What | Where |
| --- | --- |
| Name, affiliation, email, GitHub, photo path | `_config.yml` (`author:`) |
| Top navigation | `_data/navigation.yml` |
| About / bio | `_pages/about.md` |
| News | `_includes/sections/news.md` |
| Publications (home and `/publications/`) | `_includes/sections/pub.md` |
| Research experience | `_includes/sections/research.md` |
| Education | `_includes/sections/education.md` |
| Industry experience | `_includes/sections/industry.md` |
| Patents | `_includes/sections/patents.md` |
| Honors | `_includes/sections/honors.md` |
| Downloadable CV | replace `files/Yidong_Zhang_CV.pdf` |

In author lists, keep **Yidong Zhang** in bold (`**Yidong Zhang**`) and mark equal-contribution authors with `*`.

## Build locally

Requires Ruby, Bundler, and a C toolchain.

```bash
bundle config set --local path 'vendor/bundle'
bundle install
bundle exec jekyll serve --host 127.0.0.1 --port 4000
```

Then open http://127.0.0.1:4000. The publications page is at http://127.0.0.1:4000/publications/.

## License

Theme: MIT, [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) (influenced by Minimal Mistakes and Academic Pages). Site content belongs to Yidong Zhang.
