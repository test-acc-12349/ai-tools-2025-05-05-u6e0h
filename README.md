# AI Tools Directory 🤖

> The ultimate directory of AI tools and resources for developers, creators, and businesses.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Netlify Status](https://api.netlify.com/api/v1/badges/your-badge/deploy-status)](https://app.netlify.com/)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization](#customization)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [Support](#support)

## Overview

AI Tools Directory is a responsive, modern directory website showcasing artificial intelligence tools and resources in a clean, three-column grid layout. Built with HTML, CSS, and JavaScript, it offers easy customization and quick deployment options.

## Features

- 📱 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category filtering
- ⚡ Fast loading times
- 🎨 Customizable styling
- 📊 SEO optimized
- 🔄 Easy content updates

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Git
- Text editor (VS Code recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── assets/
│   ├── images/
│   ├── css/
│   └── js/
├── data/
│   └── tools.json
├── components/
├── layouts/
├── pages/
├── public/
└── config.js
```

## Customization

### Adding Directory Items

1. Open `data/tools.json`
2. Add new items following this structure:

```json
{
  "id": "tool-name",
  "title": "Tool Name",
  "description": "Tool description",
  "category": "category-name",
  "url": "https://toolurl.com",
  "image": "/images/tool-image.png"
}
```

### Modifying Categories

Edit the categories in `config.js`:

```javascript
export const categories = [
  {
    id: "chatbots",
    label: "Chatbots"
  },
  // Add more categories
];
```

### Updating Hero Section

Modify the hero section in `components/Hero.js`:

```html
<div class="hero">
  <h1>Your New Title</h1>
  <p>Your new description</p>
</div>
```

### Customizing Colors

Edit `assets/css/variables.css`:

```css
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
  --background-color: #your-color;
}
```

## Deployment

### Netlify Deployment

1. Push your repository to GitHub
2. Login to Netlify
3. Click "New site from Git"
4. Select your repository
5. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy site"

### Vercel Deployment

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

## Custom Domain Setup

1. Purchase domain from your preferred registrar
2. Add domain in deployment platform:
   ```
   Domain: yoursite.com
   ```
3. Update DNS records:
   ```
   A     @     76.76.21.21
   CNAME www   yoursite.netlify.app
   ```

## Troubleshooting

### Common Issues

- **Images not loading**: Check image paths in `tools.json`
- **Categories not filtering**: Verify category IDs match in `config.js`
- **Styling issues**: Clear browser cache and rebuild

### Debug Mode

Enable debug mode in `config.js`:

```javascript
export const debug = true;
```

## Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## Support

- 📖 [Documentation](https://docs.yoursite.com)
- 💬 [Discord Community](https://discord.gg/yourserver)
- 📧 [Email Support](mailto:support@yoursite.com)
- 🐛 [Issue Tracker](https://github.com/yourusername/ai-tools-directory/issues)

## License

MIT © [Your Name]

---

Made with ❤️ by [Your Name](https://yoursite.com)