# A Garden For You

A romantic, interactive website built around white lilies. It is a single self-contained file: `garden.html`.

## How to open it

- **Locally:** double-click `garden.html`. It opens in any modern browser.
- **Online:** upload the file to any static host (GitHub Pages, Netlify, Cloudflare Pages) and share the link.
- **On a phone:** send her the hosted link. The page is built for phone and desktop widths.

An internet connection is only needed for the Google Fonts. Without it the page falls back to system fonts and still works.

## What's in it

1. **Opening screen.** Lilies slowly bloom, then the greeting and the "Open your little surprise" button appear.
2. **A little reminder for you.** A bouquet of lilies blooms while the messages appear one by one as she scrolls.
3. **Things I adore about you.** A flower bed of eight lilies. Tapping one makes it bloom and reveals a message. Opening all eight unlocks a bonus line and a petal shower.
4. **A garden of compliments.** A vine grows as she scrolls, and a lily blooms beside each compliment.
5. **A final letter.** Handwritten-style text on cream paper, fading in line by line.
6. **Finale.** "You're my favourite flower in a garden full of lilies," with a shower of hundreds of petals and a button to replay it.

Extras:

- Soft background music toggle, off by default (top right).
- Floating back-to-top button.
- Six hidden glowing sparkles that reveal little notes, with a counter at the end.
- Floating petals, glowing particles, and a sparkle trail that follows the mouse.
- Reduced-motion support for people who turn animations off.

## Music

The music is generated in the browser with the Web Audio API (soft chords and bell tones), so there is no audio file to host. Browsers only allow sound after a tap, which is why it starts when she presses the toggle.

## Customising

Everything is inside `garden.html`. Search for the names below.

| To change | Search for |
| --- | --- |
| Opening greeting and button | `class="to"`, `class="sub"`, `id="open"` |
| The five reminder messages | `class="msg` |
| The eight garden messages | `const MSG` |
| The eight walk compliments | `const WALK` |
| Hidden sparkle notes | `data-msg=` |
| Letter text | `const P1` and the `p2` line below it |
| Final line | `class="final-line"` |
| Colours and fonts | the `:root` block at the top of the `<style>` |

Tip: if you want to add her name, put it in the opening greeting or at the top of the letter.

## Notes

- No tracking, no accounts, no data leaves the page.
- Tested for script syntax only. Open it on a phone and a computer before sending it, and check that the music toggle works on her device.
