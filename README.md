# X Speed Controller

A Chromium extension that adds a popup to your toolbar with:

- An **on/off** toggle
- A **speed slider** from `0.1x` to `4.0x` (default: `2.0x`)
- A **Turbo** speed slider from `2.0x` to `4.0x` (default: `2.0x`)

When enabled, X videos play at the chosen speed automatically. When disabled, playback returns to normal (`1.0x`). Settings sync across browsers through `chrome.storage.sync`.

<video src="https://github.com/user-attachments/assets/12213146-d3af-4315-9571-251ec27cccb6" width="100%" controls></video>

## Install (unpacked, dev mode)

1. Open `chrome://extensions`
2. Toggle **Developer mode** on (top right)
3. Click **Load unpacked**
4. Select this folder

The icon will appear in your toolbar, click it to open the popup.

## Files

| File           | Intent                                                      |
| -------------- | ----------------------------------------------------------- |
| `manifest.json`| MV3 manifest                                                |
| `popup.html`   | Toolbar popup (toggle, sliders, speed display)              |
| `popup.js`     | Popup logic, reads/writes settings via `chrome.storage.sync`|
| `content.js`   | Sets the playback rate, deals with X's SPA nav              |
| `icon.png`     | Icon                                                        |

## Notes

Built upon the previous code of the [Youtube Speed Controller](https://github.com/AsLeonardo/Youtube_Speed_Controller) repository, therefore, may contain redundant code.

## Mentions

Inspired by [dobval/youtube2x](https://github.com/dobval/youtube2x), a script in which it hardcodes 2x playback on YouTube.\
This extension aims to widen it, through an UI, a switch and an adjustable slider.

## License

[MIT](LICENSE)
