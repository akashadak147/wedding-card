# 💍 Royal Bengali Wedding Online Invitation Card

An ultra-luxury, interactive digital wedding invitation card website with smooth animations, custom Bengali typography, traditional royal aesthetic, background shehnai music, and interactive elements.

Direct replica and customizable template of the online wedding invitation: [https://online-invitation-card-jh9w.vercel.app/](https://online-invitation-card-jh9w.vercel.app/)

---

## ✨ Features & Sections

1. **Preloader & Auspicious Blessing**:
   - Golden animated winged butterfly motif with glowing aura and progress line.
   - Sacred Sanskrit / Bengali blessing: *"প্রজাপতয়ে নমঃ"* (*Prajapataye Namah*).

2. **Grand Stage & Gate Opening**:
   - Royal maroon drapes with golden tassels that part upon entering.
   - Traditional auspicious seals and motifs.

3. **Background Music & Sound Controls**:
   - High-fidelity traditional wedding background music (`bgm.mp3`).
   - Floating interactive spinning vinyl gold button with Play/Pause state and Bengali tooltip (*"মিউজিক অন / অফ"*).

4. **Hero & Parallax Canopy**:
   - High-definition couple portrait with parallax depth and animated video loop backdrop.
   - Golden foil Bengali typography (*"শুভ বিবাহ"*), couple names, wedding date, and real-time floating rose petals canvas effect.

5. **I · The Couple (*বর ও কনে*)**:
   - Ornate architectural arch frames (`arch__frame`) dynamically generated with SVG gold bevels.
   - Bride profile (photo, parents, bio).
   - Groom profile (photo, parents, bio).
   - Swinging temple bells (`bells`) with animated golden bead strings.

6. **II · The Invitation Envelope (*নিমন্ত্রণপত্র*)**:
   - Interactive 3D wedding card envelope with royal wax seal and opening ceremony.
   - Sacred Vedic wedding mantra:
     > *যদেতৎ হৃদয়ং তব, তদস্তু হৃদয়ং মম।*  
     > *যদিদং হৃদয়ং মম, তদস্তু হৃদয়ং তব॥*  
     *(তোমার এই হৃদয় আমার হোক, আমার এই হৃদয় তোমার।)*
   - Formal invitation letter with interactive toggle between **Bride Side (*কন্যাপক্ষ*)** and **Groom Side (*বরপক্ষ*)**.

7. **III · The Auspicious Date (*শুভ দিন*)**:
   - Date breakdown: Friday, 22 January 2027.
   - Auspicious Lagna (*"শুভ লগ্ন রাত ৯টা ১২ মিনিট"*).
   - Interactive calendar widget with date highlight and **"Add to Google Calendar"** button.

8. **IV · Countdown Timer (*আর মাত্র*)**:
   - Real-time live countdown timer (Days, Hours, Minutes, Seconds) ticking down to the Shubhodrishti ceremony.

9. **V · Memories & Kolkata Stories (*আমাদের কলকাতা*)**:
   - Photo gallery capturing memorable spots: Prinsep Ghat (*প্রথম দেখা*), College Street (*পুরোনো বইয়ের গন্ধ*), Howrah Bridge (*নৌকায়, সূর্য ডোবার আগে*), Victoria Memorial (*শীতের দুপুর*), Shobhabazar Rajbari (*যেখানে হ্যাঁ বলা*).
   - Smooth horizontal gallery carousel track.

10. **VI · Itinerary & Functions (*অনুষ্ঠানসূচি*)**:
    - Comprehensive multi-day wedding schedule cards:
      * **আশীর্বাদ (Ashirbad)** · Wednesday, 20 Jan · 11:00 AM · Sen bari, Behala
      * **গায়ে হলুদ (Gaye Holud)** · Friday, 22 Jan · 8:00 AM · দু'বাড়িতেই
      * **বিয়ে (Biye)** · Friday, 22 Jan · 7:00 PM · Golap Bagan Banquet, Behala
      * **বৌভাত (Boubhat)** · Sunday, 24 Jan · 7:30 PM · Mukherjee bari, Salt Lake

11. **VII · Wedding Night Timeline (*বিয়ের রাত*)**:
    - Step-by-step evening timeline with progress line:
      * **7:00 PM** · বর বরণ (Bor Boron)
      * **8:00 PM** · খাওয়াদাওয়া (Dinner)
      * **9:12 PM** · শুভদৃষ্টি ও মালাবদল (Shubhodrishti & Mala Bodol)
      * **11:30 PM** · সিঁদুরদান (Sindoor Daan)

12. **VIII · The Venue & Location (*কোথায়*)**:
    - Venue photograph in an ornate golden antique frame.
    - Banquet name & address with parking note.
    - Interactive embedded Google Map + 1-click **"Get Directions"** Google Maps link.
    - Traditional dress code guide with royal color palette swatches: Oxblood (`#4a0a12`), Crimson (`#9e1b2b`), Gold (`#c9a24a`), Ivory (`#f3e9d6`).

13. **IX · Closing & Share (*আসবেন কিন্তু*)**:
    - Heartfelt closing note from both families (*"সেন ও মুখার্জি পরিবার"*).
    - Floating rose petals canvas.
    - 1-click **"Share invite"** button using the Web Share API (WhatsApp, Messages, Facebook) with automatic fallback to clipboard copy.

---

## 🚀 How to Run Locally

### Option 1: Using Node.js (Recommended)
Run the built-in HTTP server:
```bash
npm start
```
Or:
```bash
node server.js
```
Then open your browser and navigate to:  
👉 **[http://localhost:3000](http://localhost:3000)**

### Option 2: Using Python
If you have Python installed:
```bash
python -m http.server 3000
```
Open **[http://localhost:3000](http://localhost:3000)**.

### Option 3: Using VS Code Live Server / NPX Serve
```bash
npx serve -l 3000 .
```

---

## 🎨 How to Customize Everything (`config.js`)

You do **NOT** need to edit complicated code or run build tools to personalize your wedding card!  
Simply open `config.js` in any text editor and update the fields:

```javascript
window.INVITE = {
  // Couple Information
  couple: {
    initials: ["A", "R"],
    bride: {
      first: "Ahana",
      full: "Ahana Sen",
      parents: "Mitali & Subrata Sen",
      parentsBn: "মিতালি ও সুব্রত সেনের মেয়ে",
      about: "স্কুলে ফিজিক্স পড়ায়, আর রবীন্দ্রসংগীত ধরলে ঘরটা চুপ হয়ে যায়।"
    },
    groom: {
      first: "Ritwik",
      full: "Ritwik Mukherjee",
      parents: "Rupa & Debashis Mukherjee",
      parentsBn: "রূপা ও দেবাশিস মুখার্জির ছেলে",
      about: "পেশায় আর্কিটেক্ট। ইস্টবেঙ্গল হারলে সেদিন আর ফোন ধরে না।"
    }
  },

  // Wedding Dates & Auspicious Lagna
  wedding: {
    startISO: "2027-01-22T19:00:00+05:30",
    endISO: "2027-01-23T00:30:00+05:30",
    weekday: "Friday",
    short: "22 · 01 · 2027",
    city: "Kolkata",
    bnDay: "শুক্রবার",
    bnDate: "২২শে জানুয়ারি",
    bnYear: "২০২৭",
    bnLagna: "শুভ লগ্ন রাত ৯টা ১২ মিনিট",
    lagna: "9:12 PM",
    year: 2027,
    monthIndex: 0, // 0 = Jan, 1 = Feb, ...
    day: 22
  },

  // Venue & Google Maps
  venue: {
    name: "Golap Bagan Banquet",
    address: "Behala, Kolkata",
    mapQuery: "Behala, Kolkata",
    note: "পার্কিং আছে, গেটে বললেই দেখিয়ে দেবে।"
  },

  // Multi-day events (Ashirbad, Gaye Holud, Biye, Boubhat)
  events: [ ... ],

  // Night timeline (Bor Boron, Dinner, Shubhodrishti, Sindoor Daan)
  night: [ ... ],

  // Photo Gallery
  gallery: [ ... ]
};
```

### Changing Photos:
Simply replace the images in the `assets/` folder:
- Bride photo: `assets/bride.webp`
- Groom photo: `assets/groom.webp`
- Couple photo: `assets/couple.webp`
- Venue photo: `assets/venue.webp`
- Gallery photos: `assets/kolkata-1.webp` to `assets/kolkata-5.webp`

### Changing Background Music:
Replace `assets/bgm.mp3` with your preferred wedding track or Shehnai music!

---

## 🌐 Free 1-Click Deployment (Vercel / Netlify / GitHub Pages)

### Deploy to Vercel:
1. Install Vercel CLI (or push this repository to GitHub):
   ```bash
   npx vercel
   ```
2. Follow the on-screen prompts (accept default settings).
3. Your wedding invitation card will be live instantly with a free SSL URL (e.g., `https://your-wedding-card.vercel.app`)!

### Deploy to Netlify:
- Drag and drop this folder directly into the [Netlify Drop](https://app.netlify.com/drop) dashboard.

### Deploy to GitHub Pages:
- Push the repository to GitHub and enable **GitHub Pages** from Repository Settings -> Pages -> Deploy from Branch (`main` / root).

---

## 📱 WhatsApp & Social Media Preview

When sharing the link on WhatsApp, Facebook, or Instagram, a rich card will automatically appear with:
- Title: *"Ahana & Ritwik · শুভ বিবাহ"*
- Description: *"২২শে জানুয়ারি, ২০২৭ · আহানা ও ঋত্বিকের শুভ বিবাহে আপনাকে সপরিবারে আন্তরিক নিমন্ত্রণ।"*
- Image: `assets/og-preview.jpg` (1200x630)

You can customize these OpenGraph meta tags in [index.html](file:///c:/Users/User/OneDrive/Desktop/Wedding/index.html).

