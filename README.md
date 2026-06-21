# The Armchair Gazette — How to Use This Site

This is a single self-contained website. No installation, no server, no database —
just one HTML file plus an images folder.

## Opening it
Double-click `index.html` and it opens in any browser, on a computer or phone.
That alone works as a finished gift — nothing else required.

## Adding a new article
Open `index.html` in any text editor and find the `const articles = [ ... ]` list
near the bottom (search for "ARTICLE DATA"). Copy one of the existing entries and
add a comma-separated object above or below it with these fields:

- `id` — a unique short slug, no spaces, e.g. `"rose-bowl-1998"`
- `title` — the headline
- `date` — `"YYYY-MM-DD"` (this controls the order — newest date appears first)
- `author` — the writer's name
- `sport` — a short label like `"Football"` or `"Hockey"` (optional)
- `image` — path to the photo, e.g. `"assets/images/your-photo.jpg"`
- `caption` — a short italic caption shown under the photo (optional)
- `excerpt` — a one or two sentence teaser shown on the home page
- `body` — the article text, written as a list of paragraphs, e.g.
  `["First paragraph...", "Second paragraph...", "Third paragraph..."]`

Save the file and refresh the browser — the new article appears automatically,
sorted into place by date. No other code needs to change.

## Adding a photo
Drop the image file into the `assets/images` folder, then reference its filename
in the `image` field above. Keep one or two photos per article, as planned.
Photos are automatically given a soft vintage tint to match the front-page look,
so even ordinary phone photos will fit the style.

## Hosting it online (optional)
If you'd rather share a link instead of a file:
- Drag the whole folder onto **netlify.com/drop** for an instant free link, or
- Create a free GitHub repository, upload the folder, and enable **GitHub Pages**
  in the repo settings.

Either way works on mobile and desktop with no changes to the code.

## Sending Claude more articles later
Just upload the new article text (and photo, if you have one) in a chat with
Claude and ask for it to be added to this site — paste in this same `index.html`
file so the new entry can be appended in the right place.
