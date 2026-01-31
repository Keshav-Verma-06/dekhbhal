# 🔗 Dekhbhal App - Complete Navigation Map

## 📱 Full Page Connection Overview

### 🎬 **Onboarding Flow** (First-time users)
```
1. index.html (Welcome Screen)
   ├─ "Shuru Karein" → bhasha_chunein/code.html
   └─ "Login" → aaj_ka_din/code.html (Skip to dashboard)

2. bhasha_chunein/code.html (Language Selection)
   ├─ Back → index.html
   └─ "Aage Badhein" → pehchaan_chunein/code.html

3. pehchaan_chunein/code.html (Profile Selection)
   ├─ Back → bhasha_chunein/code.html
   ├─ "Select Profile" (Patient) → savan_se_miliye/code.html
   └─ "Select Profile" (Caregiver) → savan_se_miliye/code.html

4. savan_se_miliye/code.html (Meet Savan)
   ├─ Back → pehchaan_chunein/code.html
   ├─ "Test Voice" → Plays sample voice
   └─ "Continue to Dashboard" → aaj_ka_din/code.html
```

---

## 🏠 **Main App Navigation** (After onboarding)

### **Dashboard Hub: aaj_ka_din/code.html**
The main dashboard with bottom navigation to all major sections:

**Bottom Navigation Bar:**
```
┌──────────┬──────────┬──────────┬──────────┬──────────┐
│   Home   │  Dawai   │   Book   │ Pragati  │ Profile  │
│  (Stay)  │  (Meds)  │ (Diary)  │(Progress)│ (Info)   │
└──────────┴──────────┴──────────┴──────────┴──────────┘
     ↓          ↓          ↓          ↓          ↓
   Current  meri_dawai meri_diary aapki_prag  (Tab view)
             yan/code    /code     ati/code
```

**Features on Dashboard:**
- Greeting with profile picture
- Daily timeline of activities
- Medication reminders
- Caregiver messages
- Internal tabs for different views

---

## 💊 **Medication Flow**

### **meri_dawaiyan/code.html** (My Medications)
```
Features:
├─ Back Button → aaj_ka_din/code.html
├─ Progress Summary (e.g., "2/3 completed")
├─ Medicine Cards (clickable)
│  ├─ Click card → dawai_ki_jankari/code.html
│  ├─ "Li gayi" button → dawai_ki_yaad-dihani/code.html
│  └─ Info icon → dawai_ki_jankari/code.html
└─ Bottom Nav Bar:
   ├─ Home → aaj_ka_din/code.html
   ├─ Dawai (current)
   ├─ Pragati → aapki_pragati/code.html
   └─ Diary → meri_diary/code.html
```

### **dawai_ki_jankari/code.html** (Medicine Details)
```
Features:
├─ Back Button → meri_dawaiyan/code.html
├─ Medicine image
├─ Dosage information
├─ Timing (subah/dopahar/raat)
├─ Instructions (khane ke baad, etc.)
├─ Savan's message
├─ "Dawai Li" button
└─ Bottom Nav Bar (same as above)
```

### **dawai_ki_yaad-dihani/code.html** (Medicine Reminder)
```
Full-screen reminder with:
├─ Loved one's photo background
├─ Medicine name & time
├─ "Haan, le li" (Yes, taken) → aaj_ka_din/code.html
└─ "Abhi nahi" (Not now) → aaj_ka_din/code.html
```

---

## 📈 **Progress Tracking**

### **aapki_pragati/code.html** (Your Progress)
```
Features:
├─ Back Button → aaj_ka_din/code.html
├─ Growth visualization (rising sun)
├─ Weekly adherence view
├─ Motivational messages
├─ "Theek Hai" button (acknowledgment)
└─ Bottom Nav Bar:
   ├─ Home → aaj_ka_din/code.html
   ├─ Dawai → meri_dawaiyan/code.html
   ├─ Pragati (current)
   └─ Diary → meri_diary/code.html
```

---

## 📔 **Health Diary**

### **meri_diary/code.html** (My Diary)
```
Features:
├─ Back Button → aaj_ka_din/code.html
├─ Timeline of entries:
│  ├─ Today's entries
│  └─ Yesterday's entries
├─ Entry types:
│  ├─ Symptoms (chakkar aaya)
│  ├─ Medicine intake
│  └─ Side effects
├─ "Naya Note" button (Add new entry)
└─ Bottom Nav Bar:
   ├─ Home → aaj_ka_din/code.html
   ├─ Dawai → meri_dawaiyan/code.html
   ├─ Pragati → aapki_pragati/code.html
   └─ Diary (current)
```

---

## 🎯 **Quick Navigation Reference**

### All Pages Can Navigate To:
✅ **Back to Previous Page** (Back button in header)
✅ **Main Dashboard** (Bottom nav "Home" button)
✅ **Medications** (Bottom nav "Dawai" button)
✅ **Progress** (Bottom nav "Pragati" button)
✅ **Diary** (Bottom nav "Book" button)

### Special Navigation:
- **Welcome/Login** → Skips onboarding
- **Medicine Cards** → Medicine details
- **Medicine Actions** → Reminders or completion
- **Reminders** → Return to dashboard after action

---

## 🔄 **Complete User Journey Examples**

### **Example 1: First-time User**
```
Welcome → Language → Profile → Meet Savan → Dashboard
  ↓
Explore: Meds → Progress → Diary → Back to Dashboard
```

### **Example 2: Returning User Taking Medicine**
```
Dashboard → Medications → Click "Aspirin" → View Details → "Dawai Li"
  ↓
Back to Dashboard (medicine marked complete)
```

### **Example 3: Responding to Reminder**
```
(Reminder notification appears)
dawai_ki_yaad-dihani → "Haan, le li" → Dashboard
```

### **Example 4: Checking Progress**
```
Dashboard → Progress → View weekly adherence → "Theek Hai" → Dashboard
```

---

## 🎨 **Interactive Elements**

### Buttons That Work:
✅ All navigation buttons
✅ All back buttons
✅ Language selection radio buttons
✅ Profile selection cards
✅ Medicine cards (clickable)
✅ "Li gayi" (Taken) buttons
✅ Info buttons
✅ Bottom navigation tabs
✅ Dark mode toggle (floating button)
✅ Action buttons on reminders

---

## 🚀 **How to Test the Full App**

1. **Start Fresh:** Open `index.html`
2. **Onboarding:** Click "Shuru Karein" → Select language → Choose profile → Meet Savan
3. **Dashboard:** Explore the timeline and sections
4. **Navigate:** Use bottom navigation to visit all main sections
5. **Medications:** Click on medicine cards to see details
6. **Return:** Use back buttons to navigate back
7. **Dark Mode:** Toggle using floating button (bottom-right)

---

## ✅ **Verification Checklist**

- [x] Welcome page connects to language selection
- [x] Language selection connects to profile
- [x] Profile selection connects to Savan intro
- [x] Savan intro connects to dashboard
- [x] Dashboard has bottom navigation
- [x] All bottom nav buttons work
- [x] Back buttons on all pages work
- [x] Medicine list connects to details
- [x] Medicine details has proper navigation
- [x] Reminders return to dashboard
- [x] Progress page is accessible
- [x] Diary page is accessible
- [x] All pages maintain same design/images
- [x] Dark mode works across all pages

---

**Status: ✨ ALL PAGES FULLY CONNECTED AND FUNCTIONAL ✨**

The complete app is now ready to use! All navigation flows work seamlessly, and users can move through the entire application without any dead ends.
