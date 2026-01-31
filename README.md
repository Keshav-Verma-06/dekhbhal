# Dekhbhal - Healthcare App

A complete, connected healthcare app designed for elderly patients and their caregivers, with Hindi/English bilingual support.

## 🎯 App Overview

**Dekhbhal** (meaning "Care" in Hindi) is a healthcare companion app that helps elderly patients manage medications, track health progress, and maintain a health diary. The app features a warm, caring assistant named **Savan** who guides users through their healthcare journey.

## 📱 App Flow

### Complete Navigation Flow:

```
index.html (Welcome)
    ↓
bhasha_chunein (Language Selection)
    ↓
pehchaan_chunein (Profile Selection - Patient/Caregiver)
    ↓
savan_se_miliye (Meet Savan - Voice Assistant)
    ↓
aaj_ka_din (Today's Dashboard - Main Hub)
    ├→ meri_dawaiyan (My Medications)
    │   ├→ dawai_ki_jankari (Medicine Details)
    │   └→ dawai_ki_yaad-dihani (Medicine Reminder)
    ├→ aapki_pragati (Your Progress)
    └→ meri_diary (My Diary)
```

## 📄 Pages Description

### 1. **index.html** - Welcome Screen
- App introduction with warm illustration
- Two CTAs: "Shuru Karein" (Start) and "Login"
- Entry point to the app

### 2. **bhasha_chunein/code.html** - Language Selection
- Choose from Hindi, English, Marathi, Tamil, Telugu
- Visual language selector with radio buttons
- Selected language highlighted with sage green

### 3. **pehchaan_chunein/code.html** - Profile Selection
- Choose user role:
  - **Main Mareez Hoon** (I am the patient)
  - **Main Dekhbhal Kar Raha Hoon** (I am the caregiver)
- Beautiful card-based selection with images

### 4. **savan_se_miliye/code.html** - Meet Savan
- Introduction to Savan, the AI healthcare companion
- Voice test feature
- Warm, welcoming character design

### 5. **aaj_ka_din/code.html** - Today's Dashboard (Main Hub)
- Daily greeting with user profile
- Timeline view of daily activities
- Progress tracking
- **Bottom Navigation Bar** for quick access to:
  - Home (Aaj ka Din)
  - Dawai (Medications)
  - Pragati (Progress)
  - Diary

### 6. **meri_dawaiyan/code.html** - My Medications
- Daily medication list
- Progress summary (e.g., "2/3 completed")
- Medication cards with:
  - Medicine name
  - Time
  - Status (completed/pending)
  - Quick action buttons
- Click on any medicine for details

### 7. **dawai_ki_jankari/code.html** - Medicine Details
- Complete medicine information
- Dosage and timing
- Instructions (e.g., "खाने के बाद" - After food)
- Savan's caring message about the medicine
- "Dawai Li" (Took Medicine) button

### 8. **dawai_ki_yaad-dihani/code.html** - Medicine Reminder
- Full-screen reminder with emotional connection
- Shows loved one's photo
- Two action buttons:
  - "Haan, le li" (Yes, I've taken it)
  - "Abhi nahi" (Not now - Remind in 15 mins)
- Designed like an incoming call for urgency

### 9. **aapki_pragati/code.html** - Your Progress
- Visual progress tracking
- Growth visualization (rising sun metaphor)
- Weekly adherence view
- Motivational messages
- Past days rhythm visualization

### 10. **meri_diary/code.html** - My Diary
- Health journal/notes
- Timeline of entries
- Today and yesterday sections
- Entries include:
  - Symptoms/feelings
  - Medicine intake
  - Side effects
- "Naya Note" (New Note) button

## 🎨 Design Features

### Color Palette:
- **Primary**: `#e89c30` (Warm saffron/gold)
- **Background Light**: `#fdfaf5` (Soft cream)
- **Background Dark**: `#211a11` (Dark brown)
- **Sage Highlight**: `#d1e8e2` (For selected states)

### Typography:
- **Font Family**: Lexend (primary), Noto Sans (for Hindi text)
- Clean, readable, modern

### UI Elements:
- Rounded corners (border-radius: 0.5rem to 1.5rem)
- Soft shadows
- Smooth transitions
- Active states with scale effects
- Dark mode support throughout

### Navigation:
- **Bottom Navigation Bar** on main pages:
  - Home (Aaj ka Din)
  - Dawai (Medications)
  - Pragati (Progress)
  - Diary
- Back buttons on all screens
- Contextual navigation (e.g., medicine card → medicine details)

## 🔗 Interactive Features

### Button Actions:
- All navigation buttons are functional
- Medicine cards link to detail pages
- Action buttons (Li gayi, Info) work correctly
- Progress tracking updates
- Dark mode toggle

### Smart Navigation:
- Linear onboarding flow
- Bottom nav for main app sections
- Back buttons maintain context
- Medicine reminder redirects after action

## 🌐 Bilingual Support

The app is designed for Hindi-speaking elderly users but supports:
- Hindi (primary)
- English (secondary labels)
- Other Indian languages (Marathi, Tamil, Telugu)

## 📱 Responsive Design

- Maximum width: 430px (mobile-first)
- Centered on larger screens
- iOS-style spacing and indicators
- Touch-friendly interactive elements

## 🚀 How to Use

1. Open `index.html` in your browser to start
2. Click "Shuru Karein" for onboarding or "Login" to go directly to dashboard
3. Follow the onboarding: Language → Profile → Meet Savan
4. Use the bottom navigation to switch between main sections
5. Click on medication cards for details
6. Dark mode toggle is in the bottom-right corner

## 🛠️ Technical Stack

- **HTML5**: Semantic markup
- **Tailwind CSS**: Utility-first styling via CDN
- **JavaScript**: Vanilla JS for interactions
- **Google Fonts**: Lexend, Material Symbols
- **No build process required**: Pure HTML/CSS/JS

## 📝 Files Structure

```
stitch/
├── index.html                          # Main welcome page
├── README.md                          # This file
├── aaj_ka_din/code.html              # Today's dashboard
├── aapki_pragati/code.html           # Progress tracking
├── bhasha_chunein/code.html          # Language selection
├── dawai_ki_jankari/code.html        # Medicine details
├── dawai_ki_yaad-dihani/code.html    # Medicine reminder
├── meri_dawaiyan/code.html           # Medication list
├── meri_diary/code.html              # Health diary
├── pehchaan_chunein/code.html        # Profile selection
├── savan_se_miliye/code.html         # Meet Savan
└── welcome_to_dekhbhal/code.html     # Alternative welcome page
```

## 🎭 User Experience Highlights

- **Warm & Caring**: Designed with emotional intelligence
- **Culturally Appropriate**: Indian context, Hindi language
- **Elder-Friendly**: Large buttons, clear text, simple navigation
- **Visual Hierarchy**: Important actions are prominent
- **Feedback**: Visual states for all interactions
- **Consistency**: Same navigation pattern throughout

## 🌟 Key Features

✅ Complete onboarding flow
✅ Daily medication tracking
✅ Medicine reminders with emotional connection
✅ Progress visualization
✅ Health diary/journal
✅ AI companion (Savan)
✅ Bilingual support
✅ Dark mode
✅ Mobile-optimized
✅ No internet required (after initial load)

## 📞 Support

This is a complete, functional prototype. All navigation is connected, and the UI/images remain exactly as designed. Users can navigate through the entire app seamlessly.

---

**Made with care for elderly healthcare management** 💛
