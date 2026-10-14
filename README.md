# CV

Federico Bello's CV. The source is `cv.html`; a GitHub Action renders it to PDF with headless Chrome and publishes it to the `build` branch, served by GitHub Pages at <https://fede-bello.github.io/cv/> (redirects to `cv.pdf`).

## Local build

```sh
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --no-pdf-header-footer \
  --virtual-time-budget=10000 --print-to-pdf=cv.pdf "file://$PWD/cv.html"
```

The build fails if the PDF is not exactly one page.
