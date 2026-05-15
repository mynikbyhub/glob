# Global Free IPTV Web Application

A fully functional, lightweight IPTV streaming application optimized for low-bandwidth environments (2G/3G) and unstable network connections. Stream live TV channels from Pakistan, India, and around the world.

![IPTV App](https://img.shields.io/badge/License-MIT-blue.svg)
![Bandwidth](https://img.shields.io/badge/Optimized-2G%2F3G-green.svg)

## Features

- **📺 Live TV Streaming**: Stream free-to-air channels from Pakistan, India, and global sources
- **🌐 Network Resilience**: Adaptive bitrate handling with auto-reconnect for unstable connections
- **📱 Mobile-First Design**: Fully responsive interface optimized for smartphones, tablets, and desktops
- **⚡ Low Bandwidth Mode**: Toggle for reduced stream quality to save data on slow connections
- **🎯 Category Navigation**: Browse channels by country (Pakistan/India) or type (News/Sports/Entertainment)
- **🔄 Auto-Retry Logic**: Automatically attempts to reconnect on stream failures
- **🎨 Modern UI**: Clean, intuitive interface with dark theme

## Technology Stack

- **HTML5**: Semantic markup for structure
- **CSS3**: Custom responsive styling with mobile-first approach
- **Vanilla JavaScript**: No heavy frameworks for optimal performance
- **Video.js**: Professional-grade video player
- **HLS.js**: HTTP Live Streaming support for m3u8 streams
- **Font Awesome**: Icon library (via CDN)

## Quick Start

### Option 1: Run Locally

1. **Download the Project**
   ```bash
   git clone https://github.com/yourusername/global-free-iptv.git
   cd global-free-iptv
   ```

2. **Open in Browser**
   - Simply open `index.html` in any modern web browser
   - No server required! Works directly from file system

3. **Start Watching**
   - Select a category from the sidebar
   - Click on any channel to start streaming

### Option 2: Deploy to GitHub Pages

1. **Create a GitHub Repository**
   - Go to [GitHub](https://github.com) and create a new repository
   - Name it something like `iptv-app`

2. **Upload Files**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/iptv-app.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository settings
   - Scroll to "Pages" section
   - Select "main" branch as source
   - Click Save

4. **Access Your Site**
   - Your site will be available at: `https://yourusername.github.io/iptv-app/`
   - Wait 1-2 minutes for deployment

### Option 3: Deploy to Netlify

1. **Drag and Drop**
   - Visit [Netlify Drop](https://app.netlify.com/drop)
   - Drag the entire project folder
   - Get instant live URL

2. **Or Use Netlify CLI**
   ```bash
   npm install -g netlify-cli
   netlify deploy --prod
   ```

### Option 4: Deploy to Vercel

1. **Install Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **Deploy**
   ```bash
   vercel --prod
   ```

## File Structure

```
global-free-iptv/
│
├── index.html          # Main application file (standalone)
├── README.md           # Documentation (this file)
└── channels.json       # Optional: External channel configuration
```

## Channel Configuration

All channels are embedded in `index.html` for simplicity. To add/modify channels, locate the `CHANNELS` array in the JavaScript section:

```javascript
const CHANNELS = [
    {
        name: "Channel Name",
        logo: "https://example.com/logo.png",
        url: "https://example.com/stream.m3u8",
        category: "pakistan|india|global",
        type: "news|entertainment|sports"
    },
    // Add more channels...
];
```

### Supported Stream Formats

- **HLS (.m3u8)**: Recommended for best compatibility
- **MP4**: Direct video files
- **Other formats**: May work depending on browser support

## Low Bandwidth Optimization

The app includes several optimizations for slow connections:

1. **Adaptive Bitrate**: Automatically adjusts quality based on connection
2. **Reduced Buffer Size**: Minimizes initial loading time
3. **Auto-Detection**: Detects 2G/3G and enables low bandwidth mode
4. **Efficient Retry Logic**: Smart reconnection without excessive data usage

### Enabling Low Bandwidth Mode

- **Automatic**: App detects 2G/3G connections and enables automatically
- **Manual**: Toggle the "Low Bandwidth Mode" switch in the header
- **Effect**: Reduces buffer size, selects lower quality streams, optimizes for data saving

## Browser Compatibility

| Browser | Desktop | Mobile | HLS Support |
|---------|---------|--------|-------------|
| Chrome  | ✅      | ✅     | Via HLS.js  |
| Firefox | ✅      | ✅     | Via HLS.js  |
| Safari  | ✅      | ✅     | Native      |
| Edge    | ✅      | ✅     | Via HLS.js  |
| Opera   | ✅      | ✅     | Via HLS.js  |

## Network Requirements

- **Minimum**: 2G connection (128 kbps)
- **Recommended**: 3G or higher (1 Mbps+)
- **Optimal**: 4G/WiFi (5 Mbps+)

## Legal Disclaimer

⚠️ **IMPORTANT**: This application provides access to publicly available free-to-air (FTA) streams only. 

- We do **NOT** host, store, or distribute any content
- All streams are sourced from publicly available URLs
- Users are responsible for verifying the legality of content in their region
- Some streams may be geo-restricted or require permissions
- This project is for **educational purposes only**

Always respect copyright laws and content licensing in your country.

## Troubleshooting

### Stream Won't Play

1. **Check Connection**: Ensure you have active internet
2. **Try Another Channel**: Some streams may be temporarily offline
3. **Enable Low Bandwidth Mode**: If on slow connection
4. **Check Browser Console**: Look for specific error messages
5. **Try Different Browser**: Some streams work better on certain browsers

### Buffering Issues

1. **Enable Low Bandwidth Mode**: Reduces quality for smoother playback
2. **Close Other Apps**: Free up bandwidth
3. **Move Closer to Router**: Improve WiFi signal
4. **Try Different Time**: Some streams have peak hours

### Channel Not Loading

- Stream may be offline or geo-blocked
- Try using a VPN if stream is region-restricted
- Report broken streams by opening an issue

## Adding Custom Channels

To add your own channels:

1. Open `index.html` in a text editor
2. Find the `CHANNELS` array (around line 600)
3. Add a new channel object:

```javascript
{
    name: "My Channel",
    logo: "https://example.com/logo.png",
    url: "https://example.com/stream.m3u8",
    category: "pakistan",  // or "india", "global"
    type: "news"           // or "entertainment", "sports"
}
```

4. Save and refresh the browser

## Performance Tips

1. **Close Unused Tabs**: Free up memory
2. **Use WiFi When Possible**: More stable than mobile data
3. **Clear Browser Cache**: If experiencing issues
4. **Update Browser**: Use latest version for best performance
5. **Disable Extensions**: Some may interfere with playback

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/NewFeature`)
3. Commit changes (`git commit -m 'Add NewFeature'`)
4. Push to branch (`git push origin feature/NewFeature`)
5. Open a Pull Request

### What to Contribute

- 🎯 New working channel streams
- 🐛 Bug fixes
- 🎨 UI/UX improvements
- 📱 Mobile optimizations
- 🌍 Translation/localization
- 📝 Documentation improvements

## Known Issues

- Some streams may be geo-restricted
- Certain channels may go offline without notice
- Safari on iOS may have autoplay restrictions
- Very slow 2G connections may struggle with HLS streams

## Future Enhancements

- [ ] Favorites/bookmarking system
- [ ] EPG (Electronic Program Guide) integration
- [ ] Chromecast support
- [ ] Multiple language subtitles
- [ ] Picture-in-Picture mode
- [ ] Offline channel list caching
- [ ] User-submitted channel database

## License

This project is licensed under the MIT License - see below:

```
MIT License

Copyright (c) 2026 Global Free IPTV

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/iptv-app/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/iptv-app/discussions)

## Acknowledgments

- [Video.js](https://videojs.com/) - HTML5 video player
- [HLS.js](https://github.com/video-dev/hls.js/) - HLS streaming library
- [Font Awesome](https://fontawesome.com/) - Icon library
- [IPTV-org](https://github.com/iptv-org/iptv) - Community channel sources

## Privacy

This application:
- ✅ Does NOT collect any user data
- ✅ Does NOT use cookies
- ✅ Does NOT track users
- ✅ Works completely client-side
- ✅ No analytics or third-party tracking

Your privacy is completely protected.

---

**Made with ❤️ for cord-cutters worldwide**

Optimized for 2G/3G • No Ads • Open Source • Privacy First
