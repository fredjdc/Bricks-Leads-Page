# Bricks Leads - Brand Guidelines

## 🎨 Brand Overview

Bricks Leads is a real estate agent management app designed for the Peruvian market. The brand follows the same design principles as the main Bricks.pe mortgage calculator app, maintaining consistency across the product ecosystem.

**Brand Personality:**
- Professional yet approachable
- Modern and clean
- Trustworthy and reliable
- User-friendly and intuitive

---

## 🎯 Color Palette

### Primary Colors
```css
/* Main Brand Blue */
primary: "#007AFF"        /* Primary brand color */
primaryDark: "#0056CC"    /* Darker blue for hover states */

/* Accent Colors */
secondary: "#5856D6"      /* Purple accent */
accent: "#34C759"         /* Success green */
warning: "#FF9500"        /* Warning orange */
danger: "#FF3B30"         /* Error red */
```

### Text Colors
```css
textPrimary: "#1C1C1E"    /* Primary text - Dark gray */
textSecondary: "#3C3C43"  /* Secondary text - Medium gray */
textTertiary: "#8E8E93"   /* Tertiary text - Light gray */
```

### Background Colors
```css
background: "#FFFFFF"           /* Main background - White */
backgroundSecondary: "#F2F2F7" /* Secondary background - Light gray */
backgroundTertiary: "#E5E5EA"  /* Tertiary background - Lighter gray */
```

### Border Colors
```css
border: "#C7C7CC"        /* Standard border */
borderLight: "#E5E5EA"   /* Light border */
```

---

## 📝 Typography

### Font Family
- **Primary Font:** Inter (Google Fonts)
- **Fallback:** system-ui, sans-serif
- **Weights:** 300, 400, 500, 600, 700, 800

### Font Usage Guidelines

#### Headings
```css
/* Hero Title */
text-5xl md:text-6xl lg:text-7xl font-bold leading-tight tracking-tight

/* Section Headings */
text-4xl md:text-5xl font-bold leading-tight

/* Subsection Headings */
text-xl font-semibold
```

#### Body Text
```css
/* Large Body Text */
text-xl leading-relaxed font-light

/* Standard Body Text */
text-base leading-relaxed

/* Small Text */
text-sm
```

#### Navigation
```css
/* Navigation Links */
text-sm font-medium
```

---

## 🎨 Design Elements

### Gradients

#### Hero Gradient
```css
.hero-gradient {
    background: linear-gradient(135deg, #007AFF 0%, #5856D6 100%);
}
```

#### Card Gradient (Glassmorphism)
```css
.card-gradient {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.1) 0%, rgba(255, 255, 255, 0.05) 100%);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255, 255, 255, 0.2);
}
```

#### Button Gradient
```css
.btn-primary {
    background: linear-gradient(135deg, #007AFF 0%, #0056CC 100%);
}

.btn-primary:hover {
    background: linear-gradient(135deg, #0056CC 0%, #004499 100%);
}
```

### Shadows

```css
/* Soft Shadow */
shadow-soft: "0 2px 8px rgba(0, 0, 0, 0.08)"

/* Medium Shadow */
shadow-medium: "0 4px 16px rgba(0, 0, 0, 0.12)"

/* Large Shadow */
shadow-large: "0 8px 32px rgba(0, 0, 0, 0.16)"
```

### Border Radius
```css
/* Small radius */
rounded-lg    /* 8px */

/* Medium radius */
rounded-xl    /* 12px */

/* Large radius */
rounded-2xl   /* 16px */

/* Extra large radius */
rounded-3xl   /* 24px */

/* Full circle */
rounded-full  /* 50% */
```

---

## 🎭 Component Styles

### Buttons

#### Primary Button
```css
.btn-primary {
    background: linear-gradient(135deg, #007AFF 0%, #0056CC 100%);
    color: white;
    font-weight: 600;
    padding: 1rem 2rem;
    border-radius: 12px;
    transition: all 0.3s ease;
}

.btn-primary:hover {
    background: linear-gradient(135deg, #0056CC 0%, #004499 100%);
    transform: translateY(-1px);
    box-shadow: 0 8px 25px rgba(0, 122, 255, 0.3);
}
```

#### Secondary Button
```css
/* Navigation links */
text-textSecondary hover:text-primary px-3 py-2 rounded-lg text-sm font-medium transition-all duration-200 hover:bg-backgroundSecondary
```

### Form Elements

#### Input Fields
```css
.input-field {
    padding: 1rem 1.25rem;
    border-radius: 12px;
    border: 2px solid transparent;
    transition: all 0.3s ease;
    background: rgba(255, 255, 255, 0.9);
    backdrop-filter: blur(4px);
}

.input-field:focus {
    border-color: #007AFF;
    box-shadow: 0 0 0 3px rgba(0, 122, 255, 0.1);
}
```

### Cards

#### Feature Cards
```css
.feature-card {
    background: white;
    border-radius: 16px;
    padding: 2rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
    border: 1px solid #E5E5EA;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.feature-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 40px rgba(0, 0, 0, 0.15);
}
```

#### Icon Containers
```css
/* Feature icons */
w-16 h-16 bg-primary/10 rounded-2xl flex items-center justify-center mb-6

/* Success icons */
w-16 h-16 bg-accent rounded-full flex items-center justify-center mx-auto mb-4
```

---

## 🎬 Animations & Interactions

### Floating Animation
```css
.floating {
    animation: floating 4s ease-in-out infinite;
}

@keyframes floating {
    0%, 100% {
        transform: translateY(0px) rotate(-2deg);
    }
    50% {
        transform: translateY(-15px) rotate(-1deg);
    }
}
```

### Pulse Glow
```css
.pulse-glow {
    animation: pulse-glow 2s ease-in-out infinite alternate;
}

@keyframes pulse-glow {
    from {
        box-shadow: 0 0 20px rgba(0, 122, 255, 0.4);
    }
    to {
        box-shadow: 0 0 30px rgba(0, 122, 255, 0.7);
    }
}
```

### Transitions
```css
/* Standard transition */
transition: all 0.3s ease

/* Smooth transition */
transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1)
```

---

## 📱 Layout Guidelines

### Spacing System
```css
/* Section padding */
py-24 px-4 sm:px-6 lg:px-8

/* Container max width */
max-w-7xl mx-auto

/* Grid gaps */
gap-8    /* Cards */
gap-16   /* Hero sections */
gap-12   /* Footer sections */
```

### Responsive Breakpoints
```css
/* Mobile first approach */
sm: 640px   /* Small screens */
md: 768px   /* Medium screens */
lg: 1024px  /* Large screens */
xl: 1280px  /* Extra large screens */
```

### Grid Layouts
```css
/* Hero section */
grid grid-cols-1 lg:grid-cols-2 gap-16 items-center

/* Feature cards */
grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8

/* Footer */
grid grid-cols-1 md:grid-cols-2 gap-12
```

---

## 🎨 Visual Hierarchy

### Text Sizes
```css
/* Hero title */
text-5xl md:text-6xl lg:text-7xl

/* Section headings */
text-4xl md:text-5xl

/* Subsection headings */
text-xl

/* Body text */
text-xl (large)
text-base (standard)
text-sm (small)
```

### Icon Sizes
```css
/* Large icons */
text-4xl

/* Medium icons */
text-3xl

/* Small icons */
text-2xl
```

---

## 🔧 Technical Implementation

### TailwindCSS Configuration
```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                primary: "#007AFF",
                primaryDark: "#0056CC",
                secondary: "#5856D6",
                accent: "#34C759",
                warning: "#FF9500",
                danger: "#FF3B30",
                textPrimary: "#1C1C1E",
                textSecondary: "#3C3C43",
                textTertiary: "#8E8E93",
                background: "#FFFFFF",
                backgroundSecondary: "#F2F2F7",
                backgroundTertiary: "#E5E5EA",
                border: "#C7C7CC",
                borderLight: "#E5E5EA"
            },
            fontFamily: {
                sans: ["Inter", "system-ui", "sans-serif"]
            },
            boxShadow: {
                soft: "0 2px 8px rgba(0, 0, 0, 0.08)",
                medium: "0 4px 16px rgba(0, 0, 0, 0.12)",
                large: "0 8px 32px rgba(0, 0, 0, 0.16)"
            }
        }
    }
}
```

### CSS Custom Properties
```css
/* Custom scrollbar */
::-webkit-scrollbar {
    width: 8px;
}

::-webkit-scrollbar-track {
    background: #F2F2F7;
}

::-webkit-scrollbar-thumb {
    background: #C7C7CC;
    border-radius: 4px;
}

::-webkit-scrollbar-thumb:hover {
    background: #8E8E93;
}
```

---

## 📋 Usage Guidelines

### Do's ✅
- Use the primary blue (#007AFF) for main actions and branding
- Maintain consistent spacing with the defined system
- Use Inter font family for all text
- Apply hover effects on interactive elements
- Use glassmorphism effects for hero sections
- Maintain proper contrast ratios for accessibility

### Don'ts ❌
- Don't use colors outside the defined palette
- Don't mix different font families
- Don't skip hover states on interactive elements
- Don't use hard shadows (always use the defined shadow system)
- Don't use border radius values outside the defined system

### Accessibility
- Ensure sufficient color contrast (WCAG AA compliant)
- Use semantic HTML elements
- Provide focus indicators for keyboard navigation
- Maintain readable font sizes (minimum 16px for body text)

---

## 🎯 Brand Consistency

### With Bricks.pe
- Same color palette and typography
- Consistent button and form styling
- Similar gradient usage
- Matching visual hierarchy
- Compatible design language

### File Structure
```
Bricks-Leads-Page/
├── index.html          /* Main landing page */
├── thank-you.html      /* Success page */
├── images/             /* Brand assets */
│   ├── heroimage1.png  /* Hero mockup */
│   └── image1.PNG      /* Favicon */
├── CNAME               /* Domain configuration */
└── BRANDING.md         /* This file */
```

---

## 🔄 Version History

### v1.0 (Current)
- Initial brand implementation
- Matches Bricks.pe design system
- Professional real estate focus
- Peruvian market optimization
- Modern, clean aesthetic

---

*This document should be updated whenever brand changes are made to maintain consistency across all Bricks products.* 