# FinNLP 2026

Website for **The 11th Workshop on Financial Technology and Natural Language Processing** (FinNLP-2026), co-located with **EMNLP 2026** in Budapest, Hungary (October 24–29, 2026).

Static site — no build step required.

## Structure

```
.
├── index.html                 # Landing page
├── call-for-papers.html       # Call for Papers
├── call-for-challenges.html   # Call for Challenges (shared tasks)
├── .nojekyll                  # Disables Jekyll on GitHub Pages
└── README.md
```

## Local preview

Just open `index.html` in a browser, or serve the directory:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create an empty repo on GitHub (e.g. `finnlp-2026`).
2. Push this directory:

   ```bash
   git remote add origin git@github.com:<your-org>/finnlp-2026.git
   git branch -M main
   git push -u origin main
   ```

3. In the repo settings → **Pages**, set source to **Deploy from a branch**, branch `main`, folder `/ (root)`. The site will be available at `https://<your-org>.github.io/finnlp-2026/`.

   For a custom domain (e.g. `finnlp.org`), add a `CNAME` file at the root containing the domain.

## Update important dates

Edit the `.date-row` entries in `call-for-papers.html` and `call-for-challenges.html`. The `[ TBA ]` placeholders are intentional and should be filled in as dates are finalized.

## Credits

- ACL SIG-FinTech — official reference page: <https://sigfintech.github.io/finnlp.html>
- Proceedings archive: <https://aclanthology.org/venues/finnlp/>
- Contact: <aclsigfintech@gmail.com>
