# Kora Goods: Responsive Store Landing Page

**Live demo:** https://faith-amanze.github.io/Responsive_Store_Landing_Page_Design/

A responsive landing page for a small online store selling handmade bags, ceramics, candles and baskets.
Built with HTML, custom CSS and Bootstrap 5.

## Screenshots (live page)
| Desktop (1440px) | Tablet (768px) |
|---|---|
| ![Desktop](Screenshots/desktop-1440-full.png) | ![Tablet](Screenshots/tablet-768-full.png) |

| Mobile (390px) | Mobile menu open |
|---|---|
| ![Mobile](Screenshots/mobile-390-full.png) | ![Mobile menu](Screenshots/mobile-390-menu-open.png) |

## Files
- `index.html`: page structure (header, hero, product section, about strip, footer)
- `styles.css`: all custom styling, commented by section
- `images/`: four product photos (JPG, cropped square and compressed)
- `Screenshots/`: desktop (1440px), tablet (768px), mobile (390px, plus menu open)

To run it locally, open `index.html` in a browser. Bootstrap loads from a CDN, so an internet connection is needed.

## Design choices
**Concept.** A small store for handmade bags, ceramics, candles and baskets. Picking a real subject gave me
believable copy, prices (in naira) and product imagery instead of generic placeholders.

**Colour.** Three working colours: deep navy for text and dark surfaces, cobalt for primary actions and the
about band, and marigold as the only warm accent (hover states, footer logo). A cool grey-blue page background
keeps the white product section distinct. All colours are CSS variables at the top of `styles.css`.

**Typography.** A system font stack (fast, no external requests) with tight letter-spacing and heavy weights
on headings. Heading sizes use `clamp()` so they scale smoothly instead of jumping at breakpoints.

**Layout.** The hero's overlapping tilted photos are the one memorable element; everything else stays quiet.
Product cards use flexbox so descriptions of different lengths still leave every "Shop Now" button aligned.

**Responsive strategy (mobile-first).**
- Products: 1 column on phones, 2 on tablets (`sm`), 4 on desktop (`xl`), via Bootstrap's `row-cols-*`.
- Navigation collapses into a hamburger menu below 768px.
- Section spacing is fluid (`clamp()`), so it tightens on small screens.
- Custom media queries adjust hero text size, card padding and hero image alignment.
- Checked at 1440, 768 and 390px with no horizontal scrolling.

**Images.** Photos are cropped square to match the cards (`object-fit: cover`), compressed to under 100 KB each,
and lazy-loaded below the hero. Every image has alt text describing what it shows.

**Library (extra points).** Bootstrap 5.3 provides the grid, collapsing navbar and button base. Custom CSS loads
after it and restyles components so the page doesn't look like default Bootstrap. The Bootstrap files use
Subresource Integrity hashes.

**Accessibility.** Skip link, visible focus outlines, alt text on every image, semantic landmarks
(`header`, `main`, `footer`), labelled nav, and reduced-motion support.

## Image sources
These photos are used as placeholder images for a coursework project. I am not the photographer of any of them,
and all rights remain with the original owners. The sources below are the ones I could trace; where I say
"similar listing", the exact original page is not confirmed.

- **Candle** (`images/candle.jpg`): photo from
  [Mason Jar Candle Ideas using Ylang Ylang Scent](https://confessionsofanover-workedmom.com/mason-jar-candle-ideas/)
  by Ellen Christian, Confessions of an Overworked Mom.
- **Woven baskets** (`images/basket.jpg`): similar product listings on
  [Temu](https://www.temu.com/bh/2-woven-baskets-with-handles-festive-decorations-creative-wedding-full-gifts-souvenir-baskets-valentines-day-packaging-baskets-woven-bags-shelf-baskets-home-kitchen-supplies-courtyard-flower-arrangement-baskets-wedding-party-g-606045602686963.html),
  [SHEIN](https://eur.shein.com/1pc-Woven-Basket-With-Handle-Multipurpose-Storage-Box-Suitable-For-Home-Decor-Wedding-Favors-And-Gift-Packaging-Baby-Shower-Gifts-Souvenir-Baskets-Wooden-Gift-Baskets-Packaging-Baskets-Storage-Baskets-Creative-Gift-Display-p-313280823.html),
  [Snoonu](https://snoonu.com/product/wooden-gift-baskets/6980c989b90390da6a023496) and
  [AliExpress](https://www.aliexpress.com/item/1005009149971647.html).
- **Cup and saucer** (`images/mug.jpg`): similar vintage stoneware listings on
  [eBay Germany](https://www.ebay.de/itm/387626352448) and
  [Tradera](https://www.tradera.com/da/item/201105/752337767/kaffe-te-koppar-nittsjo-11-delar).
- **Tote bag** (`images/tote.jpg`): similar product listings on
  [IndiaMART](https://www.indiamart.com/proddetail/pu-leather-tote-bags-2855568264491.html) and
  [Jumia Nigeria](https://www.jumia.com.ng/fashion-simple-elegant-large-capacity-pu-leather-tote-handbag-women-office-large-capacity-quality-shoulder-handbag-customized-new-ladies-bag-designer-bag-luxury-lady-handbag-pu-leather-women-handbags-tote-bag-419316438.html).

The product names, descriptions and prices on the page are made up for this exercise. Replace these photos with
licensed or original images before using the design for anything beyond coursework.
