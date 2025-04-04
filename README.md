# EduEasy - South African Educational App

EduEasy is a mobile application designed to simplify access to tertiary education in South Africa. It supports offline use, local language accessibility, POPIA compliance, and integrates with national systems like NSFAS and university portals.

## 🛠 Local Development Setup

1. **Requirements**:
   - Flutter SDK (3.x)
   - Dart SDK
   - Android Studio / Xcode / VS Code
   - Firebase CLI (optional for emulator support)

2. **Installation**:
   ```bash
   git clone https://github.com/you/edueasy.git
   cd edueasy
   flutter pub get
   ```

3. **Running the App**:
   ```bash
   flutter run
   ```

4. **Flutter Commands**:
   - Format code: `flutter format .`
   - Analyze code: `flutter analyze`
   - Run tests: `flutter test`

## 🧪 Testing Guidelines

- Unit tests for domain layer logic
- Widget tests for UI rendering
- Integration tests for feature flows
- Simulated offline environments using Android Emulator or iOS Simulators

## 🤝 Contributing

1. Fork the repo
2. Create your feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add my feature'`
4. Push to the branch: `git push origin feature/my-feature`
5. Open a Pull Request 🚀

## 📁 Project Structure

- `lib/features/` - Feature-first architecture
- `lib/packages/` - Reusable core components and services
- `lib/main.dart` - App entry point
- `assets/` - Ndebele patterns, icons, and illustrations
- `l10n/` - Localization assets

## 🌍 Localization

Supports English (`intl_en.arb`) and Zulu (`intl_zu.arb`). Easily extendable to isiXhosa and others.

## 🔐 POPIA & Security

- All user data encrypted with Flutter Secure Storage
- Consent-driven analytics and feedback
- Offline token persistence and expiration warnings

## 🔌 Integration Map

- NSFAS API (funding)
- University Portals (applications)
- Africa's Talking SMS Gateway
- South African ID Verification (if permitted)

## 🧭 System Flow Diagram

```plaintext
[User Interface]
    ↓
[Presentation Layer]
    ↓
[Use Cases / Domain Logic]
    ↓
[Repositories / Data Layer]
    ↓
[Local (Hive, Secure Storage) | Remote APIs (NSFAS, SMS, Identity)]
```

## 🗺️ Feature Roadmap

```plaintext
[✓] University Application Form
[✓] Funding Integration (NSFAS, Bursaries, Scholarships)
[✓] Thandi AI Mentorship
[✓] Full Offline Support
[✓] Feedback and Voice Input
[ ] Live Chat Integration
[ ] Web Companion App
```

## 🔍 Critical Development Requirements

- ✅ Robust Error Handling (offline aware, bilingual)
- ✅ Complete Form Validation with cultural context
- ✅ Comprehensive Loading States and UX
- ✅ CI/CD pipeline for Android & iOS, with POPIA checks
- ✅ Strong Security & Authentication architecture
- ✅ Accessibility (screen readers, voice input, high contrast)
- ✅ Privacy-respecting, opt-in Analytics

## 🧱 Architecture Diagram

```plaintext
                    +------------------+
                    |     UI Layer     |
                    +------------------+
                             ↓
                    +------------------+
                    | Presentation     |  <Widgets, Screens>
                    +------------------+
                             ↓
                    +------------------+
                    | Domain Layer     |  <Use Cases, Entities>
                    +------------------+
                             ↓
                    +------------------+
                    | Data Layer       |  <Repositories, Models>
                    +------------------+
                         ↓        ↓
              +----------------+  +----------------------+
              |   Local Cache  |  |  Remote APIs (HTTPS) |
              |  (Hive, Secure)|  |   NSFAS, SMS, ID     |
              +----------------+  +----------------------+
```

## 📬 Contact

For questions, suggestions, or collaboration:
- 📧 hello@edueasy.co.za
- 🌐 https://www.edueasy.co.za

> EduEasy is built for the future of accessible, equitable, and digitally inclusive education in South Africa.