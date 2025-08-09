# Plant PV Website

Modern, mobile-friendly Vue.js website for Plant PV solar technology company.

## Features

- **Responsive Design**: Fully mobile-friendly layout that adapts to all screen sizes
- **Modern Tech Stack**: Built with Vue.js 3 and TypeScript for optimal performance
- **Clean UI**: Professional design with blue color scheme matching the brand
- **Timeline Component**: Interactive timeline showcasing company milestones
- **Fast Loading**: Optimized build with Vite for quick page loads

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment to Dreamhost

1. Build the production version: `npm run build`
2. Upload the contents of the `dist/` folder to your Dreamhost public_html directory
3. The site will be available at your domain

## Project Structure

```
src/
├── components/
│   ├── Header.vue      # Site header with logo
│   ├── Hero.vue        # Hero section with company intro
│   ├── Timeline.vue    # Company timeline with milestones
│   └── Footer.vue      # Site footer
├── App.vue             # Main application component
├── main.ts             # Application entry point
└── style.css           # Global styles
```

## Technology Stack

- Vue.js 3
- TypeScript
- Vite
- CSS3 with Flexbox and Grid
