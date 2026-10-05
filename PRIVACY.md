# Privacy Policy — HomeScreen New Tab

**Last updated:** 2026-10-05
**Applies to:** HomeScreen New Tab (browser extension), versions 2.3.0 and later.

---

## Summary

**We do not collect, store, transmit, or sell any personal data.**

HomeScreen New Tab runs entirely on your device. There is no account, no server, no
analytics, no advertising, and no tracking of any kind. Your browsing history stays
in your browser.

---

## What the extension stores locally

The extension uses `chrome.storage.local` to save your settings **on your own device
only**. This includes:

- Appearance preferences (theme, language, tile size, spacing, colors, blur, motion)
- Tile and folder layout, including the order you drag tiles into
- Which tiles you have hidden
- Your bookmark configuration, if you chose the HTML-file or local-folder source
- A local cache of site icons (`favCache`) so icons still display while offline

This data never leaves your device. Clearing it is a matter of clearing extension
storage, which you can do from the extension's settings or by removing the extension.

## What the extension accesses

The extension requests these browser APIs, and uses each **only** for the feature it
names:

| Permission | Why it is needed |
| --- | --- |
| `bookmarks` | To display your bookmarks and bookmark folders on the new tab page |
| `topSites` | To populate the "Top Sites" section |
| `history` | To populate the "History" section |
| `downloads` | To populate the "Downloads" section, and to open a download when you click it |
| `tabs` | To notice when a tab navigates, so icons can be refreshed after a page loads |
| `favicon` | To read the icon a site already has in your browser's cache |
| `storage` / `unlimitedStorage` | To save your settings and icon cache on your device |
| `<all_urls>` | To download a site's icon file when it is not already cached, so tiles look correct |

## Network requests

The extension makes **one kind of network request**: fetching a website's icon
(`favicon.ico` or a similar icon path) so it can display a tile image.

These requests:

- Go **directly from your browser to the website's own server** (or to the icon
  service the site publishes on its own domain).
- Send **no information about you, your history, or your bookmarks**.
- Transmit only the address of the site whose icon is being requested — the same
  request any browser makes when it displays a tab favicon.
- Use `referrerPolicy: "no-referrer"`, so no referring page URL is sent.

The extension has **no server of its own** and sends nothing to the developer.

## Third parties

None. The extension integrates with no analytics service, no advertising network,
no font CDN, and no telemetry endpoint. It cannot be used to fingerprint you,
because it does not report anything back to anyone.

## Permissions and remote code

The extension contains all of its code inside the extension package. It does **not**
download or execute remote code.

## Children

The extension is suitable for all ages and collects no data from anyone, including
children.

## Changes

If a future version changes what data is handled, this policy will be updated and the
"Last updated" date above will change. Any change that affects data handling will be
noted in the extension's changelog.

## Contact

Questions about this policy are welcome. Contact details are available on the
extension's Chrome Web Store listing.

---

## Store disclosure (for reference when filling in the dashboard)

In the Chrome Web Store "Privacy practices" tab, the accurate answers for this
extension are:

- **Single purpose description:** Replaces the new tab page with a tile-based home
  screen that shows the user's own bookmarks, top sites, history, and downloads.
- **User data collection:** **No** — the extension does not collect any of the listed
  categories of user data. (Fetching a site's own favicon is a network request to
  that site, not collection of user data by the extension.)
- **Data usage:** Not applicable.
- **Data selling:** Not applicable.
- **Data transmission for purposes unrelated to the single purpose:** Not applicable.
- **Independent review of privacy practices:** Not applicable.
