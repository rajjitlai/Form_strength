# 🔐 Form Strength - Password Strength Validator

A modern, responsive registration form featuring real-time password strength validation with visual feedback.

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

- **🎨 Modern Design**: Beautiful gradient UI with glassmorphism effects
- **📱 Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **🔒 Real-time Password Validation**: Instant feedback on password strength
- **⚡ Fast & Lightweight**: No heavy frameworks, just vanilla JavaScript with jQuery
- **♿ Accessible**: ARIA labels and semantic HTML for better accessibility
- **🎯 5-Level Strength Indicator**: Very Weak, Weak, Mediocre, Strong, Very Strong
- **🌈 Smooth Animations**: Engaging hover effects and transitions

## 📸 Screenshots

### Desktop View
The form features a clean, centered layout with a purple gradient background and white form card.

### Password Strength Levels
- **Very Weak** (Red): Basic password
- **Weak** (Orange): Needs improvement
- **Mediocre** (Yellow): Getting better
- **Strong** (Light Green): Good password
- **Very Strong** (Green): Excellent password

## 🚀 Quick Start

### Option 1: Direct Download
1. Clone this repository or download the ZIP file
2. Open `index.html` in your web browser
3. Start testing the password strength validator!

### Option 2: Using Git
```bash
git clone https://github.com/rajjitlai/Form_strength.git
cd Form_strength
# Open index.html in your browser
```

## 📁 Project Structure

```
Form_strength/
├── assets/
│   └── images/
│       └── user.png           # User profile icon
├── css/
│   └── style.css              # All styling and responsive design
├── js/
│   └── password-strength.js   # Password strength calculator plugin
├── index.html                 # Main HTML file
├── README.md                  # This file
└── LICENSE                    # MIT License
```

## 🔧 How It Works

### Password Strength Calculation

The password strength is calculated based on several criteria:

- **Character Length**: +1 point per character
- **Spaces**: +1 point per space
- **Lowercase Letters**: +2 points
- **Uppercase Letters**: +2 points
- **Numbers**: +4 points
- **Special Symbols**: +5 points

**Total Score Breakdown:**
- 0-5 points: Very Weak (Red)
- 6-10 points: Weak (Orange)
- 11-15 points: Mediocre (Yellow)
- 16-20 points: Strong (Light Green)
- 21+ points: Very Strong (Green)

### Customization

#### Change Color Scheme
Edit the gradient colors in `css/style.css`:

```css
body {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

#### Adjust Scoring System
Modify the points system in `js/password-strength.js`:

```javascript
points: {
    forEachCharacter: 1,
    forEachSpace: 1,
    containsLowercaseLetter: 2,
    containsUppercaseLetter: 2,
    containsNumber: 4,
    containsSymbol: 5
}
```

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)

## 📦 Dependencies

- [jQuery 3.6.0](https://jquery.com/) - For DOM manipulation and plugin functionality
- [Font Awesome 4.7.0](https://fontawesome.com/v4.7.0/) - For icons

## 🎨 Design Features

### Responsive Breakpoints
- **Desktop**: Full-width form (max 550px)
- **Tablet** (< 768px): Adjusted padding and sizing
- **Mobile** (< 480px): Optimized for small screens

### Visual Effects
- Smooth hover animations on form and inputs
- Gradient backgrounds with backdrop blur
- Box shadows for depth
- Rounded corners for modern look
- Animated password strength indicator

## 🛠️ Development

### Prerequisites
- A modern web browser
- Text editor (VS Code, Sublime Text, etc.)
- Basic knowledge of HTML, CSS, and JavaScript

### Local Development
```bash
# No build process required! Just open the file
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```

## 📝 Usage Example

```html
<!-- Initialize password strength validator -->
<script>
  $(function () {
    $("#password").passwordStrength();
  });
</script>
```

### Custom Configuration
```javascript
$(function () {
  $("#password").passwordStrength({
    secureStrength: 30,  // Change threshold for "very strong"
    text: true,          // Show text indicator
    indicatorDisplayType: "block"  // Display style
  });
});
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Rajjit Laishram**
- GitHub: [@rajjitlai](https://github.com/rajjitlai)
- Year: 2026

## 🙏 Acknowledgments

- Password strength algorithm inspired by common security best practices
- Design inspired by modern web UI/UX trends
- Icons provided by Font Awesome
- jQuery for cross-browser compatibility

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Check existing issues for solutions
- Review the code documentation

## 🔮 Future Enhancements

- [ ] Add password confirmation field
- [ ] Implement form submission handling
- [ ] Add email validation feedback
- [ ] Dark/Light theme toggle
- [ ] Remove jQuery dependency (vanilla JS version)
- [ ] Add password visibility toggle
- [ ] Implement password generation feature
- [ ] Add input field animations
- [ ] Multi-language support

## 📊 Version History

### v2.0.0 (2026-02-17)
- ✨ Complete project reorganization
- 📱 Added responsive design
- 🎨 Modernized UI with gradients and animations
- ♿ Improved accessibility
- 📚 Comprehensive documentation
- 🗂️ Better folder structure

### v1.0.0 (Initial Release)
- Basic form with password strength validation
- Simple CSS styling
- jQuery-based password strength calculator

---

Made with ❤️ by Rajjit Laishram

⭐ If you found this helpful, please consider giving it a star!
