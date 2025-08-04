# **Opsfolio Branding Assets**

This repository contains the **official branding assets** for **Opsfolio Suite**
and its sub-products (**Surveilr, Fleetfolio, Opsfolio CaaS**). The structure is
designed to ensure **easy access for humans** and **AI-friendly ingestion**
(RAG, MCP servers, design automation).

---

## **Repository Goals**

- Centralized source for **logos, colors, typography, and templates**
- **Consistent naming and versioning** for reuse across products and campaigns
- Structured metadata (`manifest.json`) for **AI and automation workflows**
- Scalable to include **future sub-brands and campaigns**

---

## **Folder Structure**

```plaintext
/opsfolio-branding
│
├── /core                 # Primary Opsfolio Suite brand identity
│   ├── /logos            # Official logos (primary, monochrome, favicon)
│   ├── /colors           # Color palette (JSON + usage notes)
│   ├── /typography       # Fonts + guidelines
│   ├── /icons            # Icon sets (system, product-specific)
│   └── brand-guidelines.pdf
│
├── /sub-brands           # Product-specific assets
│   ├── /surveilr
│   ├── /fleetfolio
│   └── /opsfolio-caas
│
├── /templates            # Ready-to-use design templates
│   ├── /presentations
│   ├── /social-media
│   ├── /print
│   └── /email
│
├── /marketing-assets     # Campaign creatives, case studies, compliance reports
│
├── /media                # Stock/custom photography, illustrations, videos
│
└── manifest.json         # AI-readable master reference
```

---

## **Core Components**

### **1. Logos**

- **Primary**: Full-color brand logo for light backgrounds.
- **Monochrome**: Single-color variants for dark/light backgrounds.
- **Favicons**: Web usage (16x16, 32x32, etc.).

### **2. Colors**

- Stored in `core/colors/palette.json` with HEX, RGB, CMYK values and usage
  notes.
- Example snippet:

```json
[
    { "name": "Primary Blue", "hex": "#0052CC", "usage": "Buttons, headers" },
    { "name": "Neutral Gray", "hex": "#7A7A7A", "usage": "Backgrounds, text" }
]
```

### **3. Typography**

- Fonts (TTF/WOFF) with weight variations (400, 700, etc.).
- Usage rules in `typography-guidelines.pdf`.

### **4. Templates**

- Presentation decks, social media posts, email templates, print materials.
- File formats: `.pptx`, `.fig`, `.psd`, `.ai`, `.html`.

### **5. Sub-Brands**

- Dedicated folders for Surveilr, Fleetfolio, Opsfolio CaaS with their own
  logos, palettes, and icon sets.

---

## **AI Ingestion**

### **Manifest JSON**

The `manifest.json` provides:

- Paths to primary assets (logos, fonts, colors)
- Sub-brand references
- Template locations
- Versioning & description for automated pipelines

### **Usage**

- Can be ingested by **LLMs, MCP servers, or design tools** to:

  - Retrieve brand colors, logos, templates dynamically
  - Generate brand-consistent marketing copy or designs
  - Ensure compliance with brand standards in automated workflows

---

## **Naming Conventions**

- Use **lowercase and hyphen-separated** file names:
  `opsfolio-logo-primary.svg`, `linkedin-post-template.fig`
- Include **versioning** for major rebrands: `opsfolio-logo-primary-v2025.svg`

---

## **Versioning**

- Major brand updates: `vYYYY-Q#` (e.g., `v2025-Q3`)
- Campaign-specific updates: stored under `/marketing-assets/campaign-name`

---

## **Compliance & Legal**

- All assets are **copyrighted** by Opsfolio.
- Internal use only unless explicitly approved by the marketing team.
- Check `brand-guidelines.pdf` for usage permissions.

---

## **How to Add New Assets**

1. Place new files in the correct folder (core, sub-brand, template, etc.)
2. Update `manifest.json` with the new file path and metadata
3. If relevant, update `palette.json` or typography guidelines
4. Commit changes with descriptive messages (e.g., `add: Surveilr logo v2`)

---

## **Quick Links**

- [Brand Guidelines (PDF)](core/brand-guidelines.pdf)
- [Color Palette JSON](core/colors/palette.json)
- [Manifest JSON](manifest.json)

---
