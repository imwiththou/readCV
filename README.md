# readCV archive

A modern, minimalist portfolio and CV website built with Next.js. Showcases your projects, experience, writing, and professional achievements with a clean, responsive design.

## Features

- 📱 **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- ✨ **Smooth Animations** - Powered by Framer Motion for delightful interactions
- 📝 **Markdown Support** - Write articles and content in Markdown
- 🎨 **Customizable Profile** - Easy-to-edit JSON-based profile data
- 🖼️ **Media Gallery** - Display projects with images and rich media
- 🔍 **SEO Optimized** - Built with Next.js for best SEO practices
- 🌙 **Modern Stack** - TypeScript, React 19, and Next.js 15

## Tech Stack

- **Framework**: [Next.js](https://nextjs.org/) 15
- **UI Library**: [React](https://react.dev/) 19
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Animation**: [Framer Motion](https://www.framer.com/motion/)
- **Markdown**: [React Markdown](https://github.com/remarkjs/react-markdown)
- **Styling**: CSS Modules
- **Package Manager**: npm

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/imwiththou/readCV.git
cd readCV
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the site.

## Customization

### Profile Data

Edit `public/content/profileData.json` to customize your profile information:

```json
{
  "general": {
    "displayName": "Your Name",
    "profession": "Your Title",
    "location": "Your Location",
    "byline": "Your tagline",
    "about": "About you",
    "profilePhoto": "/content/media/profilePhoto.jpg"
  }
}
```

### Adding Projects

Add project entries to the `projects` array in `profileData.json`:

```json
{
  "id": "unique-id",
  "year": "2024",
  "heading": "Project Name",
  "description": "Project description",
  "url": "https://project-url.com"
}
```

### Writing Content

Add Markdown files to `public/content/writing/` and they'll be automatically picked up by the site.

### Media Assets

Place images and media files in `public/content/media/` and reference them in your content.

## Project Structure

```
.
├── app/                           # Next.js app directory
│   ├── page.tsx                  # Home page
│   ├── [slug]/                   # Dynamic route for case studies
│   ├── layout.tsx                # Root layout
│   └── *.module.css              # Component styles
├── public/
│   └── content/
│       ├── profileData.json      # Main profile configuration
│       ├── media/                # Images and assets
│       ├── writing/              # Markdown articles
│       └── collaborators/        # Collaborator data
├── next.config.ts                # Next.js configuration
├── tsconfig.json                 # TypeScript configuration
└── package.json                  # Dependencies
```

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## Building for Production

1. Build the project:
```bash
npm run build
```

2. Start the production server:
```bash
npm start
```

The built application will be optimized and ready for deployment.

## Deployment

This project can be easily deployed to [Vercel](https://vercel.com/) (recommended for Next.js):

1. Push your repository to GitHub
2. Visit [vercel.com](https://vercel.com/) and import your repository
3. Vercel will automatically detect Next.js and deploy with optimal settings

Other hosting options:
- [Netlify](https://netlify.com/)
- [GitHub Pages](https://pages.github.com/)
- Traditional VPS/server

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Support

For questions or issues, please open an issue on the GitHub repository.

---

Built with ❤️ by [Steve Wang](https://imwiththou.com)
