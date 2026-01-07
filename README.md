# NewYearLove - Interactive New Year Greeting

A beautiful, interactive HTML5 application for sharing New Year greetings with animated elements and special effects.

## Features

- 🎄 Animated tree growing animation
- ❄️ Falling snowflakes with random characters
- ⭐ Twinkling stars in the background
- 💡 Decorative lights animation
- 🎀 Ornament decorations
- 🎵 Background audio with interactive playback
- 📊 Integrated with Vercel Web Analytics for visitor tracking

## Project Structure

```
├── index.html              # Main application file
├── file/
│   ├── default.css        # Stylesheet
│   ├── functions.js       # Utility functions
│   ├── love.js            # Core animation logic
│   ├── jquery.min.js      # jQuery library
│   └── jscex-*.min.js     # Jscex async libraries
├── aud.mp3                 # Background audio
├── img.png                 # Main image asset
├── img2.png                # Secondary image asset
├── README.md               # This file
└── VERCEL_ANALYTICS_SETUP.md # Analytics setup guide
```

## How It Works

The application uses Jscex (an async/await style library for JavaScript) to create a sequence of animations:

1. **Seed Animation** - Displays and scales a seed
2. **Grow Animation** - Animates tree growth
3. **Flower Animation** - Adds flowers to the tree
4. **Move Animation** - Animates tree movement with canvas snapshots
5. **Text Animation** - Displays the greeting message with typewriter effect

Additional visual effects include:
- Randomly generated stars that twinkle
- Continuously spawning snowflakes with random characters
- Decorative lights that flash
- Ornamental decorations positioned around the page

## Interactive Elements

- **Canvas Click** - Click on the seed to trigger animations
- **Mouse Hover** - The cursor changes when hovering over the seed
- **Audio Playback** - Background audio plays automatically, with click to restart

## Vercel Web Analytics Integration

This project is integrated with Vercel Web Analytics to track visitor metrics. The analytics are implemented using the HTML-based approach, which is ideal for static HTML applications.

### Analytics Setup

The following scripts are included in `index.html`:

```html
<!-- Vercel Web Analytics -->
<script>
    /* Queue function for early hits */
    window.va =
        window.va ||
        function () {
            (window.vaq = window.vaq || []).push(arguments);
        };
</script>

<!-- Loads the tracker from your own domain -->
<script defer src="/_vercel/insights/script.js"></script>
```

### Viewing Analytics Data

1. Go to your [Vercel Dashboard](https://vercel.com/dashboard)
2. Select this project
3. Click the **Analytics** tab
4. View visitor metrics, page views, and other insights

For detailed setup instructions, see [VERCEL_ANALYTICS_SETUP.md](./VERCEL_ANALYTICS_SETUP.md).

## Deployment

This project is deployed on Vercel. To deploy your own version:

1. Push code to a GitHub/GitLab/Bitbucket repository
2. Connect your repository to Vercel
3. Deploy automatically on every push to main branch

Alternatively, use the Vercel CLI:

```bash
vercel deploy
```

## Browser Compatibility

This application uses modern JavaScript features and canvas rendering. Best viewed in:
- Chrome
- Firefox
- Edge
- Safari (latest versions)

## License

This is a personal project created for sharing New Year greetings with loved ones.

## Getting Started

1. Open `index.html` in a modern web browser
2. Wait for animations to load (seeds and tree will appear)
3. Click on the seed to trigger the full animation sequence
4. Enjoy the interactive greeting and animations!

## Customization

You can customize the greeting message by editing the text in the `<span class="say">` elements in `index.html`:

```html
<span class="say">My  💞</span><br>
<span class="say"> 🎈</span><br>
<span class="say">And give u many happiness 💕</span><br>
```

Feel free to update these messages and add your own personal touch!
