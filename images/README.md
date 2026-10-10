# Images

## Profile photo — action required

The site expects a profile photo at:

    images/anar.jpg

This is your professional CV headshot. **Add it here** to make it appear in:

- the home-page **hero** (circular avatar, ~140px, beside your name)
- the **About** page **Professional Profile** card (~150px headshot)

### How to add it

1. Save your CV photo as `anar.jpg` and place it in this `images/` folder.
2. Recommended: a **square** crop, at least **400×400px** (600×600 ideal) so it stays
   crisp on high-DPI screens. The CSS crops to a circle with `object-fit: cover`,
   so a square source looks best.
3. Commit and push:

       git add images/anar.jpg
       git commit -m "Add profile photo"
       git push

Until the file exists, the `<img>` tags are set to hide themselves (`onerror`),
so there is **no broken-image icon** — the hero and About card simply render
without a photo.

If you prefer a different filename or format (e.g. `anar.png`), update the
`src="images/anar.jpg"` references in `index.Rmd` and `about.Rmd`.
