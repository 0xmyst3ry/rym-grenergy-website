# RYM Grenergy website

A single-page parallax website for RYM Grenergy Solution, an energy-storage startup working on a uni-polar programmed supercapacitor. Plain HTML, CSS and JavaScript, with no build step.

The hardware side of the same project is in [Uni-Polar-Programmed-Supercapacitor](https://github.com/0xmyst3ry/Uni-Polar-Programmed-Supercapacitor).

## Sections

- **Home:** layered parallax hero (base, middle and front layers shift by different amounts as the pointer moves)
- **Who are we?**
- **Meet our team**
- **Achievements:** a timeline whose entries open an event-details dialog

The behaviour is in [`app.js`](app.js) (a single `RYMWebsite` class that respects `prefers-reduced-motion`), the layout in [`index.html`](index.html) and the styling in [`styles.css`](styles.css).

## Run it

It is a static site. Either open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Known gaps

- The achievements gallery refers to images that are not in this repo (`layers/pic1.jpg`, `pic2.jpg`, `pic3.jpeg` and the `tech*.jpg` files), so those thumbnails do not load.
- The jQuery fallback points to `js/jquery-3.6.4.min.js`, which is not included. It is only used if the Google-hosted copy fails to load.

## License

No license has been chosen yet. The repo has more than one contributor and includes the company logo and team photos, so please do not reuse the content without asking.
