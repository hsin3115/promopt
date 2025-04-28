提示詞:
You are a senior web designer and front-end engineer. From zero, generate a fully responsive, multi-page personal branding website using HTML5, Tailwind CSS (v3.x+), Font Awesome, Google Fonts (Noto Sans TC + Inter), and vanilla JavaScript only. The deliverable is four standalone .html files plus one optional custom CSS file:

- index.html (Home)
- about.html (About)
- portfolio.html (Portfolio)
- contact.html (Contact)
- (optional) styles.css for custom overrides

=== 1. Global Requirements ===
• **Responsive Design**: Desktop (grid/flex layout, multi-columns, generous whitespace) vs Mobile (single-column stack, touch-friendly spacing).  
• **Theme Toggle**: Dark/Light mode switch (persisted in localStorage).  
• **Typography**: Define base font-sizes, line-heights; `<h1> > h2 > h3 > p` hierarchy clear.  
• **Color Palette**:
  - Primary Blue: `#1E40AF`
  - Dark Gray: `#111827`
  - Light Ivory: `#F9FAFB`
  - Accent Gradient: `from-blue-700 to-blue-500`
• **Images**: Use Lorem Picsum placeholders. Backgrounds: low-opacity background images, blurred “glassmorphism” panels.  
• **Icons**: Use Font Awesome.  
• **Animations**:  
  - **Page load**: fade-in + slide-up for sections  
  - **Hover**: cards/buttons scale up `transform: scale(1.03)`, shadow intensifies  
  - **Mobile**: additional scroll-triggered parallax or reveal animations (e.g. slide from sides)  
  - **Lightbox**: portfolio items open in a modal overlay with fade-in.  
• **Accessibility**: semantic HTML, `aria` labels for menu, modal, toggle.

=== 2. Common Components ===
1. **Header**: fixed at top, logo/title left, nav right.  
   - Desktop: inline links.  
   - Mobile: hamburger icon toggles slide-in nav drawer.  
2. **Footer**: centered text, “© 2025 Your Name”, theme toggle button.  
3. **Back-to-Top**: bottom-right floating button appears after scroll.

=== 3. index.html (Home) ===
1. **Hero**: full-viewport, background image (blurred + dark overlay), centered avatar (circular), name, tagline, call-to-action button (scroll to portfolio).  
2. **About Preview**: card with short intro + “Read More” link.  
3. **Skills**: 4–6 skill cards in grid, each with icon + title + progress bar (animated width).  
4. **Portfolio Preview**: 3 sample portfolio cards with image + title + hover lift + “View More” link to portfolio.html.  
5. **CTA**: full-width section with gradient background, invitation to contact.

=== 4. about.html (About) ===
1. **Introduction**: two-column on desktop (text + image), single-column on mobile.  
2. **Timeline**: vertical timeline of education & work—icons on left, text on right.  
3. **Skills Detail**: horizontal progress bars with labels + percentage (animated on scroll).  
4. **Back to Home** button.

=== 5. portfolio.html (Portfolio) ===
1. **Gallery Grid**: responsive grid of 6–8 projects; each tile is an image with overlay title.  
2. **Lightbox Modal**: click tile to open full-size image + description + next/prev buttons.  
3. **Load More** button (pure front-end stub).  
4. **Scroll animations**: staggered fade-in on viewport entry.

=== 6. contact.html (Contact) ===
1. **Contact Form**: fields (Name, Email, Subject, Message) with floating labels effect.  
2. **Submit**: on submit prevent default + show custom toast notification (“Thank you for your message!”).  
3. **Map Embed Placeholder**: static image or blank box.  
4. **Quick Links**: buttons to Home, About, Portfolio.

=== 7. Technical Details ===
• Use Tailwind utility classes (`container`, `grid`, `flex`, `gap`, `space`, `max-w`, `min-h-screen`).  
• For custom effects, include `<link rel="stylesheet" href="styles.css">` or `<style>` block.  
• Include Font Awesome CDN and Google Fonts in `<head>`.  
• Write clear comments in HTML/CSS/JS.  
• Scripts at bottom: theme toggle, mobile menu toggle, scroll animations, lightbox logic.

=== 8. Folder Structure Suggestion ===
