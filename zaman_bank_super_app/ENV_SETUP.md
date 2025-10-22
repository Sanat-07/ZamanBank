# Environment Setup

## OpenAI API Key Configuration

This application uses OpenAI API for voice recognition, text-to-speech, and AI-powered financial advice.

### Setup Instructions

1. Get your OpenAI API key from: https://platform.openai.com/api-keys

2. **For Development:**
   
   Run the app with the API key as an environment variable:
   
   ```bash
   flutter run --dart-define=OPENAI_API_KEY=your_api_key_here
   ```

3. **For Production Build:**
   
   ```bash
   flutter build apk --dart-define=OPENAI_API_KEY=your_api_key_here
   ```

### Security Note

- Never commit your actual API keys to the repository
- The `.env` file is git-ignored for your security
- Use the `.env.example` file as a template

### Files Using OpenAI API

- `lib/services/chat_service.dart` - Voice-to-text and text-to-speech
- `lib/services/voice_service.dart` - Voice recognition features
- `lib/screens/financial_analysis_screen.dart` - AI financial advice

