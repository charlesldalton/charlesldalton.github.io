# charlesldalton.github.io

University Scholars Program e-portfolio. Plain HTML and CSS — no build step, no
dependencies. Edit the `.html` files directly and push.

## Publish it

1. Create the repository on GitHub named exactly **`charlesldalton.github.io`** (public).
2. Put every file in this folder at the **root** of the repository — not inside a subfolder.
3. Push to the `main` branch.
4. In the repository, go to **Settings → Pages** and set *Source* to
   **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. Wait a minute or two, then open **https://charlesldalton.github.io**.

If you already have the repo cloned:

```bash
cp -r * /path/to/charlesldalton.github.io/
cd /path/to/charlesldalton.github.io
git add .
git commit -m "Add e-portfolio"
git push
```

Public accessibility is a program requirement: the repository must be **public**,
and Pages must be enabled. Open the live URL in a private browsing window to
confirm it loads without you being signed in.

## Files

| File | What it is |
| --- | --- |
| `index.html` | About / landing page — headshot, summary line, bio, research interests |
| `research.html` | Index of the four research projects |
| `research-ornl.html` | Project page: double-pulse LIBS at Oak Ridge |
| `research-hartig.html` | Project page: Hartig Lab optical diagnostics |
| `research-ncsu.html` | Project page: SALT furnace at NC State |
| `research-jung.html` | Project page: Jung Lab GC–MS |
| `coursework.html` | Majors, courses, honors, involvement |
| `cv.html` | CV download button plus featured sections |
| `styles.css` | All styling |
| `assets/Charles_Dalton_CV.pdf` | The downloadable CV |
| `images/` | Your photos go here |

## Before you publish — three things to do

**1. Add your photos.** See `images/README.txt`. Each slot in the HTML is a
dashed placeholder box with the replacement `<img>` tag written right above it in
a comment. Drop the file in `images/`, delete the placeholder `<div>`, paste the
`<img>` tag in, and write a real `alt` description.

**2. Check the details I inferred.** Search the HTML for these and correct them:

- `research-hartig.html` — the department line says "Nuclear Engineering Program".
  Use whatever wording Dr. Hartig's group uses officially.
- `research-jung.html` — the PI is listed as "Dr. S. Jung". Fill in the full name
  and the correct department.
- `coursework.html` — the course codes are plausible but not taken from your
  transcript. Fix or replace them; the list does not have to be exhaustive.
- `research-ornl.html` — the focus and responsibilities sections describe findings
  from the manuscript that is still in preparation. Check with Dr. Andrews and
  Dr. Kitzhaber about what is fine to state publicly before this goes live.

**3. Update the CV.** `assets/Charles_Dalton_CV.pdf` is the resume you uploaded.
Replace the file whenever you update it — keep the same filename and every
download button keeps working.

## Editing

Every page shares the same header, footer, and stylesheet, so if you change the
navigation or the contact block, change it in all eight HTML files. The contact
section lives in the `<footer class="site-foot">` block at the bottom of each page.
