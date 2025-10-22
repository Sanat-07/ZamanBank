# 🏦 Zaman Bank Super App

Ислам банкинг принциптеріне негізделген толыққанды мобильді банкинг қосымшасы.

## 📱 Жобаның сипаттамасы

Zaman Bank Super App - бұл Flutter фреймворкінде жасалған заманауи мобильді банкинг қосымшасы. Қосымша ислам банкингінің қағидаттарын сақтай отырып, пайдаланушыларға толыққанды банктік қызметтерді ұсынады.

### 🎯 Негізгі мүмкіндіктер

#### 💳 Банктік операциялар
- **Шоттарды басқару**: Барлық банктік шоттарды көру және басқару
- **Ақша аударымы**: Банк ішінде және басқа банктерге аударым жасау
- **Төлем тарихы**: Барлық транзакцияларды көру және іздеу
- **Шотты толықтыру**: Картаны немесе шотты толықтыру

#### 📊 Инвестициялар және брокерлік қызмет
- **Акциялар портфолиосы**: Өз инвестицияларыңызды басқару
- **Нарық талдауы**: Нақты уақыттағы акциялар бағамдары
- **Акция сатып алу/сату**: Тікелей қосымша арқылы
- **Брокерлік шот**: Инвестициялық шотты басқару

#### 🎯 Мақсаттар және жоспарлау
- **Қаржылық мақсаттар**: Жинақтау мақсаттарын қою
- **Прогресс tracking**: Мақсаттарға жету барысын бақылау
- **Ұсыныстар**: AI көмегімен жеке қаржылық кеңестер

#### 📈 Қаржылық талдау
- **Шығын талдауы**: Шығындарды категориялар бойынша көру
- **Кіріс-шығын есебі**: Толық қаржылық есеп
- **Диаграммалар**: Визуалды графиктер мен диаграммалар
- **AI кеңестері**: OpenAI көмегімен жеке қаржылық ұсыныстар

#### 💬 AI ассистент
- **Дауыстық басқару**: Микрофон арқылы командалар беру
- **Умный чат**: 24/7 жұмыс істейтін AI көмекші
- **Функционалды командалар**: "Ақша аудар", "Балансты көрсет" т.б.
- **Дауыстық жауап**: Text-to-Speech технологиясы

#### 👤 Профиль және баптаулар
- **Жеке деректер**: Профильді басқару
- **Қауіпсіздік**: PIN код, биометрия
- **Тілді таңдау**: Көптілділік қолдауы
- **Хабарландырулар**: Push хабарландырулар

## 🏗️ Архитектура

### Frontend (Flutter)
```
zaman_bank_super_app/
├── lib/
│   ├── constants/          # Константалар және баптаулар
│   │   └── app_constants.dart
│   ├── models/            # Деректер модельдері
│   │   ├── user.dart
│   │   └── goal.dart
│   ├── providers/         # State басқару (Provider)
│   │   ├── auth_provider.dart
│   │   └── chat_notification_provider.dart
│   ├── screens/           # UI экрандары
│   │   ├── splash_screen.dart
│   │   ├── login_screen.dart
│   │   ├── registration_screen.dart
│   │   ├── home_screen.dart
│   │   ├── transfer_screen.dart
│   │   ├── funds_transfer_screen.dart
│   │   ├── top_up_screen.dart
│   │   ├── transactions_screen.dart
│   │   ├── transaction_history_screen.dart
│   │   ├── chat_screen.dart
│   │   ├── support_screen.dart
│   │   ├── goals_screen.dart
│   │   ├── portfolio_screen.dart
│   │   ├── broker_account_screen.dart
│   │   ├── broker_portfolio_screen.dart
│   │   ├── stock_details_screen.dart
│   │   ├── financial_analysis_screen.dart
│   │   └── profile_screen.dart
│   ├── services/          # API қызметтері
│   │   ├── auth_service.dart
│   │   ├── balance_service.dart
│   │   ├── transaction_service.dart
│   │   ├── chat_service.dart
│   │   ├── goal_service.dart
│   │   └── voice_service.dart
│   ├── widgets/           # Қайта пайдаланылатын компоненттер
│   │   ├── account_card.dart
│   │   ├── action_button.dart
│   │   ├── bottom_navigation.dart
│   │   ├── broker_bottom_navigation.dart
│   │   ├── brokerage_button.dart
│   │   ├── category_selection_widget.dart
│   │   ├── finance_card.dart
│   │   ├── loading_widget.dart
│   │   ├── news_card.dart
│   │   ├── portfolio_card.dart
│   │   ├── promo_card.dart
│   │   ├── stock_holding_card.dart
│   │   ├── stock_search_bar.dart
│   │   ├── support_section.dart
│   │   ├── transaction_card.dart
│   │   └── voice_widgets.dart
│   ├── utils/             # Қосымша функциялар
│   │   ├── function_call_handler.dart
│   │   ├── navigation_utils.dart
│   │   └── page_transitions.dart
│   └── main.dart          # Қосымшаның кіру нүктесі
├── android/               # Android платформасы
├── ios/                   # iOS платформасы
├── web/                   # Web платформасы
└── pubspec.yaml          # Тәуелділіктер
```

### Backend (Spring Boot)
```
zaman_bank_api/
├── src/main/java/org/example/zaman_bank_api/
│   ├── config/           # Конфигурациялар
│   ├── controller/       # REST API контроллерлері
│   ├── dto/             # Data Transfer Objects
│   ├── entity/          # Дерекқор моделдері
│   ├── repository/      # Дерекқормен жұмыс
│   ├── service/         # Бизнес логика
│   └── ZamanBankApiApplication.java
└── src/main/resources/
    ├── application.properties
    └── db/migration/    # Дерекқор миграциялары
```

## 🚀 Қалай орнату керек

### Талаптар

#### Frontend үшін:
- **Flutter SDK**: >=3.0.0
- **Dart SDK**: >=3.0.0
- **Android Studio** немесе **VS Code** (Flutter плагинімен)
- **Xcode** (iOS үшін, тек macOS-та)

#### Backend үшін:
- **Java**: JDK 17+
- **Gradle**: 7.0+
- **PostgreSQL**: 14+ (немесе басқа SQL дерекқор)

### Орнату қадамдары

#### 1. Репозиторийді клондау

```bash
git clone https://github.com/Sanat-07/ZamanBank.git
cd ZamanBank
```

#### 2. Backend орнату

```bash
cd zaman_bank_api

# Тәуелділіктерді орнату және құрастыру
./gradlew build

# Қолданбаны іске қосу
./gradlew bootRun
```

Backend келесі портта іске қосылады: `http://localhost:8080`

**Дерекқорды баптау:**

`application.properties` файлында өз дерекқор параметрлеріңізді орнатыңыз:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/zaman_bank
spring.datasource.username=your_username
spring.datasource.password=your_password
```

#### 3. Frontend орнату

```bash
cd ../zaman_bank_super_app

# Тәуелділіктерді орнату
flutter pub get

# Қолданбаны іске қосу (OpenAI API ключсіз)
flutter run

# OpenAI мүмкіндіктерімен іске қосу
flutter run --dart-define=OPENAI_API_KEY=your_openai_api_key_here
```

### 🔑 OpenAI API орнату

Қосымша дауыстық басқару, AI чат және қаржылық талдау үшін OpenAI API қолданады.

1. **API ключін алу**: https://platform.openai.com/api-keys

2. **Қолданбаны іске қосу**:
```bash
flutter run --dart-define=OPENAI_API_KEY=sk-your-key-here
```

3. **Production build**:
```bash
# Android үшін
flutter build apk --dart-define=OPENAI_API_KEY=sk-your-key-here

# iOS үшін
flutter build ios --dart-define=OPENAI_API_KEY=sk-your-key-here
```

**Толық нұсқаулық**: `zaman_bank_super_app/ENV_SETUP.md`

## 🎨 Дизайн принциптері

### Түстер (Ислам банкинг тақырыбы)

- **Басты түс**: Жасыл (#10b981) - өсу мен гүлденуді білдіреді
- **Фон**: Ашық сұр (#f8f9fa) - таза және заманауи көрініс
- **Акцент**: Көк (#3b82f6) - сенімділік пен қауіпсіздік

### UI/UX мүмкіндіктері

- ✅ Material Design 3 принциптері
- ✅ Responsive дизайн (барлық экран өлшемдеріне)
- ✅ Тегіс анимациялар және өтулер
- ✅ Қараңғы режим қолдауы (болашақта)
- ✅ Accessibility стандарттары

## 📦 Қолданылған технологиялар

### Frontend
```yaml
dependencies:
  flutter: SDK
  provider: ^6.1.1              # State басқару
  http: ^1.1.0                  # HTTP сұраулар
  shared_preferences: ^2.2.2    # Локальді деректерді сақтау
  intl: ^0.18.1                 # Интернационализация
  fl_chart: ^0.65.0            # Графиктер мен диаграммалар
  image_picker: ^1.0.7         # Сурет таңдау
  record: ^5.0.4               # Аудио жазу
  audioplayers: ^5.2.1         # Аудио ойнату
  path_provider: ^2.1.2        # Файл жолдары
```

### Backend
```gradle
dependencies {
    implementation 'org.springframework.boot:spring-boot-starter-web'
    implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
    implementation 'org.springframework.boot:spring-boot-starter-security'
    implementation 'org.postgresql:postgresql'
    implementation 'io.jsonwebtoken:jjwt-api:0.11.5'
    implementation 'org.springdoc:springdoc-openapi-starter-webmvc-ui:2.0.2'
}
```

## 🔐 Қауіпсіздік

- **JWT Token**: Аутентификация үшін
- **Password Hashing**: BCrypt алгоритмі
- **HTTPS**: SSL/TLS шифрлау
- **API Key қорғанысы**: Environment variables
- **Session Management**: Қауіпсіз сессия басқару

## 🧪 Тестілеу

```bash
# Flutter тесттері
cd zaman_bank_super_app
flutter test

# Integration тесттері
flutter drive --target=test_driver/app.dart

# Backend тесттері
cd zaman_bank_api
./gradlew test
```

## 📱 Қолдайтын платформалар

- ✅ Android (API 21+)
- ✅ iOS (iOS 11.0+)
- ✅ Web (Chrome, Safari, Firefox)
- ⏳ Desktop (Windows, macOS, Linux) - болашақта

## 🌐 API Endpoints

### Аутентификация
- `POST /api/auth/register` - Тіркелу
- `POST /api/auth/login` - Кіру
- `POST /api/auth/refresh` - Token жаңарту

### Транзакциялар
- `GET /api/transactions` - Барлық транзакциялар
- `POST /api/transactions/transfer` - Ақша аударым
- `GET /api/transactions/history` - Тарих

### Баланс
- `GET /api/balance` - Қолда бар баланс
- `POST /api/balance/top-up` - Шотты толықтыру

### AI чат
- `POST /api/chat/with-context` - AI-мен чат
- `POST /api/chat/system-message` - Жүйелік хабарлама

Толық API документациясы: `http://localhost:8080/swagger-ui.html`

## 🔄 CI/CD

```yaml
# GitHub Actions мысалы
name: Build and Test
on: [push, pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: subosito/flutter-action@v2
      - run: flutter pub get
      - run: flutter test
      - run: flutter build apk
```

## 📈 Болашақ жоспарлар

### Version 2.0
- [ ] Биометриялық аутентификация (Face ID, Touch ID)
- [ ] Оффлайн режим
- [ ] Көптілділік (Қазақша, Орысша, Ағылшынша)
- [ ] Қараңғы режим
- [ ] Криптовалюта қолдауы

### Version 3.0
- [ ] Blockchain интеграциясы
- [ ] NFT портфолиосы
- [ ] Халықаралық аударымдар
- [ ] AI қаржылық кеңесші (толық)
- [ ] Социальді төлемдер

## 👥 Команда

- **Разработчик**: Zaman Bank Dev Team
- **Дизайн**: UI/UX Design Team
- **Backend**: Java Spring Boot Team
- **Mobile**: Flutter Development Team

## 🤝 Үлес қосу (Contributing)

Үлес қосқыңыз келсе:

1. Репозиторийді fork жасаңыз
2. Feature branch жасаңыз (`git checkout -b feature/AmazingFeature`)
3. Өзгерістерді commit жасаңыз (`git commit -m 'Add some AmazingFeature'`)
4. Branch-ке push жасаңыз (`git push origin feature/AmazingFeature`)
5. Pull Request ашыңыз

## 📄 Лицензия

Бұл жоба демонстрациялық мақсатта жасалған.

## 📞 Байланыс

- **Email**: support@zamanbank.kz
- **Website**: https://zamanbank.kz
- **GitHub**: https://github.com/Sanat-07/ZamanBank

## 🙏 Алғыс

- Flutter команда
- OpenAI (GPT-4, Whisper, TTS)
- Spring Boot команда
- Open source қауымдастығы

---

**Made with ❤️ in Kazakhstan**

**Ислам банкингінің принциптеріне сай жасалған** ☪️

