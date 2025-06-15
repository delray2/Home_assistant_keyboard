# Onscreen Dashboard Keyboard

A customizable onscreen keyboard template for Home Assistant dashboards. Easily add a virtual keyboard to your Lovelace UI for touchscreens, kiosks, or accessibility needs.

## Installation

### HACS (Recommended)
1. Go to HACS in your Home Assistant sidebar.
2. Click on "Custom repositories" (three dots in the top right).
3. Add this repository URL as a repository.
4. Search for "Onscreen Dashboard Keyboard" in HACS and install.
5. After installation, reload your browser.

### Manual
1. Download `onscreen-keyboard.js` from the `www/` folder in this repository.
2. Place it in your Home Assistant `www/` directory (create it if it doesn't exist).
3. Restart Home Assistant or reload resources.

## Adding to Lovelace

1. Go to **Settings > Dashboards > Resources** in Home Assistant.
2. Click **Add Resource**.
3. URL: `/local/onscreen-keyboard.js`
4. Resource type: `JavaScript Module`
5. Save and refresh your dashboard.

## Usage Example

Add the custom element to your Lovelace dashboard YAML or through the UI:

```yaml
- type: custom:onscreen-keyboard
  layout: qwerty
  theme: dark
  target_entity: input_text.keyboard_input
```

- `layout`: Keyboard layout (e.g., `qwerty`, `numeric`).
- `theme`: Visual theme (`dark`, `light`).
- `target_entity`: The Home Assistant entity to receive keyboard input.

## License

This project is licensed under the MIT License. 