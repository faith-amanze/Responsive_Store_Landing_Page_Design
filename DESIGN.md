# Northwind Goods: Responsive Store Landing Page

## Files
- `index.html`: page structure (header, hero, features, product section, footer)
- `styles.css`: custom styles and media queries
- `screenshots/`: desktop, mobile, and mobile menu open

## Design choices
1. **Store concept.** Northwind is a small online store for everyday-carry gear (bags, audio, desk items). A single clear theme keeps the placeholder content believable.
2. **Colour palette.** Near-black navy for text and the footer, one bright blue for every call-to-action button, and a very light grey-blue for the hero background. Using one accent colour makes the "Shop Now" buttons the first thing the eye finds.
3. **Typography.** Poppins in several weights: heavy and tightly spaced for headlines, regular for body text, so the hierarchy is clear without extra decoration.
4. **Layout.** A sticky header keeps navigation within reach. The hero puts the message and buttons beside a product image. A short strip of store promises (shipping, returns, warranty) builds trust before the products. Four product cards follow, then a dark footer that anchors the page.
5. **Product cards.** Each card has an image, name, short description, price and a "Shop Now" button. Prices and buttons are pinned to the bottom of each card, so all cards line up even when the text lengths differ. Cards lift slightly on hover.
6. **Responsive design.**
   - Bootstrap's grid shows the products in 4 columns on desktop, 2 on tablets and 1 on phones.
   - The navigation collapses into a menu button under 768px.
   - Media queries in `styles.css` (992px, 768px and 576px) reduce heading sizes and section spacing and center the footer on smaller screens.
   - Long text such as the email address wraps so the page never scrolls sideways on a phone.
7. **CSS framework (extra points).** Bootstrap 5 provides the grid, navbar, cards, badges and buttons, and Bootstrap Icons provides the icons. Custom CSS is loaded after Bootstrap to apply the brand colours and spacing.
8. **Accessibility.** Images have alt text, buttons and links have a visible keyboard focus outline, social icons have labels, and animation is turned off for users who prefer reduced motion.
9. **Code quality.** Colours and radius are CSS variables in one place, class names describe their purpose, and every section of the HTML and CSS has a comment.

## Notes
- Product images are placeholders from placehold.co. Replace the `src` of each image with real photos.
- Bootstrap, the icons and the font load from a CDN, so an internet connection is needed to see the page as designed.
