# feedme-core 🍔

The open-source engine behind [feedme](https://github.com/sirmews/feedme): turn any RSS/Atom feed into a permanent, SEO-optimized static website.

## Usage

```bash
# From a config file
bunx feedme-core build --config feedme.json

# Or directly from a feed URL
bunx feedme-core build --url https://news.ycombinator.com/rss
```

By default, output is written to `./content`.

## Config (`feedme.json`)

```json
{
  "feedUrl": "https://news.ycombinator.com/rss",
  "outputDir": "./content",
  "llmDefense": {
    "enabled": true,
    "injectHiddenPrompts": true
  }
}
```

## License

MIT
