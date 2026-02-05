# Synora Brand Guide & Design System

## Table of Contents
1. [Brand Identity](#brand-identity)
2. [Logo System](#logo-system)
3. [Color Palette](#color-palette)
4. [Typography](#typography)
5. [Icon System](#icon-system)
6. [Visual Hierarchy](#visual-hierarchy)
7. [Component Library](#component-library)
8. [Voice & Tone](#voice--tone)
9. [Usage Guidelines](#usage-guidelines)

---

## Brand Identity

### Brand Essence
**Synora** represents the future of intelligent decentralized finance, combining cutting-edge AI technology with secure blockchain infrastructure.

### Brand Personality
- **Innovative**: Forward-thinking and technologically advanced
- **Secure**: Trustworthy and reliable
- **Intelligent**: Smart and efficient
- **Inclusive**: Accessible to all users
- **Professional**: Clean and sophisticated

### Brand Promise
*"Intelligent DeFi for Everyone"*

---

## Logo System

### Primary Logo
The Synora logo consists of a stylized "S" letterform with DeFi network nodes, representing connectivity and decentralization.

### Logo Variations
1. **Primary Logo**: Full wordmark with icon
2. **Icon Only**: Stylized "S" with network nodes
3. **Wordmark Only**: "Synora" typography
4. **AI Badge**: "AI" identifier for AI-powered features

### Logo Usage Rules
- **Minimum Size**: 24px height for digital
- **Clear Space**: Minimum 0.5x logo height on all sides
- **Background**: Use on light or dark backgrounds with sufficient contrast
- **Modifications**: Do not alter, stretch, or modify the logo

### Logo Files
- `favicon.svg` - Browser icon
- `logo-primary.svg` - Main logo
- `logo-icon.svg` - Icon only
- `logo-wordmark.svg` - Wordmark only

---

## Color Palette

### Primary Colors
```css
--synora-blue: #3b82f6;      /* Primary brand color */
--synora-purple: #8b5cf6;    /* Secondary brand color */
--synora-gradient: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 100%);
```

### Secondary Colors
```css
--synora-green: #10a37f;     /* Success, AI, growth */
--synora-orange: #f97316;    /* Warning, attention */
--synora-red: #ef4444;        /* Error, danger */
```

### Neutral Colors
```css
--synora-gray-50: #f8fafc;    /* Lightest background */
--synora-gray-100: #f1f5f9;   /* Light background */
--synora-gray-200: #e2e8f0;   /* Borders, dividers */
--synora-gray-300: #cbd5e1;   /* Disabled states */
--synora-gray-400: #94a3b8;   /* Placeholders */
--synora-gray-500: #64748b;   /* Secondary text */
--synora-gray-600: #475569;   /* Body text */
--synora-gray-700: #334155;   /* Headings */
--synora-gray-800: #1e293b;   /* Dark backgrounds */
--synora-gray-900: #0f172a;   /* Darkest text */
```

### Semantic Colors
```css
--synora-success: #22c55e;    /* Success states */
--synora-warning: #eab308;    /* Warning states */
--synora-error: #ef4444;       /* Error states */
--synora-info: #3b82f6;        /* Information */
```

### Color Usage Guidelines
- **Primary Blue**: Main CTAs, links, primary actions
- **Purple**: Secondary actions, special features
- **Green**: Success states, AI features, growth indicators
- **Neutrals**: Text, backgrounds, borders
- **Semantic**: Status indicators, alerts

---

## Typography

### Font Families
```css
--font-primary: 'Inter', system-ui, -apple-system, sans-serif;
--font-mono: 'JetBrains Mono', 'Courier New', monospace;
```

### Typography Scale
| Size | Usage | Weight | Line Height |
|------|-------|--------|-------------|
| 3.75rem (60px) | Hero titles | 800 | 1 |
| 3rem (48px) | H1 | 700 | 1 |
| 2.25rem (36px) | H2 | 600 | 1.1 |
| 1.5rem (24px) | H3 | 600 | 1.2 |
| 1.25rem (20px) | H4 | 500 | 1.3 |
| 1rem (16px) | Body | 400 | 1.5 |
| 0.875rem (14px) | Small | 400 | 1.4 |
| 0.75rem (12px) | Caption | 400 | 1 |

### Typography Classes
```css
.hierarchy-primary   /* Hero titles */
.hierarchy-secondary  /* Main headings */
.hierarchy-tertiary   /* Subheadings */
.hierarchy-body      /* Body text */
.hierarchy-caption   /* Captions, small text */
```

### Font Usage Rules
- **Inter**: All UI elements, body text, headings
- **JetBrains Mono**: Code, addresses, technical data
- **Weights**: 300-900 available, use sparingly
- **Colors**: Follow hierarchy with appropriate color weights

---

## Icon System

### Icon Categories
1. **Brand Icons**: Logo variations, AI badge
2. **Payment Icons**: Cards, crypto, bank transfer
3. **Governance Icons**: Voting, proposals, treasury
4. **Security Icons**: Shield, fraud detection
5. **AI Icons**: Brain, chat, processing
6. **Analytics Icons**: Charts, portfolio
7. **Banking Icons**: Lend, borrow, stake
8. **Utility Icons**: Success, warning, error
9. **Status Icons**: Online, pending, offline

### Icon Usage
- **Size**: 16px, 20px, 24px, 32px standard sizes
- **Color**: Use brand colors appropriately
- **Style**: Consistent stroke width (2px)
- **Format**: SVG for scalability

### Icon Library
All icons are defined in `assets/icons.svg` with semantic IDs:
- `#synora-logo` - Main brand icon
- `#payment-card` - Credit card payments
- `#crypto-eth` - Ethereum/cryptocurrency
- `#governance-vote` - Voting interface
- `#security-shield` - Security features
- `#ai-brain` - AI capabilities

---

## Visual Hierarchy

### Hierarchy Principles
1. **Size**: Larger elements are more important
2. **Color**: Bright colors draw attention
3. **Contrast**: High contrast for primary elements
4. **Spacing**: More space around important elements
5. **Position**: Top-left to bottom-right reading order

### Hierarchy Implementation
```css
/* Primary - Most Important */
.hierarchy-primary {
  font-weight: 700;
  font-size: 2rem;
  color: var(--synora-gray-900);
}

/* Secondary */
.hierarchy-secondary {
  font-weight: 600;
  font-size: 1.5rem;
  color: var(--synora-gray-800);
}

/* Tertiary */
.hierarchy-tertiary {
  font-weight: 500;
  font-size: 1.25rem;
  color: var(--synora-gray-700);
}

/* Body */
.hierarchy-body {
  font-weight: 400;
  font-size: 1rem;
  color: var(--synora-gray-600);
}

/* Caption */
.hierarchy-caption {
  font-weight: 400;
  font-size: 0.875rem;
  color: var(--synora-gray-500);
}
```

---

## Component Library

### Buttons
```css
.synora-button {
  background: var(--synora-gradient);
  color: white;
  font-family: var(--font-primary);
  font-weight: 600;
  padding: 0.75rem 1.5rem;
  border-radius: 0.5rem;
  transition: all 0.3s ease;
  border: none;
  cursor: pointer;
}

.synora-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 25px rgba(59, 130, 246, 0.3);
}
```

### Cards
```css
.synora-card {
  background: white;
  border-radius: 1rem;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
  border: 1px solid var(--synora-gray-200);
  transition: all 0.3s ease;
}

.synora-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 20px 25px rgba(0, 0, 0, 0.1);
}
```

### Form Elements
```css
.synora-input {
  font-family: var(--font-primary);
  border: 1px solid var(--synora-gray-300);
  border-radius: 0.5rem;
  padding: 0.75rem;
  transition: all 0.3s ease;
}

.synora-input:focus {
  outline: none;
  border-color: var(--synora-blue);
  box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.1);
}
```

---

## Voice & Tone

### Brand Voice
- **Intelligent**: Knowledgeable and precise
- **Approachable**: Friendly and accessible
- **Confident**: Assured and professional
- **Innovative**: Forward-thinking and modern

### Tone Guidelines
- **Educational Content**: Informative, clear, helpful
- **Marketing Copy**: Energetic, inspiring, benefit-focused
- **Error Messages**: Calm, constructive, solution-oriented
- **Success Messages**: Celebratory, encouraging, clear

### Writing Style
- **Active Voice**: Use active voice predominantly
- **Simple Language**: Avoid jargon when possible
- **Inclusive**: Use gender-neutral language
- **Concise**: Get to the point efficiently

---

## Usage Guidelines

### Do's
- ✅ Use the logo as provided
- ✅ Maintain clear space around logos
- ✅ Use brand colors consistently
- ✅ Follow typography hierarchy
- ✅ Ensure accessibility (WCAG AA compliance)
- ✅ Test on all devices and screen sizes

### Don'ts
- ❌ Modify or distort the logo
- ❌ Use unapproved colors
- ❌ Mix font families arbitrarily
- ❌ Ignore visual hierarchy
- ❌ Overcrowd designs
- ❌ Break accessibility guidelines

### Brand Application Examples
1. **Website Headers**: Logo + navigation + CTA
2. **Mobile Apps**: Icon-only logo + simplified navigation
3. **Marketing Materials**: Full logo with tagline
4. **Social Media**: Icon + brand colors
5. **Documentation**: Wordmark + professional styling

### Quality Assurance
- **Color Contrast**: Minimum 4.5:1 for normal text
- **Touch Targets**: Minimum 44px for mobile
- **Loading States**: Use brand colors for loading indicators
- **Error Handling**: Consistent error styling
- **Success States**: Clear success feedback

---

## Implementation Checklist

### Design Phase
- [ ] Logo system implemented
- [ ] Color palette applied
- [ ] Typography hierarchy set
- [ ] Icon system integrated
- [ ] Component library built

### Development Phase
- [ ] CSS variables defined
- [ ] Component classes created
- [ ] Responsive design tested
- [ ] Accessibility verified
- [ ] Cross-browser compatibility checked

### Launch Phase
- [ ] Brand guide distributed
- [ ] Assets organized and shared
- [ ] Team training completed
- [ ] Quality assurance passed
- [ ] Documentation updated

---

## Contact & Resources

### Brand Assets Location
- **Logos**: `/assets/logos/`
- **Icons**: `/assets/icons.svg`
- **Colors**: CSS variables in main stylesheet
- **Typography**: Google Fonts (Inter, JetBrains Mono)

### Support
For brand-related questions or asset requests, contact the design team.

### Updates
This brand guide is updated quarterly. Last updated: February 2026.

---

*This brand guide ensures consistency across all Synora touchpoints while maintaining flexibility for innovation and growth.*
