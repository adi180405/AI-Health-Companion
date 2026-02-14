# 🤖 AI Health Companion

An intelligent health and nutrition assistant powered by Google's Gemini AI that provides personalized meal planning, food analysis, and health insights based on your unique health profile.

## Features

### 📋 Personalized Meal Planning
- Generate custom 7-day meal plans tailored to your health goals
- Nutritional breakdown with calories and macros
- Context-aware meal suggestions based on your dietary preferences
- Organized shopping lists and preparation tips
- Downloadable meal plans for offline access

### 🍽️ Food Analysis
- Upload photos of your meals for instant nutritional analysis
- Get detailed macronutrient breakdowns
- Identify potential health benefits and concerns
- Receive portion size recommendations
- Multi-item meal analysis

### 💡 Health Insights
- Ask nutrition and health-related questions
- Get science-backed, personalized recommendations
- Practical advice tailored to your health profile
- Evidence-based suggestions for foods and supplements

### 👤 Health Profile Management
- Track your health goals
- Record medical conditions
- Log fitness routines
- Set food preferences and dietary restrictions
- Persistent profile across sessions

## Installation

### Prerequisites
- Python 3.8 or higher
- Google API key for Gemini AI

### Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd ai-health-companion
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the project root:
```env
GOOGLE_API_KEY=your_gemini_api_key_here
```

4. Run the application:
```bash
streamlit run app.py
```

## Required Dependencies

```txt
streamlit
python-dotenv
google-generativeai
Pillow
```

## Usage

### Setting Up Your Health Profile

1. Open the sidebar
2. Fill in your health information:
   - **Health Goals**: Weight loss, muscle gain, improved energy, etc.
   - **Medical Conditions**: Any relevant health conditions
   - **Fitness Routines**: Current exercise habits
   - **Food Preferences**: Vegetarian, vegan, keto, etc.
   - **Dietary Restrictions**: Allergies, intolerances, ethical restrictions
3. Click "Update Profile" to save

### Generating a Meal Plan

1. Navigate to the "Meal Planning" tab
2. Add any specific requirements (optional)
3. Click "Generate Personalized Meal Plan"
4. Review your custom 7-day plan
5. Download the plan using the download button

### Analyzing Food

1. Go to the "Food Analysis" tab
2. Upload a photo of your meal (JPG, JPEG, or PNG)
3. Click "Analyze Food"
4. Review the nutritional breakdown and recommendations

### Getting Health Insights

1. Switch to the "Health Insights" tab
2. Type your health or nutrition question
3. Click "Get Expert Insights"
4. Read the personalized, evidence-based response

## Configuration

The app uses Google's Gemini 2.5 Flash model by default. You can modify the model in the code:

```python
model = genai.GenerativeModel('gemini-2.5-flash')
```

## Privacy & Security

- All data is stored locally in session state
- Health profiles persist only during your session
- No data is sent to third parties except Google's Gemini API for processing
- Ensure your `.env` file is added to `.gitignore` to protect your API key

## Limitations

- Meal plans and health advice are AI-generated and should not replace professional medical advice
- Always consult with healthcare professionals for medical decisions
- Nutritional estimates from food images are approximations
- API rate limits may apply based on your Google Cloud account

## Troubleshooting

**Issue**: "Error generating response"
- **Solution**: Check your GOOGLE_API_KEY in the `.env` file
- Verify your API key has access to Gemini models

**Issue**: Image upload fails
- **Solution**: Ensure the image is in JPG, JPEG, or PNG format
- Check file size (large images may take longer to process)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Disclaimer

This application is for informational purposes only and is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Powered by [Google Gemini AI](https://deepmind.google/technologies/gemini/)
- Icons from emoji sets

## Support

For issues, questions, or suggestions, please open an issue on the GitHub repository.

---

**Made with ❤️ for healthier living**
