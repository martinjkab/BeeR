# BeeR - Beer Rating Application

BeeR is a sophisticated Flutter application designed for beer enthusiasts. It allows users to browse an extensive catalog of beers, view detailed information about ingredients and brewing specs, and rate their favorite brews. The application leverages the Punk API for data and integrates with Firebase for backend services.

## 📱 Features

- **Browse Beers**: Explore a comprehensive list of beers fetched dynamically from the Punk API.
- **Detailed Insights**: View in-depth information including ABV, IBU, description, and specific ingredients (Malt, Hops, Yeast).
- **Infinite Scrolling**: Seamlessly load more items as you scroll with `infinite_scroll_pagination`.
- **Localization**: Native support for multiple languages, currently English (`en`) and Hungarian (`hu`).
- **Robust Error Handling**: User-friendly error messages and network handling.
- **Modern UI**: Clean interface using `auto_size_text` for responsive typography and custom fonts (Poppins).

## 🛠 Tech Stack

- **Framework**: [Flutter](https://flutter.dev/)
- **Network**: [Dio](https://pub.dev/packages/dio) for robust HTTP requests.
- **Backend**:
  - [Firebase Core & Firestore](https://firebase.google.com/) for data persistence.
  - [Supabase](https://supabase.com/) (Integration ready).
- **State Management & Architecture**: Repository Pattern with separation of concerns.
- **Localization**: `flutter_localizations` & `intl`.
- **Assets**: SVG support via `flutter_svg`.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (Version >=2.18.4 <3.0.0)
- Dart SDK
- An IDE (VS Code or Android Studio)
- Google Services configuration files (required for Firebase to work):
  - `android/app/google-services.json`
  - `ios/Runner/GoogleService-Info.plist`

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/rating_app.git
    cd rating_app
    ```

2.  **Install dependencies:**

    ```bash
    flutter pub get
    ```

3.  **Run the application:**
    ```bash
    flutter run
    ```

## 📂 Project Structure

```
lib/
├── l10n/              # Localization files (arb)
├── beer_item.dart     # Widget for individual beer list items
├── beer_list.dart     # Beer List View implementation
├── beer_page.dart     # Detailed Beer View
├── logic.dart         # Data models and JSON serialization logic
├── repo.dart          # Data Repository
├── service.dart       # API Service (Punk API integration)
├── main.dart          # Entry point and app configuration
└── ...
```

## 🤝 Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
