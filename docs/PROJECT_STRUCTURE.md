# AgroConnect - Project Structure Guide

Comprehensive guide to understanding the AgroConnect project folder structure, organization, and file purpose.

---

## 📁 Directory Tree

```
AgroConnect/
│
├── 📄 index.html                          # Main landing page
├── 📄 style.css                           # Global CSS styling
├── 📄 README.md                           # Project overview
├── 📄 LICENSE                             # License file (MIT)
├── 📄 .gitignore                          # Git ignore rules
│
├── 📁 01-HTML/                            # HTML pages directory
│   ├── about.html                         # About Us page
│   ├── blog.html                          # Blog & Articles page
│   ├── contact.html                       # Contact Us page
│   ├── login.html                         # Login page
│   ├── Organic.html                       # Organic Products page
│   └── sign-in.html                       # Sign In page
│
├── 📁 02-CSS/                             # CSS styling directory
│   ├── about.css                          # About page styles
│   ├── blog.css                           # Blog page styles
│   ├── contact.css                        # Contact page styles
│   ├── login.css                          # Login page styles
│   ├── Organic.css                        # Organic page styles
│   └── sign-in.css                        # Sign In page styles
│
├── 📁 03-script/                          # JavaScript directory
│   └── script.js                          # Main JavaScript file
│
├── 📁 04-assets/                          # Media & Assets directory
│   ├── final-text-logo-1.png              # AgroConnect logo
│   ├── 📁 about-img/                      # About page images
│   │   └── 📁 icons/                      # Icon assets
│   ├── 📁 blog-img/                       # Blog page images
│   └── 📁 Organic/                        # Organic products images
│
├── 📁 AgroConnect/                        # Project assets folder
│   └── present-logo.jpeg                  # Presentation logo
│
├── 📁 docs/                               # Documentation folder
│   ├── INSTALLATION.md                    # Installation guide
│   ├── FEATURES.md                        # Features documentation
│   ├── CONTRIBUTING.md                    # Contributing guidelines
│   ├── ROADMAP.md                         # Development roadmap
│   └── PROJECT_STRUCTURE.md               # This file
│
├── 📄 AgroConnect.drawio.pdf              # Project flow diagram
│
└── 📁 .git/                               # Git version control (hidden)
```

---

## 📄 File Descriptions

### Root Level Files

#### `index.html`
- **Purpose:** Main landing/home page of AgroConnect
- **Contains:** Hero section, navigation, feature highlights
- **Links to:** All other pages, external resources
- **Size:** ~5-10 KB
- **Key Sections:**
  - Navigation bar with logo
  - Hero banner
  - Feature highlights
  - Call-to-action buttons
  - Footer with links

#### `style.css`
- **Purpose:** Global CSS styles used across all pages
- **Contains:** 
  - CSS variables (colors, fonts)
  - Navigation styling
  - Common utility classes
  - Responsive design rules
  - Media queries
- **Size:** ~10-15 KB
- **Usage:** Linked in HTML files as primary stylesheet

#### `README.md`
- **Purpose:** Project overview and main documentation
- **Contains:**
  - Project description
  - Features list
  - Team information
  - Installation instructions
  - Usage guide
  - Links to other documentation

#### `LICENSE`
- **Purpose:** Open-source license (MIT)
- **Specifies:** Terms of use and distribution
- **Includes:** Copyright and permissions

#### `.gitignore`
- **Purpose:** Tell Git which files to ignore
- **Contains:**
  - Node modules
  - System files (like `.DS_Store`)
  - Environment variables
  - Build artifacts

---

## 📁 01-HTML/ Directory

### Purpose
Contains all HTML page files for different sections of the website.

### File Structure

#### `about.html`
- **Purpose:** About Us page
- **Contains:**
  - Company mission and vision
  - Team information
  - Company history
  - Values and principles
- **Links:** Navigation to other pages
- **Size:** ~4-6 KB

#### `blog.html`
- **Purpose:** Blog and educational content page
- **Contains:**
  - Article listings
  - Blog categories
  - Feature posts
  - Search functionality (planned)
- **Links:** Individual blog posts
- **Interactive Features:** Pagination, filtering
- **Size:** ~5-8 KB

#### `contact.html`
- **Purpose:** Contact Us / Support page
- **Contains:**
  - Contact form
  - Contact information
  - Location map (planned)
  - Social media links
- **Forms:** Contact form with validation
- **Size:** ~4-6 KB

#### `login.html`
- **Purpose:** User login page
- **Contains:**
  - Login form
  - Email/username field
  - Password field
  - Remember me checkbox
  - Forgot password link
  - Sign up link
- **Forms:** Login form
- **Planned Features:** Social login, 2FA
- **Size:** ~3-4 KB

#### `Organic.html`
- **Purpose:** Explore organic products page
- **Contains:**
  - Product listings
  - Product categories
  - Product filters
  - Farmer information
  - Price information
- **Interactive:** Product cards, filtering
- **Size:** ~6-10 KB
- **Future:** Shopping cart, checkout

#### `sign-in.html`
- **Purpose:** User sign-up/registration page
- **Contains:**
  - Registration form
  - User information fields
  - Address fields
  - Terms acceptance checkbox
  - Create account button
- **Forms:** Registration form with validation
- **Planned Features:** Email verification, social signup
- **Size:** ~4-6 KB

---

## 📁 02-CSS/ Directory

### Purpose
Contains page-specific CSS styling for better organization and maintainability.

### File Structure
Each CSS file corresponds to an HTML file:

```
HTML File          →  CSS File
about.html         →  about.css
blog.html          →  blog.css
contact.html       →  contact.css
login.html         →  login.css
Organic.html       →  Organic.css
sign-in.html       →  sign-in.css
```

### CSS File Organization

Each CSS file contains:
1. **Layout Styles** - Grid, Flexbox, positioning
2. **Typography** - Fonts, sizes, colors
3. **Component Styles** - Buttons, cards, forms
4. **Responsive Styles** - Media queries
5. **Animation** - Transitions, animations

### File Sizes
- Typical file: 2-4 KB
- Total CSS: ~15-25 KB

### Best Practices Used
- Mobile-first approach
- CSS variables for consistency
- Organized commenting
- DRY (Don't Repeat Yourself)
- Clear class naming

---

## 📁 03-script/ Directory

### Purpose
Contains JavaScript files for interactivity and functionality.

### File Structure

#### `script.js`
- **Purpose:** Main JavaScript file for client-side functionality
- **Contains:**
  - DOM manipulation
  - Event listeners
  - Form validation
  - Navigation functionality
  - User interaction handlers
- **Size:** ~5-10 KB
- **Key Functions:**
  - Menu toggle (mobile hamburger)
  - Form submission handlers
  - Input validation
  - Local storage management
  - API calls (when backend ready)

### JavaScript Features
- ES6+ syntax (arrow functions, destructuring)
- Error handling
- Comments for complex logic
- Performance optimized

---

## 📁 04-assets/ Directory

### Purpose
Store all media files (images, icons, etc.)

### Directory Structure

```
04-assets/
├── final-text-logo-1.png          # Main logo
├── about-img/                     # About page images
│   ├── about-hero.jpg
│   ├── team-member-1.jpg
│   ├── team-member-2.jpg
│   └── icons/                     # Small icon assets
│       ├── mission-icon.svg
│       ├── vision-icon.svg
│       └── values-icon.svg
├── blog-img/                      # Blog page images
│   ├── blog-post-1.jpg
│   ├── blog-post-2.jpg
│   └── featured-article.jpg
└── Organic/                       # Organic products images
    ├── vegetables/
    ├── fruits/
    └── dairy/
```

### Asset Management

**Image Naming Convention:**
- Lowercase with hyphens
- Descriptive names
- Include size indicator if relevant
- Examples: `hero-banner-1920.jpg`, `product-card-300.png`

**Image Optimization:**
- Compressed sizes
- Appropriate format (JPG/PNG/WebP)
- Alt text in HTML
- Responsive images (srcset for multiple sizes)

**Asset Types:**
- Logo files (PNG with transparency)
- Photography (JPG for compression)
- Icons (SVG or PNG)
- Backgrounds (JPG or WebP)

---

## 📁 AgroConnect/ Directory

### Purpose
Additional project-related assets and materials

### Contents
- `present-logo.jpeg` - Logo for presentations
- Other branding materials (if needed)

---

## 📁 docs/ Directory

### Purpose
Comprehensive project documentation for developers, users, and contributors.

### File Structure

#### `INSTALLATION.md`
- How to install and set up the project
- System requirements
- Step-by-step instructions
- Troubleshooting guide

#### `FEATURES.md`
- Detailed feature documentation
- User-facing features
- Technical features
- Feature status matrix

#### `CONTRIBUTING.md`
- Guidelines for contributing
- Code standards
- Commit message format
- Pull request process
- Code of conduct

#### `ROADMAP.md`
- Project development timeline
- Planned features by phase
- Success metrics
- Budget estimates

#### `PROJECT_STRUCTURE.md`
- This file
- Directory and file explanations
- Organization principles
- Naming conventions

---

## 📊 File Size Guide

### Typical File Sizes
```
index.html          ~8 KB
style.css           ~12 KB
script.js           ~8 KB
Each page HTML      ~5 KB
Each page CSS       ~3 KB
Logo                ~80 KB
Product images      ~150-300 KB each
Total package       ~1-2 MB
```

---

## 🔄 File Dependencies

```
index.html
  ├── style.css
  ├── script.js
  ├── 04-assets/final-text-logo-1.png
  └── Links to:
      ├── 01-HTML/about.html
      ├── 01-HTML/blog.html
      ├── 01-HTML/contact.html
      ├── 01-HTML/Organic.html
      └── 01-HTML/sign-in.html

Each HTML page depends on:
  ├── Its corresponding CSS file
  ├── style.css (global)
  ├── script.js
  ├── Assets for images
  └── Font Awesome (CDN)
```

---

## 📋 Naming Conventions

### HTML Files
- **Format:** kebab-case.html
- **Examples:** `about.html`, `sign-in.html`, `organic.html`
- **Note:** Use lowercase except for proper nouns

### CSS Files
- **Format:** kebab-case.css
- **Examples:** `about.css`, `sign-in.css`
- **Convention:** Match HTML filename

### JavaScript Files
- **Format:** camelCase.js or kebab-case.js
- **Examples:** `script.js`, `form-validation.js`

### CSS Classes
- **Format:** .kebab-case
- **Examples:** `.main-content`, `.button-primary`

### CSS IDs
- **Format:** #camelCase
- **Examples:** `#menuToggle`, `#userProfile`

### Image Files
- **Format:** kebab-case.extension
- **Examples:** `hero-banner.jpg`, `product-card.png`
- **Convention:** Descriptive names with optional size

---

## 📈 Folder Organization Principles

### 1. **Separation of Concerns**
- HTML in `01-HTML/`
- CSS in `02-CSS/`
- JavaScript in `03-script/`
- Assets in `04-assets/`

### 2. **Scalability**
- Easy to add new pages
- Clear structure for growth
- Ready for backend integration

### 3. **Maintainability**
- Clear file purposes
- Logical organization
- Comprehensive documentation

### 4. **Performance**
- Organized asset loading
- Minimal dependencies
- Optimized file sizes

---

## 🔍 Finding Files

### To find a specific feature:
```
Feature → Related HTML → Check CSS file → Check script.js → Check assets
```

### Example: "Where is the product listing?"
```
01-HTML/Organic.html → 02-CSS/Organic.css → 04-assets/Organic/
```

### Example: "Where is button styling?"
```
style.css (global) → 02-CSS/{page}.css (specific)
```

---

## 📝 Adding New Files

### To add a new page:
1. Create `01-HTML/new-page.html`
2. Create `02-CSS/new-page.css`
3. Add link to `index.html` navigation
4. Import CSS in the new HTML file
5. Add page-specific images to `04-assets/`
6. Update documentation

### Checklist:
- [ ] HTML file created
- [ ] CSS file created
- [ ] Links are correct
- [ ] Images added to assets
- [ ] Navigation updated
- [ ] README updated
- [ ] Tested on mobile

---

## 🚀 Quick Navigation

| Want | Location |
|------|----------|
| Add a new page | Create in `01-HTML/` + `02-CSS/` |
| Change styling | Edit `style.css` or page CSS |
| Add functionality | Edit `03-script/script.js` |
| Add images | Store in `04-assets/` |
| Installation help | Read `docs/INSTALLATION.md` |
| Contributing | Read `docs/CONTRIBUTING.md` |
| Feature info | Read `docs/FEATURES.md` |
| Roadmap | Read `docs/ROADMAP.md` |

---

## 📚 Directory Statistics

### Current Structure
- Total directories: 9
- HTML files: 7
- CSS files: 7
- JavaScript files: 1
- Documentation files: 5
- Image directories: 3

### Growth Ready
- Can easily add more pages
- Structure supports scaling
- Ready for backend integration

---

## 🔗 File Relationships

```
User visits website
        ↓
index.html loads
        ↓
Loads: style.css, script.js, logo image
        ↓
User clicks navigation
        ↓
Loads specific page HTML (e.g., about.html)
        ↓
Loads: about.css, script.js, images
        ↓
JavaScript handles interactivity
        ↓
CSS applies styling
```

---

## 📖 Documentation Reference

For more information:
- **Installation:** See `docs/INSTALLATION.md`
- **Features:** See `docs/FEATURES.md`
- **Contributing:** See `docs/CONTRIBUTING.md`
- **Roadmap:** See `docs/ROADMAP.md`
- **Main README:** See `README.md`

---

## ✅ File Checklist

When creating new content:
- [ ] File created in appropriate folder
- [ ] Proper naming convention used
- [ ] Links are relative and correct
- [ ] CSS imported properly
- [ ] Images optimized
- [ ] Mobile responsive
- [ ] No broken links
- [ ] Documentation updated
- [ ] git add and commit

---

**Last Updated:** March 2026  
**Status:** Project Structure Guide v1.0
