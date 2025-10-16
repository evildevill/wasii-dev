# 🚀 Waseem Akram - Personal Portfolio & Platform

Welcome to the public repository for [wasii.dev](https://wasii.dev) or [hackerwasii.com](https://hackerwasii.com)! A feature-rich personal portfolio and educational platform built with modern web technologies, showcasing cybersecurity expertise while providing courses, blog content, and professional services.

## 📣 Purpose of This Repository

This repository serves as a **public issue tracker and documentation hub** for the platform. Users can:

- 🐛 **Report Bugs** - Found something broken? Let us know!
- 💡 **Request Features** - Have an idea? We'd love to hear it!
- 📖 **Access Documentation** - Learn how to use the platform
- 💬 **Discuss** - Share feedback and suggestions
- 🔒 **Report Security Issues** - Follow our security policy

> **Note**: This repository contains **documentation only**. The source code is kept private for security reasons.

---

## ✨ Key Features

- 📝 **Markdown/MDX Blog** – Categories, code highlighting (Shiki), frontmatter, related posts
- 🌐 **RSS + Sitemap + SEO** – Automatic `feed.xml`, dynamic sitemap, structured data
- 🔐 **Auth (Kinde)** – User authentication and management (Google and Github)
- 🛒 **Digital Store** – Products (ebooks/tools/courses) with cart & order persistence
- 🎓 **Courses & Lectures** – Lecture ordering, progress tracking, karma points foundation
- 📑 **Course Certificates** – Auto-generated certificates on completion with QR verification, social sharing, and gallery
- 🎥 **Study Material** – Educational resources
- 💬 **Comment System** – Moderated threaded comments with moderation
- 📨 **Full Newsletter System** – Editor, batching, open/click tracking, unsubscribe, queue + cron
- 📬 **Contact & Feedback** – Validated submissions via API routes
- 📅 **Consultation Booking** – Schedule intake pipeline
- 🔗 **URL Shortener** – Create & manage custom short links with analytics tracking
- 🧾 **Legal Pages** – Terms, Privacy, Cookies, Refund
- 📊 **Analytics & Tracking** – Google Analytics + Vercel Analytics + Speed Insights
- 🌗 **Theming** – Dark/light with system preference
- 📁 **File Storage** – Cloudflare R2 (uploads) + Vercel Blob
- ⚙️ **Service Worker / PWA** – Offline experience & installable manifest
- 🛡️ **Security-Oriented** – Strict headers, validation, index-hardened DB schema
- ⚡ **Performance** – Server Components, minimal client hydration, image optimization, caching strategy
- 📂 **Modular Architecture** – Clear separation of concerns across `app`, `components`, `lib`

## 🛠️ Tech Stack

### 🎨 Frontend
- ⚡ **Next.js 15** - React framework with App Router
- ⚛️ **React 19** - UI library
- 🏷️ **TypeScript** - Type-safe JavaScript
- 🎨 **Tailwind CSS** - Utility-first CSS framework
- 🎛️ **Radix UI** - Accessible UI components
- 🌙 **Next Themes** - Dark/light mode support
- ✅ **React Hook Form** - Form validation
- 🔔 **Sonner** - Toast notifications
- 🎨 **Lucide React** - Icon library
- 🎭 **Motion** - Animation library
- 🏗️ **Zod** - Schema validation
- 🧩 **Custom Hooks** - e.g., `use-cart` for shopping cart state
- 🧰 **UI Component Library** - Modular, accessible components in `/components/ui/`

### 🔙 Backend & Database
- 🏗️ **Next.js API Routes** - Serverless functions
- 🗄️ **MongoDB** - NoSQL database
- 📜 **Mongoose** - MongoDB object modeling
- ✉️ **Nodemailer** - Email sending capabilities
- 🛠️ **Custom API Endpoints** - For contact, newsletter, orders, study material, user management, etc.

### 🔑 Authentication
- 🔐 **Kinde Auth** - User authentication and management

### 📝 Content Management
- 📜 **Gray Matter** - Markdown frontmatter parser
- 🛠️ **Unified** - Markdown processing ecosystem
- 🔄 **Rehype/Remark** - HTML/Markdown transformation
- 🎨 **Shiki** - Code syntax highlighting
- 🗂️ **Content Types**: Blog posts, walkthroughs, bug bounty resources, study material, short lectures, guides, and more (see `/content`)

### 🚀 Development & Deployment
- 🔍 **ESLint** - Code linting
- 📦 **TypeScript** - Type checking
- 🌍 **Vercel** - Deployment platform
- ⚡ **Turbopack** - Fast bundling for development
- 🛠️ **Scripts**: Database seeding, migration, and utility scripts in `/scripts`
- 🧪 **Testing**: Playwright e2e testing
- 🔄 **CI/CD**: GitHub Actions, Vercel auto-deploy

---

---
## 🛒 Store & E-commerce

- Digital products: ebooks, courses, tools, templates
- Secure checkout and order confirmation
- User dashboard for order history and downloads
- Cart management with custom React hook (`use-cart`)

---
## 📚 Content Types

- Blog posts (markdown, with code, images, frontmatter)
- Walkthroughs and guides (e.g., TryHackMe, bug bounty, Linux, cloud)
- Study material (assignments, handouts, quizzes)
- Short lectures (video-based, categorized)
- Product documentation

---

## 📈 SEO & Analytics

Implemented via `components/seo.tsx` & structured data in `components/schema-org.tsx`. Dynamic sitemap (`/sitemap.xml`) + `feed.xml` for syndication. Google Analytics + Vercel Analytics + Speed Insights included.

Highlights:
- Canonicals & OG tags from frontmatter + site defaults
- JSON-LD (BlogPosting, BreadcrumbList) injection
- Image optimization (AVIF/WebP) via Next.js image config
- Remote host allowlist (see Images section)
## 📡 RSS Feed

- Auto-generated RSS available at `/feed.xml` (built from Markdown posts in `/content`).
- Caches for a day; update frequency aligns with content changes.

---
## 📲 PWA & Offline Support

## 🐛 How to Report Issues

### Bug Reports
When reporting a bug, please include:

1. **Description** - Clear summary of the issue
2. **Steps to Reproduce** - How can we recreate it?
3. **Expected Behavior** - What should happen?
4. **Actual Behavior** - What actually happened?
5. **Environment** - Browser, OS, device
6. **Screenshots** - If applicable
7. **URL** - Page where the issue occurs

**Example:**
```markdown
**Description**: Cart page shows empty even after adding items

**Steps to Reproduce**:
1. Navigate to /store
2. Add product to cart
3. Click "View Cart"
4. Cart appears empty

**Expected**: Should show added items
**Actual**: Empty cart message displayed
**Browser**: Chrome 120 on Windows 11
**URL**: https://wasii.dev/store/cart
```

### Feature Requests
Please describe:

1. **Feature** - What do you want to see?
2. **Use Case** - Why is it useful?
3. **Example** - How would it work?
4. **Priority** - How important is this to you?

---

## 🔒 Security

Found a security vulnerability? **DO NOT** open a public issue.

Please email: **hi@wasii.dev** or **support@wasii.dev**

We take security seriously and will respond within 48 hours. See [SECURITY.md](SECURITY.md) for our full security policy.

---

## 📚 Documentation

- [User Guide](docs/USER_GUIDE.md) - How to use the platform
- [FAQ](docs/FAQ.md) - Frequently asked questions
- [API Documentation](docs/API.md) - For developers
- [Changelog](CHANGELOG.md) - Recent updates

---

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript, Tailwind CSS v4
- **Backend**: Next.js API Routes, MongoDB
- **Auth**: Kinde Auth
- **Payments**: Cryptomus (cryptocurrency)
- **Content**: Markdown/MDX with syntax highlighting
- **Storage**: Cloudflare R2, Vercel Blob
- **Email**: Nodemailer (SMTP)

---

## 🤝 Contributing

While the main codebase is private, we welcome:

- Bug reports and feature requests
- Documentation improvements
- Content suggestions
- Design feedback
- Translation help (future)

---

## 📄 License

The platform is proprietary. This public repository is for issue tracking and documentation only.

Copyright © 2025 Waseem Akram. All rights reserved.

---

## 📞 Contact

- **Website**: [wasii.dev](https://wasii.dev) or [hackerwasii.com](https://hackerwasii.com)
- **Email**: hi@wasii.dev
- **Support**: support@wasii.dev
- **Instagram**: [@Waseem Akram](https://instagram.com/wasii_254)
- **GitHub**: [@evildevill](https://github.com/evildevill)

---

## 🌟 Support the Project

If you find this platform useful:

- ⭐ Star this repository
- 🐛 Report bugs and issues
- 💡 Suggest new features
- 📢 Share with others
- 📰 Subscribe to our newsletter

---

**Last Updated**: October 2025
