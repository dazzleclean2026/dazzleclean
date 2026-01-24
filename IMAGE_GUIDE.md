# 🖼️ Image Setup Guide for DAZZLE CLEAN

## Service Cards with Images

### What You'll See:

Each service card now has this structure:

```
┌─────────────────────────────┐
│      IMAGE AREA (600x400)   │  ← Your image goes here
│   (Fallback: Emoji icon)    │
├─────────────────────────────┤
│  Service Title              │
├─────────────────────────────┤
│  • Feature 1                │
│  • Feature 2                │
│  • Feature 3                │
├─────────────────────────────┤
│  ₹Price Range               │
├─────────────────────────────┤
│  [Book Service Button]      │
└─────────────────────────────┘
```

## Image File Names (EXACT):

### 1. House Cleaning
**File Name**: `house-cleaning.jpg`
**Gradient**: Blue to Cyan background
**Size**: 600x400px (recommended)
**Content Ideas**:
- Clean living room
- Sparkling kitchen
- Bathroom after cleaning
- Person cleaning floor
- Before/After comparison

### 2. Car Cleaning  
**File Name**: `car-cleaning.jpg`
**Gradient**: Red to Orange background
**Size**: 600x400px (recommended)
**Content Ideas**:
- Car foam washing
- Detailing work
- Shiny car exterior
- Interior vacuum cleaning
- Professional wash process

### 3. Two Wheeler Cleaning
**File Name**: `two-wheeler-cleaning.jpg`
**Gradient**: Yellow to Green background
**Size**: 600x400px (recommended)
**Content Ideas**:
- Bike with shiny exterior
- Water spray on bike
- Polish and shine work
- Chrome details
- Before/After bike

## How Images Work in HTML:

```html
<div class="mb-6 w-full h-48 bg-gradient-to-br from-blue-100 to-cyan-100 
            rounded-xl flex items-center justify-center overflow-hidden">
    
    <!-- Your Image (Loads if file exists) -->
    <img src="house-cleaning.jpg" 
         alt="House Cleaning Service" 
         class="w-full h-full object-cover" 
         onerror="this.style.display='none'">
    
    <!-- Fallback Icon (Shows if image missing) -->
    <div class="text-6xl">🏠</div>
</div>
```

### How It Works:
1. ✅ If image found → **Image displays**
2. ❌ If image missing → **Emoji displays**
3. No errors → Everything works smooth

## Free Image Sources:

### Best Free Stock Photo Sites:
1. **Unsplash.com** (Free, High Quality)
   - Search: "house cleaning", "car wash", "motorcycle"
   
2. **Pexels.com** (Free, Good Selection)
   - Search: "professional cleaning", "car detailing"
   
3. **Pixabay.com** (Free, Diverse)
   - Search: "home cleaning", "automotive care"

4. **Shutterstock/Getty** (Paid, Premium)
   - Professional service photos

## Download & Setup Steps:

### Step 1: Find Images
Go to Unsplash.com → Search "house cleaning"
→ Click image → Download

### Step 2: Rename Files
Ensure files are named EXACTLY:
- `house-cleaning.jpg`
- `car-cleaning.jpg`
- `two-wheeler-cleaning.jpg`

### Step 3: Place Files
Copy files to: `d:\2026Works\`

### Step 4: Refresh Browser
Open `index.html` and refresh (Ctrl+F5 or Cmd+Shift+R)

## Image Specifications:

| Aspect | Details |
|--------|---------|
| **Format** | JPG or PNG |
| **Size** | 600x400px minimum |
| **Max File Size** | 500KB each |
| **Dimensions** | 3:2 aspect ratio |
| **Quality** | High (72+ DPI) |
| **Fallback** | Emoji icon |

## Responsive Behavior:

### Desktop (1200px+):
```
Image: Full size (600x400px)
Card: 3-column grid
```

### Tablet (768px-1199px):
```
Image: Scales down (responsive)
Card: 2-column or 3-column grid
```

### Mobile (< 768px):
```
Image: Full width (-20px margins)
Card: Single column (stacked)
Image Height: 200px (h-48)
```

## Example Folder Structure:

```
d:\2026Works\
│
├── index.html                    (Main website)
├── tailwind_3_4_17.js           (Tailwind CSS)
│
├── house-cleaning.jpg           (Service image 1)
├── car-cleaning.jpg             (Service image 2)
├── two-wheeler-cleaning.jpg     (Service image 3)
│
├── README.md                    (Overview)
├── SETUP_INSTRUCTIONS.md        (This file)
└── IMAGE_GUIDE.md              (Image details)
```

## Troubleshooting:

### Images Not Showing?

❌ **Problem**: Image file missing
✅ **Solution**: 
   - Check filename spelling
   - Use correct extension (.jpg/.png)
   - Place in same folder as index.html

❌ **Problem**: Image too large
✅ **Solution**:
   - Compress image to <500KB
   - Resize to 600x400px
   - Use image compressor tools

❌ **Problem**: Image aspect ratio wrong
✅ **Solution**:
   - Maintain 3:2 ratio (600x400)
   - Use image editor to crop
   - Recommrend: 600x400px exactly

## Image Quality Tips:

✓ Use professional, clean images
✓ Ensure good lighting
✓ Show action (people cleaning)
✓ Use consistent style across all 3
✓ Keep colors vibrant
✓ Avoid cluttered backgrounds
✓ Include company branding if possible

## Browser Testing:

### Test Image Loading:
1. Open `index.html` in browser
2. Look at Services section
3. All 3 image areas should show:
   - Either your image OR
   - Colored emoji icon

### Mobile Testing:
1. Right-click → Inspect
2. Toggle Device Toolbar (Ctrl+Shift+M)
3. Check images on mobile view
4. Should be responsive

## Alternative: AI-Generated Images

If you don't have real photos, try:
- **Midjourney** - Realistic service images
- **DALL-E** - Generated cleaning photos
- **Stable Diffusion** - Free option

Search: "professional house cleaning service photo"

---

**Need Help?**
Email: alexanderthe2005@gmail.com
Phone/WhatsApp: 9744718332

**Version**: 1.0
**Updated**: January 23, 2026
