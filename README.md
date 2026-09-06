# NixTrix

A single-page, orange-on-black arcade-style blog. Intended to host short
write-ups that get cross-posted to LinkedIn.

Everything lives in `index.html` — no build step, just open the file or
serve it as a static site (e.g. GitHub Pages).

## Adding a new post

Edit the `posts` array near the top of the `<script>` block in
`index.html`:

```js
const posts = [
  {
    title: "Your post title",
    date: "2026-01-01",
    url: "https://link-to-full-post",
    excerpt: "One-line teaser."
  },
];
```

Newest entries should go first. If the array is empty, the page shows an
"NO ENTRIES FOUND" placeholder instead.
