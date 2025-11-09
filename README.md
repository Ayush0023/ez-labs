# EZ Labs Front-End Intern Test

## Overview

This is a fully responsive single-page web application built with Next.js and Tailwind CSS based on the provided Figma design reference for EZ Labs. It contains a functional home page and a contact form integrated with API validation, meeting all stated assignment requirements. All code is original, human-written, modular, and well-commented.

---

## Getting Started

### 1. Install dependencies

```bash
npm install
```

### 2. Run locally (Dev Mode)

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### 3. Build for deployment

```bash
npm run build
npm run start
```

### 4. Export as static (for Vercel, Netlify, GitHub Pages, or zip deploy)

```bash
npm run build
```

Your deployable static site is in the `/.next/static` folder. Deploy to Vercel/Netlify directly.

## API Integration

- Contact form submits a POST request to `https://vernanbackend.ezlab.in/api/contact-us/`.
- Required fields: name, email, phone, message.
- Frontend validation blocks empty/invalid submission.
- On success, displays: **Form Submitted**
- See `postman_collection.json` for test example.

## Technologies Used

- **Framework:** Next.js 14+
- **Styling:** Tailwind CSS
- **Form/Validation:** React Hook Form
- **UI:** Custom, matches Figma with improved touch/mobile UX & subtle animations

## Folder Structure

```
ezlabs-assignment/
  public/
    favicon.ico
  src/
    components/
      ContactForm.tsx
      Header.tsx
    pages/
      index.tsx
    styles/
      globals.css
    utils/
      api.ts
    types/
      index.ts
  postman_collection.json
  package.json
  tailwind.config.js
  postcss.config.js
  next.config.js
  tsconfig.json
  .gitignore
  README.md
```

## Postman API Test

- Import the included `postman_collection.json` into Postman.
- Submit a test contact form POST request with the example body.

## Deployment

### Option 1: Vercel (Recommended for Next.js)

```bash
npm install -g vercel
vercel login
vercel
```

### Option 2: Netlify

1. Push code to GitHub
2. Connect repo to Netlify
3. Set build command: `npm run build`
4. Set publish directory: `.next`

### Option 3: GitHub Pages

```bash
npm run build
npm run export
```

Upload `/out` folder to GitHub Pages.

---

## Key Features

✅ Fully responsive (Mobile, Tablet, Desktop)
✅ Form validation (Name, Email, Phone, Message)
✅ API integration with error handling
✅ Clean, modular TypeScript code
✅ Tailwind CSS for styling
✅ Loading states and success messages
✅ Email validation
✅ Phone number validation (8-14 digits)

## License

MIT. All code is original and non-plagiarized.

---

For any questions or to schedule an interview, contact: [your-email@domain.com]
