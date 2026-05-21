# ProductReach - Barcode Scanner Mobile App

A powerful mobile application that scans product barcodes and provides detailed information about ingredients, health benefits, potential side effects, and allergen warnings.

## 🎯 Features

### Core Functionality
- **Real-time Barcode Scanning** - Scan any product barcode using your device camera
- **Detailed Product Information** - Get instant access to product details and ingredients
- **Health Benefits Analysis** - AI-powered analysis of nutritional benefits
- **Side Effects Detection** - Identify potential health concerns
- **Allergen Warnings** - Critical alerts for common allergens
- **Scan History** - Track all scanned products with timestamps
- **Nutrition Facts** - Complete nutritional information per 100g

### Smart Analysis
The app intelligently analyzes products for:

**✅ Health Benefits:**
- High fiber content (digestive health)
- High protein (muscle building)
- Low calorie (weight management)
- Rich calcium (bone health)
- Iron content (oxygen transport)
- Vitamin C (immunity boost)
- Organic, vegan, gluten-free certifications

**⚠️ Side Effects & Warnings:**
- High sodium (blood pressure concerns)
- High sugar (blood glucose impact)
- Caffeine content (sleep disruption)
- Artificial additives
- High saturated fat (cholesterol risk)
- Trans fats (heart disease risk)
- HFCS (metabolic concerns)

**🚨 Allergen Detection:**
- Milk/Dairy
- Peanuts
- Tree nuts
- Fish/Shellfish
- Eggs
- Soy
- Wheat/Gluten
- Sesame

## 📱 Installation

### Prerequisites
- Node.js and npm
- React Native CLI
- Android Studio (for Android) or Xcode (for iOS)

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/lokeshsvskodavati-web/productreach.git
   cd productreach
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Install native dependencies:**
   ```bash
   # For Android
   npm install react-native-camera
   npm install react-native-permissions
   
   # For iOS (via CocoaPods)
   cd ios && pod install && cd ..
   ```

4. **Run the app:**
   ```bash
   # Android
   npm run android

   # iOS
   npm run ios
   ```

## 🏗️ Project Structure

```
productreach/
├── App.js                          # Main app and navigation
├── screens/
│   ├── ScannerScreen.js           # Camera and barcode scanning
│   ├── ResultsScreen.js           # Product analysis and details
│   └── HistoryScreen.js           # Scan history management
├── services/
│   ├── ProductAnalyzer.js         # Product analysis logic
│   └── permissions.js             # Permission handling
├── package.json                    # Dependencies
└── README.md                       # Documentation
```

## 🔄 How It Works

1. **Scan** - Point your camera at a product barcode
2. **Fetch** - App retrieves product data from Open Food Facts database
3. **Analyze** - ProductAnalyzer processes nutrition and ingredients
4. **Display** - View benefits, side effects, and allergen warnings
5. **Save** - Automatically saved to scan history
6. **Track** - Access history anytime from the History tab

## 📊 Data Source

The app uses the **Open Food Facts API** which contains:
- 1.5+ million products worldwide
- Comprehensive nutritional data
- Ingredient listings
- Product certifications

## 🔐 Permissions Required

- **Camera** - For barcode scanning
- **Storage** - For saving scan history locally

## 🚀 Technologies Used

- **React Native** - Cross-platform mobile framework
- **React Navigation** - Screen navigation and routing
- **React Native Camera** - Barcode scanning capability
- **AsyncStorage** - Local data persistence
- **Material Icons** - Professional UI components
- **Open Food Facts API** - Product database

## 📝 Usage

### Scanning
1. Open the Scanner tab
2. Position product barcode within the frame
3. App automatically captures and analyzes
4. Results display instantly

### Viewing History
1. Tap the History tab
2. View all previously scanned products
3. Delete individual items or clear all
4. Pull to refresh

### Understanding Results
- **Green checkmarks** - Health benefits detected
- **Orange warnings** - Potential side effects
- **Red alerts** - Critical allergen warnings

## 🛠️ Customization

### Modify Analysis Rules
Edit `services/ProductAnalyzer.js` to adjust:
- Benefit thresholds (e.g., "High Protein" > 10g)
- Side effect detection criteria
- Allergen detection keywords

### Adjust UI Theme
Colors are defined in `StyleSheet` objects in each screen file:
- Primary color: `#2196F3` (Blue)
- Success color: `#4CAF50` (Green)
- Warning color: `#FF9800` (Orange)
- Error color: `#FF6B6B` (Red)

## 🐛 Troubleshooting

### Camera Not Working
- Check permissions: Settings → App → Permissions → Camera
- Ensure lighting is adequate
- Try different barcode angles

### Product Not Found
- Product may not be in the database
- Check barcode is not damaged
- Try scanning a different product

### History Not Saving
- Check storage permissions
- Clear app cache and retry
- Ensure sufficient device storage

## 📄 License

MIT License - Feel free to use and modify

## 🤝 Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push and create a Pull Request

## 📞 Support

For issues or questions:
- Open a GitHub Issue
- Check existing documentation
- Review the code comments

## 🎓 Learning Resources

- [React Native Docs](https://reactnative.dev/)
- [React Navigation Guide](https://reactnavigation.org/)
- [Open Food Facts API](https://world.openfoodfacts.org/api)

---

**Built with ❤️ using React Native**

Happy scanning! 📱✨
