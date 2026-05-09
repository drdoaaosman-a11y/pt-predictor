# PT Duration Predictor — Women's Health

A progressive web application for AI-assisted clinical decision support in physical therapy treatment duration prediction for women's health patients.

## 🚀 Features

- **Multi-step form** - Structured intake across demographics, clinical assessment, and functional evaluation
- **Intelligent prediction engine** - AI-powered duration estimates based on diagnosis, pain, comorbidities, and functional status
- **Risk stratification** - Automatic risk tier assignment (Low/Moderate/High)
- **Clinical pathways** - Evidence-based intervention recommendations
- **Real-time confidence metrics** - Model certainty scores for each prediction component
- **Offline support** - Progressive Web App with service worker caching
- **Mobile-first design** - Fully responsive, installable on iOS/Android
- **Accessibility** - WCAG-compliant with semantic HTML and ARIA labels

## 📋 Assessment Domains

### Patient Demographics
- Age, BMI, referral source, insurance type

### Clinical Intake
- Primary diagnosis (pelvic floor, prenatal/postpartum, other women's health)
- Symptom duration (acute → long-term)
- Prior PT episodes
- Pain level (0-10 scale)
- Comorbidities (diabetes, anxiety, obesity, etc.)

### Functional Assessment
- Mobility, ADL, work/activity, sleep quality, social/QoL, pelvic function
- Patient motivation & readiness
- Social support level

### Prediction Output
- **Treatment duration** (weeks) with confidence range
- **Session estimate** (total visits)
- **Risk tier** with color-coded severity
- **Sessions/week** recommendation
- **Clinical pathways** (manual therapy, pelvic floor re-ed, pain neuroscience ed., etc.)
- **Flags & considerations** (high pain, sensitive conditions, insurance barriers, etc.)

## 🛠️ Technology Stack

- **Vanilla JavaScript** - No dependencies (except Tabler Icons CDN)
- **CSS Grid & Flexbox** - Responsive layout
- **Service Worker** - Offline caching & PWA support
- **Web Manifest** - Installable app experience

## 📱 Installation

### Web Browser
Simply visit the app link and use it directly in your browser.

### Mobile Install
1. Open the app in your mobile browser
2. Tap "Add to Home Screen" (iOS) or "Install app" (Android)
3. App works offline with all data stored locally

## 🔒 Privacy & Security

- **Zero data collection** - All patient data stays on user's device
- **No backend calls** - Prediction engine runs entirely client-side
- **HIPAA-friendly** - No cloud transmission or logging
- **Local storage only** - Form data persists only in browser cache

## 📊 Prediction Algorithm

The treatment duration model factors:
- **Base diagnosis duration** - Evidence-based starting point
- **Symptom chronicity** - Acute vs. long-term modifier
- **Pain severity** - High pain adds duration
- **Comorbidities** - Anxiety, obesity, arthritis adjustments
- **Patient motivation** - High motivation reduces duration (-2 weeks)
- **Social support** - Minimal support increases duration
- **Functional status** - Higher limitation scores extend treatment
- **Age & BMI** - Geriatric and obesity factors

Result range: Predicted duration ± 3 weeks confidence band

## 🔧 Customization

Edit the `computePrediction()` function in `index.html` to:
- Adjust base diagnosis weeks
- Modify risk score thresholds
- Add new comorbidities or diagnoses
- Change clinical pathway logic

## 📞 Integration Hooks

The app includes placeholder buttons for LLM integration:
- "Explain this prediction" → Connect to Claude API
- "Suggest interventions" → Evidence-based recommendation engine
- "Reassessment milestones" → Clinical decision support

## 🤝 Contributing

For capstone project improvements or clinical feedback, please document:
1. Diagnosis accuracy vs. real outcomes
2. Duration prediction variance
3. Patient population demographics
4. Clinician feedback on recommendations

## 📄 License

Clinical decision support tool for educational & research use.
Not for diagnostic or treatment decisions without clinician review.

---

**Built for women's physical therapy clinicians** | Capstone Project | AI-Assisted Clinical Decision Support
