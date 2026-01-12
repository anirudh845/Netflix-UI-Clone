# Netflix Clone - Frontend UI

A fully responsive Netflix landing page clone built with HTML, CSS, and vanilla JavaScript. This project replicates Netflix's modern interface with smooth animations, interactive components, and seamless responsiveness across all devices.

## ✨ Features

### Core Functionality
- **Hero Section**: Eye-catching background with floating label email input and call-to-action button
- **Trending Now Slider**: Horizontal scrollable movie carousel with:
  - Custom navigation arrows (left/right)
  - Auto-hide arrows at scroll boundaries
  - Large rank numbers overlaying movie posters
  - Smooth scroll behavior
- **More Reasons Section**: Feature cards with gradient backgrounds and icons
- **FAQ Accordion**: Interactive accordion with smooth expand/collapse animations and rotating icons
- **Custom Separator**: Gradient line with glowing violet effect between sections
- **Footer**: Multi-column layout with links and language selector

### Design Highlights
- Pixel-perfect recreation of Netflix's UI
- Smooth CSS transitions and animations
- Modern gradient effects and glassmorphism
- Netflix Sans font integration
- Dark theme with vibrant accent colors

## 🛠️ Tech Stack

**Frontend:**
- **HTML5** - Semantic markup with proper accessibility (ARIA attributes)
- **CSS3**:
  - Flexbox for navigation and card layouts
  - CSS Grid for footer structure
  - Custom animations using `transition`
  - Radial and linear gradients for visual effects
  - Media queries for responsive design
  - Pseudo-elements (::before, ::after) for decorative effects
- **JavaScript (ES6+)**:
  - DOM manipulation and traversal
  - Event handling (click, scroll)
  - Dynamic class toggling
  - `requestAnimationFrame` for smooth animations
  - Smooth scrolling implementation

**Assets:**
- WebP image format for optimized loading
- SVG icons for crisp, scalable graphics
- Custom Netflix Sans font via CDN

## 📱 Responsive Design

### Breakpoints
- **Desktop**: 1025px and above (5.5 posters visible)
- **Large Tablet**: 769px - 1024px (4.5 posters visible)
- **Tablet/iPad**: 481px - 768px (5.5 posters visible)
- **Mobile**: 320px - 480px (2 posters visible, arrows hidden)
- **Extra Small**: 320px - 360px (optimized for small screens)

### Responsive Features
- Email signup stacks vertically on mobile
- Movie slider adjusts poster count based on screen size
- Cards display full-width on mobile/tablet
- Navigation buttons resize appropriately
- Font sizes scale for readability

## 💡 What I Learned

### Improved CSS Skills
- **Advanced Positioning**: Better understanding of `relative`, `absolute`, and `fixed` positioning
- **Z-index Management**: Creating proper layering for overlays and interactive elements
- **Flexbox & Grid**: Building complex layouts without CSS frameworks
- **CSS Animations**: Creating smooth transitions using `transition` and `transform`
- **Pseudo-elements**: Leveraging `::before` and `::after` for decorative effects
- **Responsive Design**: Mobile-first approach with strategic breakpoints

### Improved JavaScript Skills
- **DOM Manipulation**: Efficient querying and updating of elements
- **Event Handling**: Managing multiple similar elements efficiently
- **State Management**: Tracking FAQ open/closed states and slider positions
- **Scroll Detection**: Implementing scroll-based arrow visibility
- **Animation Timing**: Coordinating CSS transitions with JavaScript using `requestAnimationFrame`

### General Learnings
- **Floating Label Animation**: Creating animated input labels without JavaScript libraries
- **Horizontal Scroll**: Building custom scrollable carousel with navigation controls
- **Accordion Logic**: Implementing smooth open/close with proper height animations
- **Browser Compatibility**: Handling webkit-specific properties (autofill, scrollbar)
- **Performance**: Optimizing animations and using WebP images for faster load times

## 🎯 Challenges Overcome

### 1. Floating Label Animation
**Challenge**: Creating a smooth label animation that moves up when the input is focused or has content.

**Solution**: Used CSS `:focus` and `:valid` pseudo-classes combined with `transition` property for smooth animation, with proper positioning using `transform`.

### 2. Movie Slider with Custom Arrows
**Challenge**: Implementing horizontal scroll with custom navigation while showing/hiding arrows at boundaries.

**Solution**: Used JavaScript to detect scroll position (`scrollLeft`, `scrollWidth`) and toggle arrow visibility dynamically. Implemented smooth scrolling with `scrollBy()` method.

### 3. FAQ Accordion Height Animation
**Challenge**: Animating height from `0` to `auto` isn't possible with CSS transitions alone.

**Solution**: Used JavaScript to calculate `scrollHeight` dynamically and animate to that specific pixel value, then set to `auto` after animation completes.

### 4. Responsive Slider
**Challenge**: Showing different numbers of posters on different screen sizes while maintaining proper arrow positioning.

**Solution**: Used `calc()` function with viewport-based calculations: `calc(5.5 * (poster-width + gap))` to show exactly 5.5 posters, adjusted per breakpoint.

### 5. Autofill Styling
**Challenge**: Browser autofill was overriding custom dark theme with white background.

**Solution**: Used `-webkit-autofill` pseudo-class with `box-shadow` inset trick and high delay transition to maintain dark theme.

## 🔮 Future Enhancements

- [ ] **User Authentication**: Sign-up/sign-in flow with form validation
- [ ] **API Integration**: Connect to TMDB API for real movie data
- [ ] **Video Player**: Implement custom video player with controls
- [ ] **Search Functionality**: Add search bar with autocomplete
- [ ] **Multiple Sliders**: Create separate sliders for different categories
- [ ] **User Profiles**: Profile selection and management interface
- [ ] **Lazy Loading**: Implement intersection observer for image optimization
- [ ] **Accessibility**: Enhanced keyboard navigation and screen reader support

## 📝 License & Disclaimer

This project is for **educational purposes only** and is not affiliated with, endorsed by, or connected to Netflix, Inc. All Netflix trademarks, logos, and brand elements are the property of Netflix, Inc.

## 👨‍💻 Author

**Anirudh Iyer**
- GitHub: [@anirudh845](https://github.com/anirudh845)
- LinkedIn: [Anirudh Iyer](https://www.linkedin.com/in/anirudh42/)

---

⭐ **If you found this project helpful or learned something from it, please give it a star!**

💬 **Questions or suggestions?** Feel free to open an issue or reach out!
