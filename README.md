# Business Class TV 📺 — Custom WordPress Theme

A premium, bespoke WordPress theme engineered from the ground up for **Business Class TV**. This platform is designed to serve as a high-end digital editorial spread and video streaming vault, completely bypassing bloated commercial themes in favor of raw performance and strict design constraints.

This repository represents the core codebase for the STI College Ortigas-Cainta capstone project, delivering a production-ready, client-manageable media network.

## 🏗️ Architecture & Stack

This is a monolithic, custom WordPress build deployed to standard shared hosting. It prioritizes a seamless client backend experience with a highly constrained, premium frontend UI.

* **Core:** WordPress (PHP / MySQL)
* **Styling:** Custom CSS / Tailwind CSS (Strictly adhered to the Brand Blueprint)
* **Interactions:** Vanilla JavaScript
* **Content Management:** Native WP Post types (Articles) + Custom Post Types (Video Vault)

## 🎨 The Brand Blueprint (Design System)

**Any PRs that deviate from this design system will be rejected.** This platform relies on a strict "old money," editorial aesthetic. Precision is non-negotiable.

### Color Palette
* **Midnight Navy (`#0B132B`):** Primary dark backgrounds (Hero, Footer), primary text on light backgrounds.
* **Alabaster/Ivory (`#F8F9FA`):** Primary light backgrounds, primary text on dark backgrounds. NEVER use pure white (`#FFFFFF`).
* **Muted Champagne (`#C5A880`):** Primary accent (Buttons, category tags, pull quotes). 

### Typography
* **Primary Headings:** `Playfair Display` (Authority, editorial covers, massive typography).
* **Body & UI:** `Montserrat` (Clean legibility, navigation, dates, small tags).

### Global UI Rules
* **Razor Edges:** `0px` border radius globally. No rounded corners on any image, button, or container.
* **Reading Tunnel:** Article body text must never exceed `700px` in width and must be strictly left-aligned. Center-aligned body text is prohibited.
* **Image Treatment:** All featured images and video thumbnails require a CSS filter or pre-processed `-15` saturation and `+10` contrast for a unified studio aesthetic.

## 📂 File Structure

This theme avoids the bloat of standard WordPress themes. The architecture is lean and mapped directly to the primary user flows:

* `front-page.php` - The main entry point (Cinematic Hero + Grid loops)
* `archive.php` - The digital library (Vanguard article feature + 3-column loops)
* `single.php` - The immersive reading experience (700px reading column constraint)
* `archive-video.php` - The Screening Room (Custom Post Type loop for video content)
* `template-parts/` - Reusable UI components (Article cards, Video thumbnails) to maintain DRY code.

## 🚀 Local Development Setup

1.  Clone this repository into your local WordPress installation's theme folder: `wp-content/themes/business-class-tv/`
2.  Activate the theme in the WordPress Appearance dashboard.
3.  Ensure the "Videos" Custom Post Type plugin/functions are active to populate the Screening Room.
4.  Commit all CSS and template changes to a new branch before submitting a PR.
