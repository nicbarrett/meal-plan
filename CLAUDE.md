# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personalized **High-Protein Meal Plan** application built as a static website for Nic & Annika's strength training goals. The project consists of 5 interconnected HTML pages that provide a complete meal planning solution.

## Architecture

The project is structured as a **multi-page static website** with consistent styling and navigation:

- **meal-plan-index.html** - Main landing page with macro targets and feature overview
- **meal-plan-page.html** - Interactive 7-day meal plan with day navigation
- **recipes-page.html** - Complete recipes and batch cooking instructions  
- **grocery-page.html** - Organized grocery shopping lists
- **fitness-page.html** - Fitness strategies and workout plans

### Key Design Patterns

- **Consistent Navigation**: All pages use the same navigation structure with active state management
- **Responsive Grid Layouts**: CSS Grid and Flexbox for mobile-friendly layouts
- **Component-Based Styling**: Reusable CSS classes for cards, sections, and interactive elements
- **JavaScript Navigation**: Simple day/section switching functionality
- **Embedded CSS**: All styles are contained within each HTML file for portability

### File Structure

```
meal-plan/
├── meal-plan-index.html     # Homepage with overview and macro targets
├── meal-plan-page.html      # 7-day meal plan with interactive navigation
├── recipes-page.html        # Batch cooking recipes and meal prep guide
├── grocery-page.html        # Shopping lists organized by store sections  
└── fitness-page.html        # Workout plans and fitness strategies
```

## Development Commands

This project uses **no build process** - it's pure HTML/CSS/JavaScript that can be opened directly in a browser.

### Viewing the Project
```bash
# Open any HTML file directly in browser
open meal-plan-index.html
# Or use a simple HTTP server
python3 -m http.server 8000
```

### No Package Management
- No package.json, npm, or build tools required
- No dependencies to install
- No linting or testing commands configured

## Content Architecture

### Navigation Flow
- Homepage introduces the meal plan concept and macro targets
- 7-day meal plan provides daily meal breakdowns with portion customization  
- Recipes section gives detailed cooking instructions for batch prep sessions
- Grocery lists organize ingredients by store sections for efficient shopping
- Fitness section provides workout splits and supplement recommendations

### Personalization Features
- **Dual-person portions**: Separate serving sizes for Nic and Annika
- **Spice customization**: Mild base recipes with spicy additions for Nic
- **Portable options**: Work-friendly snacks and meals for Annika
- **Batch cooking**: Only 2-3 cooking sessions per week
- **Protein tracking**: Each meal shows protein content

### Content Citations
All recipes and nutritional advice include citations to reputable sources like BarBend, Men's Health, Budget Bytes, and registered dietitians for evidence-based recommendations.

## Working with this Project

### Making Content Changes
- Edit HTML files directly in any text editor
- CSS is embedded in each file's `<style>` section  
- JavaScript is minimal and embedded in `<script>` tags
- Navigation links point to specific HTML files (not hash anchors)

### Maintaining Consistency
- Use the established color scheme (purple gradients: #667eea to #764ba2)
- Follow the card-based layout pattern for new sections
- Include protein content information for any new meals
- Maintain the dual-portion approach (Nic/Annika customization)
- Keep the mobile-responsive grid layouts

### Adding New Meals or Recipes
- Follow the established macro calculation approach
- Include nutrition citations when possible  
- Maintain the spice customization pattern (mild base + spicy additions)
- Update grocery lists if adding new ingredients