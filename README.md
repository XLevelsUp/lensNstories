# Lens N Stories

A modern, multi-disciplinary creative hub offering Photography, Camera Rentals, Studio Spaces, and Podcast Production services.

![Lens N Stories](https://img.shields.io/badge/Next.js-15-black?style=for-the-badge&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=for-the-badge&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-38bdf8?style=for-the-badge&logo=tailwind-css)

## 🎯 Features

- **4 Service Verticals**: Photography, Equipment Rentals, Studio Space, Podcast Studio
- **WhatsApp Integration**: Direct booking via WhatsApp with pre-filled context
- **Modern Industrial Design**: Dark mode, sophisticated typography, premium aesthetics
- **Framer Motion Animations**: Scroll-triggered effects, parallax, micro-interactions
- **SEO Optimized**: Meta tags, Open Graph, structured data
- **Fully Responsive**: Mobile-first design with touch-friendly interactions

## 🚀 Tech Stack

- **Framework**: Next.js 15 (App Router, Turbopack)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **Font**: Inter (Google Fonts)

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/xlevelsuptech/lensnstories.git
cd lensnstories

# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🛠️ Configuration

### WhatsApp Number

Update the WhatsApp number in `lib/whatsapp.ts`:

```typescript
const WHATSAPP_NUMBER = '917010092090'; // Replace with your number
```

### SEO Metadata

Update metadata in each page's `metadata` export:

- `app/page.tsx` - Homepage
- `app/photography/page.tsx` - Photography service
- `app/rentals/page.tsx` - Equipment rentals
- `app/studio/page.tsx` - Studio rental
- `app/podcast/page.tsx` - Podcast studio

### Equipment Catalog

Edit equipment data in `lib/equipment-data.ts`:

```typescript
export const equipmentCatalog: Equipment[] = [
  {
    id: 'sony-a7iv',
    name: 'Sony A7 IV',
    category: 'camera',
    dailyRate: 2500,
    weeklyRate: 15000,
    // ...
  },
];
```

## 📁 Project Structure

```
lensnstories/
├── app/
│   ├── layout.tsx          # Root layout with navigation
│   ├── page.tsx            # Homepage
│   ├── photography/        # Photography service page
│   ├── rentals/            # Equipment rentals page
│   ├── studio/             # Studio rental page
│   └── podcast/            # Podcast studio page
├── components/
│   ├── animations/         # Framer Motion components
│   │   ├── FadeIn.tsx
│   │   ├── StaggerContainer.tsx
│   │   └── ParallaxHero.tsx
│   ├── booking/
│   │   └── BookingFlyout.tsx  # WhatsApp CTA
│   ├── navigation/
│   │   └── MainNav.tsx     # Main navigation
│   ├── services/
│   │   ├── ServiceCard.tsx
│   │   └── EquipmentCard.tsx
│   └── shared/
│       └── TrustSection.tsx
├── lib/
│   ├── whatsapp.ts         # WhatsApp link generator
│   └── equipment-data.ts   # Equipment catalog data
└── public/                 # Static assets
```

## 🎨 Design System

### Colors

```css
--bg-primary: #0f0f0f /* Deep black */ --bg-secondary: #18181b /* Zinc-900 */
  --text-primary: #fafafa /* White */ --text-secondary: #a1a1aa /* Zinc-400 */
  --accent-amber: #f59e0b /* Photography */ --accent-blue: #3b82f6 /* Rentals */
  --accent-purple: #a855f7 /* Studio */ --accent-green: #10b981 /* Podcast */;
```

### Typography

- **Font**: Inter (Google Fonts)
- **Headings**: Bold, 2xl-7xl
- **Body**: Regular, base-xl

## 📱 User Journey

1. **Land on Homepage** → See 4 service verticals
2. **Click Service Card** → Navigate to service page
3. **Click "Book" CTA** → WhatsApp opens with pre-filled message
4. **< 3 Clicks** to inquiry

## 🚢 Deployment

### Vercel (Recommended)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Manual Build

```bash
# Create production build
npm run build

# Start production server
npm start
```

## 📝 Scripts

```bash
npm run dev      # Start development server (Turbopack)
npm run build    # Create production build
npm run start    # Start production server
npm run lint     # Run ESLint
```

## 🔧 Environment Variables

No environment variables required for basic setup. All configuration is in source files.

## 📄 License

© 2026 Lens N Stories. All rights reserved.

## 🤝 Contributing

This is a private project for Lens N Stories.

## 📞 Support

For inquiries, contact via WhatsApp or visit [lensnstories.in](https://lensnstories.in)

---

**Built with ❤️ by XLevelsUp Tech**
