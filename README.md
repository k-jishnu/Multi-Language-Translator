# Multi-Language Translator

A simple, elegant web-based language translator that supports multiple languages using the MyMemory Translation API. This application provides instant translations with a user-friendly interface.

## 🌟 Features

- **Real-time Translation**: Instant translation between multiple language pairs
- **Clean & Responsive UI**: Modern design that works on all devices
- **Bidirectional Translation**: Easily swap source and target languages
- **Copy to Clipboard**: Quick copy functionality for translated text
- **Text-to-Speech**: Listen to translations (browser-dependent)
- **Character Counter**: Track input text length
- **No Authentication Required**: Free API with no sign-up needed

## 🌍 Supported Languages

The application supports translation between the following languages:

- **Arabic** (ar-SA)
- **Chinese** (zh-CN)
- **Czech** (cs-CZ)
- **Danish** (da-DK)
- **Dutch** (nl-NL)
- **English** (en-GB)
- **Finnish** (fi-FI)
- **French** (fr-FR)
- **German** (de-DE)
- **Greek** (el-GR)
- **Hindi** (hi-IN)
- **Hungarian** (hu-HU)
- **Indonesian** (id-ID)
- **Italian** (it-IT)
- **Japanese** (ja-JP)
- **Korean** (ko-KR)
- **Norwegian** (no-NO)
- **Polish** (pl-PL)
- **Portuguese** (pt-PT)
- **Romanian** (ro-RO)
- **Russian** (ru-RU)
- **Slovak** (sk-SK)
- **Spanish** (es-ES)
- **Swedish** (sv-SE)
- **Thai** (th-TH)
- **Turkish** (tr-TR)
- **Ukrainian** (uk-UA)

## 📋 Prerequisites

To run this application, you only need:

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for API calls)

## 🚀 Installation

### Option 1: Direct Download

1. Download or clone this repository:
   ```bash
   git clone https://github.com/k-jishnu/Multi-Language-Translator.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Multi-Language-Translator
   ```

3. Open `index.html` in your web browser:
   - Double-click the `index.html` file, or
   - Right-click and select "Open with" your preferred browser

### Option 2: Live Server (Recommended for Development)

1. If using VS Code, install the "Live Server" extension
2. Right-click on `index.html` and select "Open with Live Server"
3. The application will open automatically in your default browser

## 💻 Usage

1. **Enter Text**: Type or paste the text you want to translate in the left textarea
2. **Select Languages**: 
   - Choose the source language from the left dropdown
   - Choose the target language from the right dropdown
3. **Translate**: Click the "Translate Text" button
4. **View Results**: The translation appears in the right textarea
5. **Additional Actions**:
   - Click the exchange icon (🔄) to swap languages
   - Click the speaker icon (🔊) to hear the text read aloud
   - Click the copy icon (📋) to copy text to clipboard

## 🔑 API Information

This application uses the **MyMemory Translation API**:

- **API Endpoint**: `https://api.mymemory.translated.net/get`
- **Authentication**: None required (free tier)
- **Rate Limits**: 
  - Free usage: 1,000 words/day per IP
  - For higher limits, consider registering for an API key at [MyMemory](https://mymemory.translated.net/doc/)
- **API Key Setup** (Optional):
  - If you obtain an API key, add it to the fetch URL in the script:
    ```javascript
    const apiUrl = `https://api.mymemory.translated.net/get?q=${text}&langpair=${translateFrom}|${translateTo}&key=YOUR_API_KEY`;
    ```

## 📖 Example Translation

**Input (English)**: 
```
Hello, how are you today?
```

**Output (Spanish)**:
```
Hola, ¿cómo estás hoy?
```

**Output (French)**:
```
Bonjour, comment allez-vous aujourd'hui?
```

**Output (Hindi)**:
```
नमस्ते, आज आप कैसे हैं?
```

## 📁 File Structure

```
Multi-Language-Translator/
│
├── index.html          # Main application file (HTML, CSS, and JavaScript)
└── README.md           # Project documentation (this file)
```

### Code Structure Overview

The `index.html` file contains:

- **HTML**: Semantic structure with form controls, textareas, and buttons
- **CSS**: 
  - Responsive design with flexbox layout
  - Custom styling for dropdowns, buttons, and textareas
  - Icon integration using Font Awesome and Material Icons
  - Mobile-friendly media queries
- **JavaScript**:
  - Dynamic country list population
  - Translation API integration
  - Text-to-speech functionality
  - Copy-to-clipboard feature
  - Language swap functionality

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the Repository**
   ```bash
   git clone https://github.com/k-jishnu/Multi-Language-Translator.git
   ```

2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/YourFeatureName
   ```

3. **Make Your Changes**
   - Add new features
   - Fix bugs
   - Improve documentation
   - Enhance UI/UX

4. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "Add: Brief description of your changes"
   ```

5. **Push to Your Fork**
   ```bash
   git push origin feature/YourFeatureName
   ```

6. **Submit a Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Describe your changes in detail

### Contribution Ideas

- Add more language pairs
- Implement translation history
- Add language auto-detection
- Improve error handling
- Add dark mode toggle
- Create offline fallback functionality
- Add pronunciation guides
- Implement keyboard shortcuts

## 🐛 Known Issues & Limitations

- Translation quality depends on the MyMemory API
- Text-to-speech availability varies by browser and language
- Free API tier has daily word limits
- Very long texts may not translate completely

## 🔮 Future Enhancements

- [ ] Add translation history with local storage
- [ ] Implement language auto-detection
- [ ] Add dark/light theme toggle
- [ ] Create PWA (Progressive Web App) version
- [ ] Add favorite language pairs
- [ ] Implement offline mode with cached translations
- [ ] Add pronunciation and transliteration
- [ ] Support for document translation
- [ ] Multi-API support for better accuracy

## 📄 License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2025 k-jishnu

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👤 Author

**k-jishnu**

- GitHub: [@k-jishnu](https://github.com/k-jishnu)
- Project Link: [Multi-Language-Translator](https://github.com/k-jishnu/Multi-Language-Translator)

## 🙏 Acknowledgments

- [MyMemory Translation API](https://mymemory.translated.net/) for providing free translation services
- [Font Awesome](https://fontawesome.com/) for icons
- [Google Fonts](https://fonts.google.com/) for typography
- All contributors who help improve this project

---

**Made with ❤️ by k-jishnu**

*If you find this project helpful, please consider giving it a ⭐ on GitHub!*
