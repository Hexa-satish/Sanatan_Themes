# Sanatan Keyboard Themes

Public theme asset repository for [Sanatan Keyboard](https://github.com/BitIndianCoder/SanatanKeyboard).

Hosts **5 remote themes** with keys, backgrounds, and preview images. The keyboard app fetches `themes.json`, shows previews in the theme grid, downloads assets on apply, and applies them to the IME.

## Theme structure

Each theme folder contains:

```
themes/{theme_id}/
├── preview.png          # Grid thumbnail
├── keyboard_image.png   # Keyboard background
├── colorcode.png        # Text color sample (center pixel used)
├── mdpi/
│   ├── key_presed.9.png
│   ├── key_unpresed.9.png
│   └── popup_bg.9.png
├── hdpi/
├── xhdpi/
└── xxhdpi/
```

## Themes

| ID | Name | Category |
|----|------|----------|
| `ganesh_gold` | Ganesh Gold | ganesh |
| `hanuman_strength` | Hanuman Strength | hanuman |
| `krishna_bliss` | Krishna Bliss | krishna |
| `lotus_serenity` | Lotus Serenity | lotus |
| `shiv_shakti_glow` | Shiv Shakti Glow | shiv_shakti |

## App integration

1. Push this repo to GitHub as a **public** repository.
2. Update `base_url` in `themes.json` with your GitHub username.
3. In the keyboard app, set the same URL in `RemoteThemeConstants.REMOTE_MANIFEST_URL`.

The app downloads themes to:

```
{app_external_files}/remote_themes/{theme_id}/theme0/
```

## Adding a new theme

1. Create `themes/your_theme_id/` with the structure above.
2. Add an entry to `themes.json`.
3. Commit and push.

## License

Assets are provided for use with Sanatan Keyboard. Replace placeholder key images with your own designs before production release.
