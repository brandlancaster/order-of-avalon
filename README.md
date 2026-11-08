# Order of Avalon

Public website of the Order of Avalon. This is the Order site, not the Church of Chivalry site. The Church holds the public creed. The Order is how members live it.

Static HTML and CSS. There is no build step. Publish this repository from the root on Cloudflare Pages or GitHub Pages.

## Pages

| File | Page | Room label |
| --- | --- | --- |
| `index.html` | Home | Gatehouse |
| `the-way.html` | The Way | Chapel / Scriptorium |
| `the-order.html` | The Order | Great Hall |
| `training.html` | Training and Standards | Training Yard |
| `missions.html` | Missions and Programs | Armory |
| `inquire.html` | Inquire | Portcullis |

Shared styles live in `css/styles.css`. The header mark on every page is the seal at `assets/seal.png`. Use that file as it is.

## Local preview

From the repository root:

```bash
python3 -m http.server 8741
```

Open [http://127.0.0.1:8741/](http://127.0.0.1:8741/).

## Inquire form

`inquire.html` includes `#inquire-form` with `method="post"` and required fields `name`, `email`, and `message`. There is no `action` URL yet. Set `action` to the form endpoint when you deploy. Until an `action` is set, the page tells the visitor that nothing was sent. It does not report a successful submission.

A `.nojekyll` file is included so GitHub Pages serves the site as plain files.
