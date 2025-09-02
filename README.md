# Pickle-Ricks-Pixel-Trick
just a simple stenography tool....

A browser-based steganography tool that hides and reveals secret messages within ordinary images. No software installation required - just pure HTML/CSS/JavaScript magic.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-GitHub_Pages-success?style=for-the-badge)](https://yourusername.github.io/steg-and-tell)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![No Dependencies](https://img.shields.io/badge/Dependencies-None-brightgreen?style=for-the-badge)](https://github.com/yourusername/steg-and-tell)

## ✨ Features

- 🖼️ **Hide Messages in Images** - Embed secret text into any image file
- 🔍 **Reveal Hidden Messages** - Extract messages from encoded images  
- 🌐 **Browser-Based** - No downloads or installations required
- 📱 **Mobile Friendly** - Works on phones, tablets, and desktops
- 🔒 **Client-Side Only** - All processing happens in your browser (nothing uploaded to servers)
- 🎨 **Clean Interface** - Simple, intuitive design anyone can use
- 📥 **Download Support** - Save your encoded images as PNG files
- ⚡ **Lightning Fast** - Vanilla JavaScript for maximum performance

## 🎬 Demo

**Before (Original Image):**
![Original Image](demo/original.jpg)

**After (Contains Hidden Message):**  
![Encoded Image](demo/encoded.png)
*Looks identical, but contains the message: "This is a secret message!"*

## 🚀 Quick Start

### Option 1: Use the Live Version
Visit **[yourusername.github.io/steg-and-tell](https://yourusername.github.io/steg-and-tell)** and start hiding messages immediately!

### Option 2: Deploy Your Own

1. **Fork this repository**
2. **Enable GitHub Pages** in repository Settings → Pages
3. **Visit your URL**: `https://yourusername.github.io/steg-and-tell`

## 📖 Usage Guide

### 🔐 Hiding Messages

1. Click **"Hide Message"** mode
2. Upload your cover image (PNG recommended)
3. Type your secret message
4. Click **"Hide Message in Image"**  
5. Download the encoded image
6. Share the image - it looks identical but contains your hidden message!

### 🔍 Revealing Messages  

1. Click **"Decode Message"** mode (default)
2. Upload an image that contains a hidden message
3. Click **"Reveal Hidden Message"**
4. The secret message appears below!

## ⚠️ Important Notes

- **File Format Matters**: Always save/share encoded images as **PNG files**
- **No Screenshots**: Screenshots destroy hidden data - use original files only
- **Compression Kills**: Avoid platforms that compress images (social media, messaging apps)
- **Size Limits**: Longer messages require larger images

## 🔧 Technical Details

### How It Works
This tool uses **LSB (Least Significant Bit) steganography**:

1. **Encoding**: Converts your message to binary, then modifies the least significant bit of each pixel's color values
2. **Decoding**: Reads the least significant bits to reconstruct the binary message, then converts back to text
3. **End Delimiter**: Uses `1111111111111110` to mark message boundaries

### Browser Compatibility
- ✅ Chrome/Chromium 80+
- ✅ Firefox 75+  
- ✅ Safari 13+
- ✅ Edge 80+

### File Size Requirements
- **Text**: Each character needs ~8 pixels
- **Example**: 100-character message needs ~800 pixels minimum
- **Recommendation**: Use images with at least 10x more pixels than message characters

## 📁 Project Structure

```
steg-and-tell/
├── index.html          # Main application file
├── README.md           # This file
├── demo/              # Demo images
│   ├── original.jpg   # Example original image
│   └── encoded.png    # Example with hidden message
└── LICENSE            # MIT License
```

## 🛡️ Security & Privacy

- **Client-Side Only**: No data ever leaves your browser
- **No Tracking**: Zero analytics, cookies, or external requests  
- **Open Source**: All code is visible and auditable
- **No Dependencies**: No third-party libraries or CDNs

## 🎯 Use Cases

- **Digital Dead Drops**: Covert communication channels
- **Copyright Protection**: Invisible watermarking
- **Education**: Learn about steganography and digital forensics
- **Privacy**: Send sensitive information without detection
- **Fun Projects**: Digital treasure hunts and puzzles

## 🔬 Limitations

- **Compression Vulnerability**: JPEG compression destroys hidden data
- **Visual Changes**: Technically alters pixel values (usually imperceptible)
- **Size Constraints**: Large messages need large images  
- **Detection**: Advanced steganalysis tools can detect presence of hidden data
- **Not Encryption**: Hidden but not encrypted (consider combining with encryption)

## 🚀 Deployment Options

### GitHub Pages (Recommended)
1. Fork this repo
2. Settings → Pages → Source: "Deploy from branch" → main
3. Your site: `https://username.github.io/steg-and-tell`

### Netlify
1. Drag `index.html` to [netlify.com](https://netlify.com) deploy area
2. Get instant URL: `https://random-name.netlify.app`

### Vercel
1. Import this repo at [vercel.com](https://vercel.com)
2. Deploy automatically: `https://steg-and-tell.vercel.app`

### Local Testing
```bash
# Simple Python server
python -m http.server 8000

# Or Node.js
npx http-server
```

## 🤝 Contributing

Contributions welcome! Here's how:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Commit** your changes: `git commit -m 'Add amazing feature'`
4. **Push** to branch: `git push origin feature/amazing-feature`  
5. **Open** a Pull Request

### Ideas for Contributions
- [ ] Password protection for messages
- [ ] Different steganography algorithms  
- [ ] Batch processing multiple images
- [ ] Drag-and-drop file uploads
- [ ] Message encryption before hiding
- [ ] Support for other file formats
- [ ] Advanced options (bit planes, channels)

## 📚 Educational Resources

- [Steganography on Wikipedia](https://en.wikipedia.org/wiki/Steganography)
- [LSB Steganography Explained](https://www.geeksforgeeks.org/lsb-based-image-steganography-using-matlab/)
- [Digital Forensics and Steganalysis](https://resources.infosecinstitute.com/topics/digital-forensics/steganography-digital-forensics/)

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by classical steganography techniques
- Built with vanilla JavaScript for maximum compatibility
- Thanks to the open source community for making this possible

## 📧 Support

- 🐛 **Bug Reports**: Open an issue with detailed reproduction steps
- 💡 **Feature Requests**: Open an issue with your idea
- ❓ **Questions**: Check existing issues or open a new one
- 📖 **Documentation**: Suggest improvements to this README

---

**⭐ Star this repo if you find it useful!**

Made with ❤️ and a healthy dose of digital mischief.

*"The best place to hide a secret is in plain sight."* - Edgar Allan Poe (probably)
