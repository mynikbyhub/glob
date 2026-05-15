# Contributing to Global Free IPTV

Thank you for your interest in contributing! This document provides guidelines for contributing to the project.

## 🎯 How Can You Contribute?

### 1. **Add New Channels** ⭐ Most Needed!
- Find working free-to-air (FTA) streams
- Test them thoroughly
- Submit via Pull Request

### 2. **Report Broken Streams**
- Open an issue with channel name
- Specify error/problem
- Test date/time

### 3. **Improve Code**
- Bug fixes
- Performance optimizations
- New features
- Better error handling

### 4. **Enhance Documentation**
- Fix typos
- Add examples
- Translate to other languages
- Improve clarity

### 5. **Test & Report Issues**
- Test on different devices
- Report bugs with details
- Suggest improvements

---

## 📝 Contribution Guidelines

### Adding New Channels

**Requirements:**
- ✅ Must be **free-to-air** (FTA) streams
- ✅ Must be **publicly accessible** (no authentication)
- ✅ Must be **legal** in at least one jurisdiction
- ✅ Should be **stable** (not going offline frequently)
- ✅ Preferably **HLS (.m3u8)** format for compatibility

**How to Add:**

1. **Edit `index.html`**
   
   Find the `CHANNELS` array (around line 600) and add:

   ```javascript
   {
       name: "Channel Name",
       logo: "https://example.com/logo.png",  // Use Wikipedia or official logos
       url: "https://example.com/stream.m3u8", // Must be working URL
       category: "pakistan|india|global",      // Pick one
       type: "news|entertainment|sports"       // Pick one
   }
   ```

2. **Test the Channel**
   - Open index.html locally
   - Try playing the channel
   - Confirm it works on mobile
   - Check on 3G/4G connection

3. **Update `channels.json`** (Optional)
   
   Add the same channel with additional metadata:

   ```json
   {
       "id": 21,
       "name": "Channel Name",
       "logo": "https://example.com/logo.png",
       "url": "https://example.com/stream.m3u8",
       "category": "pakistan",
       "type": "news",
       "language": "urdu",
       "country": "PK"
   }
   ```

4. **Submit Pull Request**
   - Clear description
   - Mention tested devices
   - Note any limitations (geo-blocking, etc.)

---

### Code Contributions

**Before You Start:**
1. Check existing issues/PRs to avoid duplicates
2. Open an issue to discuss major changes
3. Follow existing code style

**Code Style:**
- Use consistent indentation (2 spaces)
- Add comments for complex logic
- Keep functions small and focused
- Use meaningful variable names
- Test on mobile devices

**Example Good Commit:**
```
Add retry logic for network failures

- Implements exponential backoff
- Max 5 retry attempts
- Shows user-friendly error messages
- Tested on 2G/3G connections
```

**Example Bad Commit:**
```
fixed stuff
```

---

## 🔧 Development Setup

### Prerequisites
None! Just a text editor and web browser.

### Recommended Tools
- **Editor**: VS Code, Sublime Text, or any code editor
- **Browser**: Chrome/Firefox with DevTools
- **Testing**: Chrome DevTools Network Throttling

### Testing Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/global-free-iptv.git
   cd global-free-iptv
   ```

2. **Open in Browser**
   ```bash
   # Just open index.html, or use a local server:
   python3 -m http.server 8000
   # Visit http://localhost:8000
   ```

3. **Test Changes**
   - Desktop (Chrome, Firefox, Safari)
   - Mobile (iOS Safari, Chrome Android)
   - Slow connection (DevTools throttling)
   - Different screen sizes

---

## 🐛 Reporting Bugs

### Before Reporting
- [ ] Check existing issues
- [ ] Test on latest version
- [ ] Try different browser
- [ ] Clear cache and retry

### Bug Report Template

```markdown
**Channel/Feature:** [Name of channel or feature]

**Description:** 
Clear description of the bug

**Steps to Reproduce:**
1. Go to '...'
2. Click on '...'
3. See error

**Expected Behavior:**
What should happen

**Actual Behavior:**
What actually happens

**Screenshots:**
If applicable

**Environment:**
- Device: [e.g., iPhone 12, Samsung Galaxy S21]
- OS: [e.g., iOS 15, Android 12]
- Browser: [e.g., Safari, Chrome]
- Connection: [e.g., WiFi, 4G, 3G]

**Additional Context:**
Any other relevant information
```

---

## 💡 Feature Requests

We love new ideas! Before suggesting:

1. **Check existing issues** - Maybe it's already planned
2. **Describe the use case** - Why is this needed?
3. **Consider scope** - Should fit the project's goal
4. **Think about implementation** - How would it work?

### Feature Request Template

```markdown
**Feature Name:** [Brief title]

**Problem it Solves:**
What user problem does this address?

**Proposed Solution:**
How should it work?

**Alternatives Considered:**
Other approaches you've thought about

**Additional Context:**
Mockups, examples, references
```

---

## 🔍 Stream Source Guidelines

### Where to Find Streams

**Legitimate Sources:**
- Official broadcaster websites (look for embed codes)
- IPTV-org GitHub repository
- Free IPTV community lists
- Broadcaster's official apps (extract stream URLs)

**Avoid:**
- Pirated streams
- Paid services streams
- Restreamed copyrighted content
- Unstable/temporary streams

### Testing Stream Quality

Before submitting, verify:

1. **Stability**: Works for at least 30 minutes
2. **Format**: HLS (.m3u8) preferred
3. **Resolution**: At least 480p
4. **Accessibility**: No geo-blocking (or document restrictions)
5. **Legality**: Confirm it's FTA/public

### Stream URL Best Practices

```javascript
// ✅ GOOD - Direct stream URL
"url": "https://cdn.broadcaster.com/live/stream.m3u8"

// ❌ BAD - Requires authentication
"url": "https://paid-service.com/premium/stream.m3u8"

// ❌ BAD - Temporary/dynamic URL
"url": "https://temp.com/stream?token=xyz&expires=123456"

// ✅ ACCEPTABLE - Well-known free service
"url": "https://reliable-cdn.com/public/channel.m3u8"
```

---

## 📋 Pull Request Process

### Before Submitting

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/channel-name
   # or
   git checkout -b fix/bug-description
   ```

3. **Make your changes**
   - Test thoroughly
   - Follow code style
   - Update documentation if needed

4. **Commit with clear message**
   ```bash
   git add .
   git commit -m "Add [Channel Name] to [Category]"
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/channel-name
   ```

### PR Template

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] New channel(s)
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement

## Channels Added (if applicable)
- Channel Name 1 - [Category] - Tested on [devices]
- Channel Name 2 - [Category] - Tested on [devices]

## Testing Done
- [ ] Tested on desktop
- [ ] Tested on mobile
- [ ] Tested on slow connection
- [ ] Verified no console errors
- [ ] Channel plays for 5+ minutes

## Screenshots (if applicable)
Add screenshots showing the changes

## Checklist
- [ ] Code follows project style
- [ ] Added necessary comments
- [ ] Updated documentation
- [ ] All tests pass
- [ ] No breaking changes
```

### Review Process

1. Maintainer reviews within 48 hours
2. May request changes or tests
3. Once approved, will be merged
4. Your contribution will be credited!

---

## 🏆 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes
- Project documentation

Top contributors may be invited as maintainers!

---

## 📜 Legal Considerations

### Stream Legality

By contributing streams, you confirm:

1. Stream is publicly accessible
2. No authentication required
3. You have verified it's free-to-air
4. No copyright infringement to your knowledge
5. Appropriate disclaimer is in place

**When in doubt**: Ask first, add later.

### Code License

All contributions will be under MIT License. By contributing:
- You agree to license your work under MIT
- You have rights to the code you're contributing
- You're not violating any agreements

---

## ❓ Questions?

- **General Questions**: Open a GitHub Discussion
- **Bugs**: Open an Issue
- **Security**: Email maintainer (don't post publicly)
- **Features**: Open an Issue with "Feature Request" label

---

## 🎨 UI/UX Contributions

Love design? Help us with:

- Better mobile layouts
- Color scheme improvements
- Accessibility enhancements
- Icon/logo design
- User flow optimization

Submit mockups or suggestions via GitHub Issues.

---

## 🌍 Internationalization

Want the app in your language?

1. Create a language file (e.g., `lang-fr.js`)
2. Translate UI strings
3. Submit PR with translation
4. Help us make IPTV accessible globally!

---

## 📊 Performance Contributions

Help optimize for low-bandwidth:

- Reduce initial load time
- Better caching strategies
- Optimize HLS.js configuration
- Improve retry logic
- Better error handling

---

## 🤝 Code of Conduct

### Our Pledge

We pledge to make participation harassment-free for everyone, regardless of:
- Age, body size, disability
- Ethnicity, gender identity
- Experience level
- Nationality, personal appearance
- Race, religion, sexual orientation

### Expected Behavior

- Be respectful and inclusive
- Accept constructive criticism
- Focus on what's best for the community
- Show empathy

### Unacceptable Behavior

- Harassment, trolling, insults
- Political/religious arguments
- Publishing others' private info
- Spamming or advertising
- Other unprofessional conduct

### Enforcement

Violations may result in:
1. Warning
2. Temporary ban
3. Permanent ban

Report to: [project maintainer contact]

---

## 🎯 Contribution Ideas

Not sure where to start? Try:

### Easy (Good First Issues)
- [ ] Fix typos in documentation
- [ ] Add channel logos
- [ ] Test and report broken streams
- [ ] Update README with FAQs

### Medium
- [ ] Add 10+ new working channels
- [ ] Improve mobile UI
- [ ] Add dark/light theme toggle
- [ ] Optimize loading spinner

### Advanced
- [ ] Implement favorites system
- [ ] Add Chromecast support
- [ ] Create EPG integration
- [ ] Build channel recommendation system
- [ ] Add offline mode

---

## 📞 Contact

- **Issues**: GitHub Issues
- **Discussions**: GitHub Discussions
- **Email**: [Your contact if comfortable sharing]

---

**Thank you for contributing to Global Free IPTV! 🎉**

Together we're making free television accessible to everyone, everywhere.
