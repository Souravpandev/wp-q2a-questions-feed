# Q2A Questions Feed

- Plugin Name: Q2A Questions Feed
- Plugin URI: https://github.com/Souravpandev/wp-q2a-questions-feed
- Description: Display Question2Answer questions from an RSS feed using shortcode or widget
- Version: 1.0.0
- Author: Sourav Pan
- Author URI: https://wpoptimizelab.com/
- Text Domain: q2a-feed
- Domain Path: /languages
- Requires at least: 5.0
- Requires PHP: 7.2

## 📂 Plugin Structure

```text
q2a-questions-feed/
├── admin/
│   ├── class-q2a-feed-admin.php      # Admin interface and settings
│   └── css/
│       └── admin.css                 # Admin-specific styles
├── assets/
│   └── css/
│       └── q2a-feed.css              # Frontend styles
├── includes/
│   ├── class-q2a-feed.php            # Main plugin class
│   ├── class-q2a-feed-functions.php  # Helper functions (class-based)
│   ├── class-q2a-feed-widget.php     # Widget implementation
│   └── q2a-feed-functions.php        # Standalone functions
├── q2a-questions-feed.php            # Main plugin file
├── readme.txt                        # WordPress.org readme
├── README.md                         # GitHub readme
└── uninstall.php                     # Cleanup on uninstall
```

# Q2A Questions Feed - WordPress Plugin

A lightweight WordPress plugin that displays questions from a Question2Answer (Q2A) RSS feed using shortcodes or widgets.

## Features

- Display Q2A questions in any post or page using a simple shortcode
- Add a Q2A questions feed to any widget area
- Customize the number of questions to display
- Toggle display of question dates
- Toggle display of question excerpts
- Control excerpt length
- Built-in caching for better performance
- Responsive design that works on all devices
- Easy to customize with CSS
- Admin settings page for easy configuration

## Requirements

- WordPress 5.0 or higher
- PHP 7.2 or higher
- A Question2Answer installation with RSS feed enabled

## Installation

1. Download the latest release of the plugin as a ZIP file
2. Go to your WordPress admin dashboard
3. Navigate to **Plugins > Add New**
4. Click **Upload Plugin**
5. Select the downloaded ZIP file and click **Install Now**
6. After installation, click **Activate Plugin**

## Configuration

1. After activation, go to **Settings > Q2A Feed** in your WordPress admin dashboard
2. Enter your Q2A RSS feed URL (typically `https://your-q2a-site.com/feed/qa.rss`)
3. Configure the display settings as needed
4. Click **Save Changes**

## Usage

### Shortcode

```php
[q2a_questions]
```

#### Shortcode Parameters

- `count`: Number of questions to display (default: 5)
- `show_date`: Whether to show the date (1 or 0, default: 1)
- `show_excerpt`: Whether to show the excerpt (1 or 0, default: 1)
- `excerpt_length`: Number of words in the excerpt (default: 100)

### Widget

1. Go to **Appearance > Widgets**
2. Find the **Q2A Questions Feed** widget
3. Drag and drop it to your desired widget area
4. Configure the widget settings
5. Click **Save**

## Customization

### CSS Styling

The plugin includes default styles that you can override with your theme's CSS:

```css
.q2a-questions-feed { /* Main container */ }
.q2a-questions-list { /* Questions list */ }
.q2a-question-item { /* Individual question */ }
.q2a-question-title { /* Question title */ }
.q2a-question-date { /* Question date */ }
.q2a-question-excerpt { /* Question excerpt */ }
```

## Troubleshooting

### The feed isn't displaying

1. Verify your Q2A RSS feed URL is correct
2. Check if your Q2A installation has RSS feeds enabled
3. Clear the plugin cache in the settings

### Styling issues

1. Clear your browser cache
2. Check for CSS conflicts with your theme
3. Use browser developer tools to inspect and override styles

## Support

For support, please open an issue on the [GitHub repository](https://github.com/yourusername/q2a-questions-feed/issues).

## Changelog

### 1.0.0
- Initial release

## License

GPLv2 or later
