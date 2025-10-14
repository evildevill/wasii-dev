# Changelog

All notable changes to wasii.dev (personal portfolio and educational platform) will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Released]

Features and fixes currently in development.

---

## [2.2.0] - 2025-01-15

### Added
- **User Verification System (Blue Badge)** 🌟
  - Apply for verification badge with document upload
  - Admin review dashboard for verification requests
  - Verified badges displayed across the platform
  - Real-time status tracking (verified, pending, rejected)
  
- **Course Certificates** 🎓
  - Auto-generated certificates on course completion
  - QR code verification system
  - Social media sharing (LinkedIn, Twitter/X, Facebook)
  - Certificate gallery in dashboard
  - Public verification page
  
- **Cryptomus Payment Gateway** 💰
  - Cryptocurrency payments (Bitcoin, Ethereum, USDT)
  - Invoice creation with QR codes
  - Real-time payment tracking
  - Webhook integration for order updates
  - Admin refund and payout support

### Updated
- Public profile pages now show verification badges
- Dashboard shows verification status card
- Improved certificate design to match site branding
- Enhanced payment checkout flow

### Fixed
- Certificate generation for both database and static courses
- Database index migration for course progress
- robots.txt conflict resolution
- TypeScript and ESLint production build errors

---

## [2.1.0] - 2025-01-09

### Added
- **Email Notifications** 📧
  - Welcome email for new users after onboarding
  - Verification status emails (approved/rejected)
  - Admin notification when user applies for verification
  
- **User Onboarding Flow** 🎯
  - 3-step onboarding process for new users
  - Username, display name, and bio setup
  - Profile photo upload (optional)
  - Social links configuration (optional)
  - Real-time username availability checking

### Updated
- Profile edit page with all user information
- Smart social link input (auto-constructs URLs from usernames)
- Middleware integration for onboarding redirects

---

## [2.0.0] - 2025-01-08

### Added
- **Public Profile Pages** 👤
  - Beautiful profile pages at `/u/username`
  - Profile stats and activity section
  - Share profile functionality
  - Profile cards and links for comments/posts

### Removed
- **Polar Payment Integration** 
  - Removed Polar payment provider
  - Migrated to cryptocurrency payments only

---

## [1.5.0] - 2024-12-01

### Added
- **Newsletter System** 📨
  - Full newsletter editor with markdown and drag-and-drop blocks
  - Open and click tracking
  - Unsubscribe handling
  - Queue system for large sends
  - Admin dashboard for sending newsletters

### Updated
- Enhanced newsletter UI with better block editor
- Improved email templates with responsive design

---

## [1.0.0] - 2024-10-01

### Added
- **Initial Platform Launch** 🚀
  - Blog system with markdown/MDX support
  - Course platform with progress tracking
  - Digital store with shopping cart
  - User authentication (Kinde)
  - User dashboard
  - Contact form
  - Newsletter subscription
  - Dark/light theme support

---

## Version History Summary

| Version | Release Date | Highlights |
|---------|--------------|------------|
| 2.2.0 | 2025-01-15 | Verification, Certificates, Crypto Payments |
| 2.1.0 | 2025-01-09 | Onboarding, Email Notifications |
| 2.0.0 | 2025-01-08 | Public Profiles, Payment Migration |
| 1.5.0 | 2024-12-01 | Newsletter System |
| 1.0.0 | 2024-10-01 | Initial Launch |

---

## Roadmap

### Planned Features

#### 🔜 Coming Soon
- [ ] Advanced search functionality
- [ ] Course reviews and ratings
- [ ] Discussion forums
- [ ] Live chat support
- [ ] Mobile app

#### 🎯 Under Consideration
- [ ] Multi-language support (i18n)
- [ ] Video lectures with transcripts
- [ ] AI-powered course recommendations
- [ ] Interactive coding challenges
- [ ] Team/group accounts

#### 📝 Documentation
- [ ] API documentation for developers
- [ ] Video tutorials
- [ ] Platform user guide
- [ ] Course creation guide

---

## Breaking Changes

### Version 2.0.0
- Removed Polar payment integration
- Migrated to Cryptomus for payments
- Users must use cryptocurrency for purchases

---

## Deprecations

### Version 2.0.0
- Polar payment methods deprecated (removed)
- Legacy checkout flow replaced with crypto checkout

---

## Known Issues

### Current
- None at this time

### Resolved
- ✅ Certificate generation for static courses (Fixed in 2.2.0)
- ✅ Database index migration (Fixed in 2.2.0)
- ✅ TypeScript build errors (Fixed in 2.2.0)
- ✅ Cryptomus signature generation (Fixed in 2.2.0)

---

## Security Updates

### 2.2.0
- Enhanced webhook signature verification
- IP whitelist for payment webhooks
- Secure document storage and deletion

### 2.1.0
- Improved input validation for onboarding
- XSS prevention in user profiles

---

## Notes

- For security vulnerabilities, see [SECURITY.md](SECURITY.md)
- For detailed contribution guidelines, see [CONTRIBUTING.md](CONTRIBUTING.md)
- For user documentation, see [docs/](docs/)

---

**Last Updated**: January 15, 2025
