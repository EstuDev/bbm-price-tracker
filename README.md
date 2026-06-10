# BBM Price Tracker 2026

A modern, interactive dashboard to monitor and compare Indonesian fuel (BBM) price changes between January and June 2026.

## 🎯 Features

- **Animated Price Counter** - Smooth number animations when switching between periods
- **Period Comparison** - Compare prices between January 1, 2026 and June 10, 2026
- **All BBM Types** - Track 7 different fuel types:
  - **Subsidized**: Pertalite (RON 90), Solar Subsidi (CN 48)
  - **Non-Subsidized**: Pertamax (RON 92), Pertamax Green (RON 95), Pertamax Turbo (RON 98), Dexlite (CN 51), Pertamina DEX (CN 53)
- **Visual Indicators** - Color-coded cards and type badges for quick identification
- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Dark Mode UI** - Modern dark theme with Tailwind CSS

## 📊 Price Data

### Significant Price Changes (June 10, 2026)
- **Pertamax (RON 92)**: Rp12.300 → **Rp16.250/liter** ⬆️ +32%
- **Pertamax Green (RON 95)**: Rp12.900 → **Rp17.000/liter** ⬆️ +31%
- **Subsidized fuels**: Remained stable

All prices are referenced to Jakarta (DKI) and surrounding areas.

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Tailwind CSS framework with custom animations
- **JavaScript (Vanilla)** - No dependencies required
- **Google Fonts** - Plus Jakarta Sans typography

## 📁 File Structure

```
bbm-price-tracker/
├── index.html      # Main dashboard file
├── README.md       # Documentation
└── LICENSE         # MIT License
```

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/EstuDev/bbm-price-tracker.git
cd bbm-price-tracker
```

2. Open in browser:
```bash
# Simply open the index.html file
open index.html
# Or use a local server (recommended)
python -m http.server 8000
# Then visit http://localhost:8000
```

## 📱 Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Android)

## 🎨 Customization

### Modify Price Data
Edit the `bbmData` object in the `<script>` section:
```javascript
const bbmData = {
    jan: [
        { name: "Fuel Name", ron: "RON XX", type: "Subsidi/Non-Subsidi", price: XXXXX, color: "..." },
        // ... more items
    ],
    juni: [ /* ... */ ]
};
```

### Change Animation Duration
Modify the duration parameter in `animateValue()` function (in milliseconds):
```javascript
animateValue(targetId, startVal, endVal, 1000, index); // 1000ms = 1 second
```

### Update Colors
The color system uses Tailwind CSS classes. Each BBM type has a corresponding color scheme in the `color` property.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**EstuDev** - Web Developer

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 📝 Notes

- All price data is for reference and based on Jakarta rates
- Actual prices may vary by region
- Data current as of June 10, 2026
- For real-time prices, always check official Pertamina website

## 🔗 Related Links

- [PT Pertamina Official](https://www.pertamina.com)
- [Indonesia Fuel Price Updates](https://www.pertamina.com/en/products-and-services/fuel-retail)

---

Made with ❤️ and Tailwind CSS
