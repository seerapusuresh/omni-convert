# OmniConvert

**A privacy-first file converter that works in your browser.** Pick a file, inspect the formats OmniConvert can process, then download the result. Files stay on your device.

## Live demo

https://seerapusuresh.github.io/omni-convert/

## Highlights

- Converts PNG, JPEG, WebP, and browser-decodable BMP images. Transparent pixels are placed on white when exporting JPEG.
- Converts between CSV, JSON, and plain text.
- Exports HTML as Word DOCX, RTF, Markdown, or plain text.
- Shows other likely formats as unavailable when the required conversion engine is not included.
- Uses a responsive dark glass interface, animated file analysis, and optional synthetic click sounds.
- Processes files in the browser without sending uploads to a server.

## Run locally

Install Node.js LTS, open this folder in a terminal, then run:

```sh
npm install
npm run dev
```

## Supported output formats

| Input | Available outputs |
| --- | --- |
| PNG, JPEG, WebP | PNG, JPEG, WebP |
| BMP | PNG, JPEG, WebP, when the browser can decode the BMP |
| JSON | CSV, formatted text |
| CSV | JSON, plain text |
| Plain text | JSON, CSV |
| HTML | Word DOCX, RTF, Markdown, plain text |

HTML-to-Word keeps headings and text; complex layout, images, and scripts are not carried over. Browser image conversion can vary by browser. Audio, video, PDF, Office, and archive formats that are not listed above need additional engines and are not currently converted.

## Source code

Download [OmniConvert-source.zip](OmniConvert-source.zip) to inspect or run the complete project, including the Vite configuration, source files, tests, and GitHub Pages workflow.
