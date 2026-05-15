# ❓ Frequently Asked Questions (FAQ)

Quick answers to common questions about Global Free IPTV.

---

## 📺 General Questions

### Q: Is this really free?
**A:** Yes! 100% free, no hidden costs, no subscriptions, no ads, no premium features. Everything is completely free forever.

### Q: Do I need to create an account?
**A:** No! Just open the app and start watching. No registration, no login, no personal information required.

### Q: Is it legal?
**A:** Yes, the app itself is legal. It only links to publicly available free-to-air (FTA) streams. However, you should verify that accessing these streams is legal in your country. The app includes a legal disclaimer.

### Q: Can I use this on my phone?
**A:** Absolutely! The app is mobile-first and works great on smartphones and tablets (iOS, Android).

### Q: Does it work offline?
**A:** No, you need an internet connection to stream live TV. However, the app interface loads without internet once cached.

---

## 🔧 Technical Questions

### Q: What internet speed do I need?
**A:** 
- **Minimum**: 128 kbps (2G) with Low Bandwidth Mode
- **Recommended**: 1 Mbps (3G)
- **Optimal**: 5 Mbps+ (4G/WiFi)

The app automatically adjusts quality based on your connection.

### Q: Why won't channels play?
**A:** Common reasons:
1. **Stream offline**: Channel may be temporarily down
2. **Geo-blocked**: Some channels only work in certain countries
3. **Slow connection**: Enable Low Bandwidth Mode
4. **Browser issue**: Try a different browser or clear cache
5. **Autoplay blocked**: Click the play button manually

### Q: Which browsers are supported?
**A:** 
- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Opera
- ✅ Mobile browsers (Chrome, Safari)

### Q: Do I need to install anything?
**A:** No! Just open the `index.html` file in your web browser. No installation, no setup required.

### Q: Can I run it on a web server?
**A:** Yes! You can deploy it anywhere:
- GitHub Pages
- Netlify
- Vercel
- Your own web server

See [DEPLOYMENT.md](DEPLOYMENT.md) for guides.

---

## 📱 Mobile Questions

### Q: Why doesn't autoplay work on iPhone?
**A:** Safari on iOS blocks autoplay by default. Just tap the play button when you select a channel.

### Q: Can I use it on iPad/tablet?
**A:** Yes! The responsive design works perfectly on all tablet sizes.

### Q: How do I go fullscreen on mobile?
**A:** Tap the fullscreen button in the video player controls, or rotate your device to landscape mode.

### Q: Can I Chromecast from the app?
**A:** Not yet, but it's planned for a future update. For now, you can use browser-level casting.

### Q: Does it work with my mobile data?
**A:** Yes, but it will use data. Enable Low Bandwidth Mode to reduce data usage on mobile connections.

---

## 🌍 Content Questions

### Q: How many channels are available?
**A:** Currently 20 pre-configured channels from Pakistan, India, and around the world. You can add more!

### Q: Can I add my own channels?
**A:** Yes! See [CONTRIBUTING.md](CONTRIBUTING.md) for instructions on adding channels. It's easy to edit the channel list.

### Q: Why is my favorite channel missing?
**A:** We only include free-to-air public streams. If you know of a working FTA stream, please contribute it!

### Q: Do channels have subtitles?
**A:** Only if the original stream includes them. We don't add subtitles ourselves.

### Q: Can I watch movies/shows on demand?
**A:** No, this is for **live TV only**. It's not a video-on-demand service.

### Q: Why did a channel stop working?
**A:** Streams can go offline, change URLs, or become geo-restricted. Please report broken channels via GitHub Issues.

---

## ⚙️ Feature Questions

### Q: What is Low Bandwidth Mode?
**A:** A special mode that:
- Reduces stream quality
- Uses less data
- Buffers more aggressively
- Works better on 2G/3G

Enable it from the toggle in the top-right corner.

### Q: Can I save favorite channels?
**A:** Not yet, but it's planned for future updates. For now, just remember which category they're in!

### Q: Is there a TV guide (EPG)?
**A:** Not currently, but EPG integration is being considered for future versions.

### Q: Can I rewind live TV?
**A:** Some streams support this if they're configured with DVR, but most are live-only.

### Q: Can I record streams?
**A:** The app doesn't have recording functionality. Check your local laws about recording broadcasts.

---

## 🔐 Privacy & Security Questions

### Q: Do you track what I watch?
**A:** No! We don't track anything. No analytics, no cookies, no data collection whatsoever.

### Q: Is my data safe?
**A:** Yes! The app is 100% client-side. Nothing is sent to any server. Your viewing is completely private.

### Q: Do you sell user data?
**A:** We don't collect any data, so there's nothing to sell. Ever.

### Q: Is HTTPS required?
**A:** When deployed online, yes. Most free streams require HTTPS. All recommended deployment platforms provide free SSL.

### Q: Are there ads?
**A:** No ads in the app itself. Some streams may have ads from the broadcaster.

---

## 💻 Development Questions

### Q: Can I modify the code?
**A:** Yes! It's open-source under MIT License. Feel free to customize it for your needs.

### Q: How can I contribute?
**A:** See [CONTRIBUTING.md](CONTRIBUTING.md). We welcome:
- New channels
- Bug fixes
- Feature improvements
- Documentation updates

### Q: What technologies are used?
**A:** Pure HTML5, CSS3, and vanilla JavaScript. Libraries: Video.js, HLS.js, Font Awesome.

### Q: Why no React/Vue/Angular?
**A:** To keep it lightweight and fast, especially for low-bandwidth environments. No build process needed.

### Q: Can I use this in my own project?
**A:** Yes! MIT License allows commercial and personal use. Just keep the license notice.

---

## 🌐 Regional Questions

### Q: Will it work in my country?
**A:** The app works worldwide, but some streams may be geo-restricted. Try enabling a VPN if needed.

### Q: Can I watch Pakistani channels outside Pakistan?
**A:** Most should work, but some may be geo-restricted. This depends on the broadcaster.

### Q: Same question for Indian channels?
**A:** Same answer - most work globally, but verify based on your location.

### Q: Can you add channels from [my country]?
**A:** If you can find working FTA streams, please contribute them! See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 📊 Performance Questions

### Q: Why is buffering so much?
**A:** 
1. **Slow connection**: Enable Low Bandwidth Mode
2. **Weak signal**: Move closer to WiFi router
3. **Peak hours**: Try different time
4. **Many users**: Close other apps using internet

### Q: How much data does it use?
**A:** Varies by stream quality:
- Low quality: ~100-200 MB/hour
- Medium quality: ~300-500 MB/hour
- High quality: ~500-1000 MB/hour

Low Bandwidth Mode uses the least data.

### Q: Does it drain battery quickly?
**A:** Video streaming always uses battery. Tips to save power:
- Lower screen brightness
- Use WiFi instead of mobile data
- Close other apps
- The app automatically pauses when you switch apps

### Q: Can low-end phones run it?
**A:** Yes! We've optimized it for low-end devices. Enable Low Bandwidth Mode for best performance.

---

## 🆘 Troubleshooting

### Q: Black screen, no video?
**Try:**
1. Refresh page (F5)
2. Clear browser cache
3. Try different browser
4. Check internet connection
5. Try different channel

### Q: Sound but no picture?
**A:** This is rare. Try:
1. Refresh the page
2. Update your browser
3. Disable browser extensions
4. Check video driver updates

### Q: Error: "Stream cannot be loaded"?
**A:** The stream is likely offline or geo-blocked. Try:
1. Different channel
2. VPN (if geo-blocked)
3. Report the channel as broken

### Q: Controls not working?
**A:** 
1. Click on the video player to focus it
2. Refresh the page
3. Try different browser
4. Check browser console for errors

---

## 🚀 Deployment Questions

### Q: How do I deploy this?
**A:** See [DEPLOYMENT.md](DEPLOYMENT.md) for step-by-step guides for 7+ platforms.

### Q: What's the easiest hosting option?
**A:** Netlify Drop - just drag and drop your folder and get instant URL.

### Q: Can I use my own domain?
**A:** Yes! All deployment platforms support custom domains.

### Q: Is hosting free?
**A:** Yes! GitHub Pages, Netlify, Vercel, and Cloudflare Pages all have generous free tiers.

### Q: How do I update after deployment?
**A:** Just push your changes to GitHub, or re-upload to your hosting platform.

---

## 💡 Tips & Tricks

### Q: Any hidden features?
**A:** 
- Keyboard: Space to play/pause
- Click channel card multiple times to reload
- Right-click video for more options
- Network badge shows current mode

### Q: Best channels for news?
**A:** Al Jazeera, BBC News, NDTV 24x7 are popular and reliable.

### Q: Best for slow connections?
**A:** News channels generally have lower bitrates. Enable Low Bandwidth Mode.

### Q: How often are channels updated?
**A:** Community-driven. Report broken channels and contribute new ones!

---

## 📞 Support Questions

### Q: Where do I report bugs?
**A:** [GitHub Issues](https://github.com/yourusername/iptv-app/issues)

### Q: How do I request a feature?
**A:** Open a GitHub Issue with label "Feature Request"

### Q: Can I get help with deployment?
**A:** Yes! Check [DEPLOYMENT.md](DEPLOYMENT.md) or ask in GitHub Discussions

### Q: Who maintains this?
**A:** Open-source community. Contributors welcome!

### Q: Is there a Discord/Telegram group?
**A:** Currently using GitHub Discussions. Community chat may be added later.

---

## 🎯 Comparison Questions

### Q: How is this different from paid IPTV?
**A:** 
- ✅ Completely free
- ✅ No subscription
- ✅ Open-source
- ❌ Limited channels (FTA only)
- ❌ No premium content

### Q: Why not just use YouTube?
**A:** Some channels aren't on YouTube, and this provides a unified TV-like experience.

### Q: What about other IPTV apps?
**A:** Advantages:
- No installation required
- Works in browser
- Privacy-focused
- Optimized for low bandwidth
- Open-source

---

## 📖 Documentation Questions

### Q: Where's the full documentation?
**A:** See:
- [README.md](README.md) - Full documentation
- [QUICKSTART.md](QUICKSTART.md) - Quick start guide
- [DEPLOYMENT.md](DEPLOYMENT.md) - Deployment guides
- [CONTRIBUTING.md](CONTRIBUTING.md) - How to contribute

### Q: Is there a video tutorial?
**A:** Not yet, but contributions are welcome!

### Q: Can I translate the documentation?
**A:** Yes! Translations are welcomed. See [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 🔮 Future Plans

### Q: What's coming next?
**Planned:**
- Favorites system
- EPG integration
- More channels
- UI themes
- PWA support
- Chromecast

See [CHANGELOG.md](CHANGELOG.md) for the roadmap.

### Q: Can I vote on features?
**A:** Comment on GitHub Issues for features you want!

---

## ❓ Still Have Questions?

**Not answered here?**

1. 📖 Check [README.md](README.md)
2. 🔍 Search [GitHub Issues](https://github.com/yourusername/iptv-app/issues)
3. 💬 Ask in [GitHub Discussions](https://github.com/yourusername/iptv-app/discussions)
4. 🐛 Open a new [Issue](https://github.com/yourusername/iptv-app/issues/new)

---

**Happy Streaming! 📺**
