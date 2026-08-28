# Reading Tracker

A single-file progress tracker for Redwood Research's
[AI futurism reading list](https://blog.redwoodresearch.org/p/ai-futurism-reading-list):
the 43 compulsory ("Recommended") readings of the four core weeks, with links,
time estimates, and the starred ~1-hour priority markers. A pixel owl walks
along the progress bar as you read and gets a party hat at 100%.

## Usage

Open `index.html` in a browser. No build step, no dependencies, works offline.

- Weeks expand into individual readings; tick a reading when done.
- Each row has an optional notes field; paste a URL and an "open" link appears.
- Open/closed state of the weeks is remembered.
- Progress lives in the browser's localStorage. Use "Export progress.json" to
  snapshot it and "Import" to restore it on another machine.

## Adapting to your own reading list

All data is the `READINGS` constant near the top of the script in
`index.html`: an array of `{name, items}` groups, where each item is
`{t: title, url, star: 0|1, time: "30 min"}`. Edit it in place.

## Contributing

Bug reports and pull requests are welcome via
[GitHub issues](https://github.com/yulia-volkova/reading-tracker/issues).

## License

MIT. The reading list itself is Redwood Research's; see the link above.
