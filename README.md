# 📰 News App

A modern Flutter news application that fetches real-time news headlines from around the world using the [NewsAPI](https://newsapi.org). Built with GetX state management, MVC architecture pattern, and clean code principles.

## ✨ Features

- 📰 **Real-time News Headlines** - Fetch top headlines from multiple countries
- 🏷️ **Category Filtering** - Browse news by categories (Business, Entertainment, Health, Science, Sports, Technology)
- 🔍 **News Details** - View full article information with images
- 🌍 **Multi-country Support** - Access news from different countries
- 🎨 **Modern UI** - Clean and intuitive user interface
- ⚡ **Fast Performance** - Optimized state management with GetX
- 🖼️ **Image Caching** - Cached network images for better performance
- 🔗 **External Links** - Open articles in external browser

## 🏗️ Architecture

This project follows **MVC (Model-View-Controller)** architecture pattern:

```
lib/
├── controllers/          # Business logic (GetX Controllers)
│   ├── home_controller.dart
│   └── detail_controller.dart
├── models/              # Data models
│   ├── article_model.dart
│   └── news_response_model.dart
├── views/               # UI screens
│   ├── home_view.dart
│   └── detail_view.dart
├── services/            # API calls and external services
│   └── news_api_service.dart
├── routes/              # Navigation configuration
│   ├── app_pages.dart
│   └── app_routes.dart
├── utils/               # Utility functions and constants
│   ├── app_colors.dart
│   └── date_formatter.dart
└── main.dart           # App entry point
```

## 🛠️ Technologies Used

- **Framework:** [Flutter](https://flutter.dev) (Dart 3.9.0+)
- **State Management:** [GetX](https://pub.dev/packages/get) 4.6.6
- **HTTP Client:** [http](https://pub.dev/packages/http) 0.13.5
- **Image Caching:** [cached_network_image](https://pub.dev/packages/cached_network_image) 3.3.1
- **Internationalization:** [intl](https://pub.dev/packages/intl) 0.20.2
- **URL Launcher:** [url_launcher](https://pub.dev/packages/url_launcher) 6.3.0
- **Provider:** [provider](https://pub.dev/packages/provider) 6.0.5

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [Flutter SDK](https://flutter.dev/docs/get-started/install) (3.9.0 or higher)
- [Dart SDK](https://dart.dev/get-dart) (3.9.0 or higher)
- [Android Studio](https://developer.android.com/studio) (for Android development)
- [Xcode](https://developer.apple.com/xcode/) (for iOS development)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/AhmdMaulidan/News.git
cd News
```

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Get NewsAPI Key

1. Visit [NewsAPI.org](https://newsapi.org)
2. Sign up for a free account
3. Get your API key
4. Update the API key in `lib/services/news_api_service.dart`:

```dart
static const String _apiKey = 'YOUR_API_KEY_HERE';
```

### 4. Run the Application

```bash
# Run on all connected devices/emulators
flutter run

# Run on specific device
flutter run -d <device_id>

# Run on Chrome (web)
flutter run -d chrome
```

## 📱 Supported Platforms

- ✅ **Android** (API level 21+)
- ✅ **iOS** (11.0+)
- ✅ **Web** (Chrome, Firefox, Safari)
- ✅ **macOS**
- ✅ **Windows**
- ✅ **Linux**

## 📚 API Configuration

### Available Categories

- `business` - Business news
- `entertainment` - Entertainment news
- `general` - General news
- `health` - Health news
- `science` - Science news
- `sports` - Sports news
- `technology` - Technology news

### Supported Countries

The app supports news from multiple countries. Common country codes:
- `us` - United States
- `gb` - United Kingdom
- `id` - Indonesia
- `in` - India
- `jp` - Japan
- `au` - Australia

See [NewsAPI documentation](https://newsapi.org/docs/endpoints/top-headlines) for complete country list.

## 🔧 Build & Release

### Build APK (Android)

```bash
# Debug APK
flutter build apk --debug

# Release APK
flutter build apk --release
```

### Build iOS App

```bash
# Debug IPA
flutter build ios --debug

# Release IPA
flutter build ios --release
```

### Build Web

```bash
flutter build web --release
```

## 📁 Project Structure Details

### Controllers (`lib/controllers/`)
- **HomeController** - Manages home screen logic, fetches news headlines
- **DetailController** - Handles article detail page functionality

### Models (`lib/models/`)
- **NewsResponseModel** - API response structure
- **ArticleModel** - Individual article data model

### Views (`lib/views/`)
- **HomeView** - Displays list of news articles
- **DetailView** - Shows detailed article information

### Services (`lib/services/`)
- **NewsApiService** - Handles all API calls to NewsAPI

### Utils (`lib/utils/`)
- **AppColors** - Color scheme constants
- **DateFormatter** - Date formatting utilities

## 🎨 Customization

### Change Theme Colors

Edit `lib/utils/app_colors.dart`:

```dart
class AppColors {
  static const Color accent = Color(0xFF1F2937);
  static const Color background = Color(0xFFF9FAFB);
  // ... other colors
}
```

### Modify API Request Parameters

Edit `lib/services/news_api_service.dart` to change default country or add more parameters.

## 🐛 Troubleshooting

### API Key Error
- Ensure your API key is valid and active
- Check NewsAPI quota limits at [newsapi.org dashboard](https://newsapi.org/account)

### Flutter Issues
```bash
# Clean build
flutter clean
flutter pub get
flutter run

# Update Flutter
flutter upgrade
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Ahmad Maulidan**
- GitHub: [@AhmdMaulidan](https://github.com/AhmdMaulidan)
- Email: ahmd.maulidanngmail.com

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

If you have any questions or need help, please open an [issue](https://github.com/AhmdMaulidan/News/issues) on GitHub.

## 🙏 Acknowledgments

- [NewsAPI](https://newsapi.org) - News data provider
- [GetX](https://pub.dev/packages/get) - State management
- [Flutter](https://flutter.dev) - UI framework

---

Made with ❤️ by [Ahmad Maulidan](https://github.com/AhmdMaulidan)
