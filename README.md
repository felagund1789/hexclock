# hexclock

A tiny single-file demo that turns the current time into a hexadecimal color and applies it as the page background.

**What it does**
- Reads the current time (hours, minutes, seconds).
- Formats time as a 6-digit hex string in HHMMSS order (e.g. 12:34:56 → #123456).
- Sets the page background to that color and displays the hex code.
- Updates every second.

**How to use**
- Open the HTML file in your browser (double-click the file or use a local web server).
- The page updates automatically; no build or dependencies required.

**Implementation notes**
- Main logic is plain JavaScript:
  - Pads hours/minutes/seconds with leading zeros.
  - Concatenates them into `#HHMMSS`.
  - Applies it to `document.body.style.backgroundColor` and updates the visible hex string.
- The demo is a single static file suitable for embedding or quick sharing.

**Example**
- 07:05:09 → #070509
- 21:45:03 → #214503

**Possible improvements**
- Add contrast-aware text color for accessibility.
- Smoothly animate transitions between colors.
- Offer alternate mappings (e.g., map time to HSL or to a broader color space).

**Acknowledgements**: Inspired by rushedcar's post on [reddit](https://www.reddit.com/r/unixporn/s/W065s2vPpY)

**License**: Public domain / use as you like.
