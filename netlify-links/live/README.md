
# WordCamp Larissa 2024 - Dynamic Iframe Rotator

This project dynamically rotates through URLs in an iframe while displaying a progress bar and a splash screen logo during transitions. It’s designed to showcase multiple pages or sponsors for [**WordCamp Larissa 2024**](https://larissa.wordcamp.org).

## Features

- **Dynamic URL Rotation**: Displays different URLs in an iframe, rotating every 31.5 seconds.
- **Progress Bar**: Indicates the time remaining for the current URL.
- **Splash Screen Logo**: Fades in during transitions between URLs.
- **Dynamic JSON File Selection**: Load URLs from different JSON files by passing a query parameter.
- **Automatic Refresh**: Refreshes the page after two full rounds through all URLs to ensure fresh content.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/wordcamp-larissa-2024.git
   cd wordcamp-larissa-2024
   ```

2. Place your JSON data files in the `data/` directory.

3. Open the `index.html` file in your browser.

## Usage

### JSON File Structure

The JSON file should be structured as follows:
```json
{
  "urls": [
    "https://example.com/page1",
    "https://example.com/page2",
    "https://example.com/page3"
  ]
}
```

### Query Parameter for Custom JSON File

To load a custom JSON file, append the `file` query parameter to the URL:
```
index.html?file=data/custom-urls.json
```

### Default Behavior

Without the `file` query parameter, the project defaults to loading `data/live-urls.json`.

## Customization

### Changing Rotation Interval

You can adjust the rotation interval by modifying the `INTERVAL` constant in the `startRotation` function:
```javascript
const INTERVAL = 31500; // 31.5 seconds per URL
```

### Adjusting Fade Duration

Modify the `FADE_DURATION` constant to change the transition speed:
```javascript
const FADE_DURATION = 1500; // 1.5 seconds fade transition
```

### Updating the Splash Screen Logo

Replace the file `images/splash-screen.png` with your custom logo while keeping the same file name, or update the path in the HTML:
```html
<img id="logo" src="images/your-logo.png" alt="Splash Screen Logo">
```

## Development

To modify or extend the project:

- Ensure proper structure in your JSON files.
- Use your browser's developer tools to debug any issues.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to suggest improvements.

## License

This project is licensed under the GPL-3.0 License. See the [LICENSE](https://www.gnu.org/licenses/gpl-3.0.html) file for details.

---

## Acknowledgments

- [**WordCamp Larissa 2024 Team**](https://larissa.wordcamp.org/2024/organotiki-omada/): For organizing an amazing event!
- **Special Thanks**: To all contributors and supporters.
