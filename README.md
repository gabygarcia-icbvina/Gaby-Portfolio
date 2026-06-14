# Gaby García — Portfolio

> Personal portfolio website built with Astro, showcasing projects, skills, and background as a software developer.

🌐 **Live:** [gabygarciah-pro.vercel.app](https://gabygarciah-pro.vercel.app)

---

## 🚀 Tech Stack

| Layer | Tech |
|-------|------|
| Framework | [Astro](https://astro.build) |
| Styling | [Tailwind CSS](https://tailwindcss.com) + custom CSS |
| Icons | [Font Awesome](https://fontawesome.com) · [Devicons](https://devicon.dev) |
| Fonts | [Fira Code](https://fonts.google.com/specimen/Fira+Code) |
| Deployment | [Vercel](https://vercel.com) |

---

## ✨ Features

- **Hero section** with CTA buttons and smooth scroll navigation
- **Infinite skills marquee** — server-rendered, zero JS, pauses on hover
- **Projects grid** with live demo and repo links
- **Education timeline**
- **Contact section** with email, GitHub and LinkedIn links
- Fully **static** — no client-side JS except scroll behavior
- Accessible nav with `data-goto` attributes and `scrollIntoView`

---

## 📁 Project Structure

```
/
├── public/
│   └── gg.logo.webp        # Profile image
├── src/
│   ├── layouts/
│   │   └── Layout.astro    # Base HTML layout
│   └── pages/
│       └── index.astro     # Main portfolio page
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

---

## 🛠️ Getting Started

```bash
# Clone the repository
git clone https://github.com/gabygarcia-icbvina/<repo-name>.git
cd <repo-name>

# Install dependencies
npm install

# Start dev server
npm run dev
```

Open [http://localhost:4321](http://localhost:4321) in your browser.

### Available scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build locally
```

---

## 🎨 Customization

### Adding a project

In `src/pages/index.astro`, add an entry to the `projects` array in the frontmatter:

```ts
{
  title: 'My Project',
  description: 'Short description of what it does.',
  tags: ['Astro', 'TypeScript'],
  url: 'https://myproject.vercel.app',
  repo: 'https://github.com/username/my-project',
}
```

### Adding a skill

Add an entry to the `skills` array. Use `learning: true` to show the blue "learning" badge:

```ts
{ name: 'Rust', icon: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rust/rust-original.svg', learning: true }
```

---

## 📄 License

This portfolio is open source under the [MIT License](LICENSE). Feel free to use it as a template — a credit link back is appreciated but not required.

---

<p align="center">
  Made with ♥ by <a href="https://github.com/gabygarcia-icbvina">Gaby García</a> · Built with Astro
</p>