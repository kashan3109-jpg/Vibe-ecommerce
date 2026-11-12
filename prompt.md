MASTER WEBSITE BUILD PROMPT — NOWHERE®

Premium 3D Fashion E-Commerce Experience

Brand tagline: Stay out of the loop.

Act as a senior creative frontend developer, 3D web designer, UI/UX architect, and e-commerce engineer.

Build a complete, production-quality, premium fashion e-commerce website for the fictional fashion label NOWHERE®.

This must NOT be just a landing page, static design, or animated lookbook. It must be a complete shopping website with a sophisticated 3D fashion lookbook as its signature homepage experience.

The entire website must feel like a luxury fashion editorial combined with an interactive modern shopping experience.

Main creative direction: A quiet, minimal, monochrome fashion studio with immersive 3D motion, floating fashion models, smooth transitions, elegant typography, and functional shopping features.

---

1. NON-NEGOTIABLE DESIGN DIRECTION

Preserve the original Maju Store® visual identity.

Background and colours

Use the following design tokens throughout the website:

- Studio background: "#ececec"
- Paper / cards: "#ffffff"
- Main text: "#000000"
- Muted text: "#6f6f6f"
- Main border: "#000000"
- Primary buttons: black background with white text
- Secondary buttons: white background with dashed black border.

Do not change the original light-grey studio background into a dark website.

The website must maintain a consistent grayscale identity across every page.

Use subtle shadows, realistic depth, soft lighting, transparent model cut-outs, and delicate gradients. Do not introduce unnecessary colours.

Visual language

- Minimal luxury fashion aesthetic.
- Editorial magazine-style layouts.
- Large negative spaces.
- Thin black outlines.
- Dashed rounded pills.
- Oversized editorial typography.
- High-quality product imagery.
- Sophisticated motion and transitions.
- Premium fashion brand presentation.

Avoid:

- Generic e-commerce templates.
- Colourful gradients.
- Excessive rounded cards.
- Unnecessary decorative elements.
- Excessive white sections that break the grey studio identity.
- Cartoonish animations.
- Cheap-looking 3D effects.

---

2. TECHNICAL REQUIREMENTS

Build the website using:

- HTML5
- CSS3
- Vanilla JavaScript
- CSS 3D transforms
- Web Animations API
- Canvas or lightweight native WebGL where genuinely useful.

Use a single self-contained HTML file with inline CSS and one inline IIFE JavaScript script.

No React, Vue, Angular, Bootstrap, Tailwind, or other frameworks.

No build step.

All navigation and interactions must work inside the single-page application.

Use localStorage for persistent cart and shopping state.

Use semantic HTML, accessible controls, keyboard navigation, and responsive layouts.

Do not create fake buttons or non-functional links.

If actual payment credentials or backend APIs are unavailable, implement a working demo checkout and clearly separate demo functionality from real payment processing. Never claim that an actual payment has been processed when it has not.

---

3. TYPOGRAPHY

Use embedded WOFF2 fonts.

Inter Tight

- Variable Roman: weight 300–400.
- Italic: weight 300.
- Used throughout the website.

Instrument Serif

- Latin subset.
- Weight 400.
- Used ONLY for the main centred homepage title: "Stay out of the loop".

Use the provided real WOFF2 font files encoded as base64 data URIs in "@font-face". Do not invent or fabricate base64 font data.

If the font binaries are unavailable, use an appropriate local fallback until real font files are supplied.

Global typography:

- Smooth antialiasing.
- Minimal letter spacing.
- Uppercase micro-labels.
- Tabular numerals.
- Italic Inter Tight for prices and editorial emphasis.

---

4. COMPLETE WEBSITE STRUCTURE

Build the following complete shopping experience.

A. HOMEPAGE — MAIN 3D EXPERIENCE

The homepage must immediately introduce the NOWHERE® brand.

Header / status bar

Create a floating status bar at the top.

Left:

- Live local clock.
- Signal indicator.
- Low signal text.

Centre:

- NOWHERE® logo.

Right:

- Battery indicator.
- Shopping bag button with live item count.

Maintain the original 48px desktop height and 64px mobile height.

The bag counter must update immediately whenever a product is added.

Main hero: circular fashion lookbook

This is the most important part of the entire website.

Recreate the original circular fashion lookbook with nine transparent PNG model cut-outs.

Nine fashion models must stand upright around a large elliptical ring, like a clock face viewed from above.

The ring must rotate smoothly.

The nearest model at the bottom of the circle becomes the active look.

The centre must contain:

Stay out of the loop

Below:

VOL. 01 — NINE LOOKS FOR GOING QUIET.

Add a subtle dashed ellipse around the circular model arrangement.

3D motion requirements

Implement the following animations:

1. Continuous spring-based circular rotation.
2. Perspective depth scaling.
3. Front model enlargement.
4. Back model reduction.
5. Depth-based blur.
6. Smooth opacity transitions.
7. Model movement based on the circular position.
8. Mouse drag rotation.
9. Touch drag rotation.
10. Arrow-key navigation.
11. Smooth inertia after dragging.
12. Critically damped spring movement.
13. Smooth model focus transitions.
14. Subtle parallax movement based on mouse position.
15. A soft studio lighting effect.
16. Subtle glint sweep across the ring.
17. Model hover depth effects.

The animation should feel like a premium interactive 3D installation.

Do not use a basic CSS rotating image animation as a replacement for the actual circular positioning system.

Use real calculated positioning with "sin()", "cos()", depth, scale, and perspective.

Keep the original ring positioning mathematics from the supplied specification.

Homepage controls

Left:

- Vertical Looks pill.
- Opens the complete looks drawer.

Right:

- Vertical Ring / Grid toggle.

Bottom dock:

- Active look counter, e.g. "01 / 09".
- Autoplay control.
- Current look name.
- Three item preview pills.
- Shop this fit button.

The active look and its product details must update together.

Grid mode

When Grid is selected:

- Transform the nine circular models into a clean 3×3 editorial grid.
- Use the same model cut-outs.
- Maintain consistent image sizing.
- Add smooth layout morphing.
- Add hover opacity effects.
- Show look numbers and names.
- Clicking any model opens its look detail.

Switching back to Ring must smoothly restore the original circular arrangement.

Use the specified "--morph" curve for the Ring/Grid transition.

---

5. LOOKBOOK DATA — EXACT CONTENT

Use the nine supplied model cut-outs in this order.

No.| Look name| Foot offset
01| Somewhere Else| .0501
02| Dial-Up| .0501
03| Long Walks| .0656
04| Low Battery| .0582
05| No Reply| .065
06| Analog| .047
07| Rewind| .0377
08| Out Of Office| .0891
09| Paper Maps| .0588

Shop-dot coordinates

Coordinates are "[left%, top%]" of the model figure.

Look| Dot 01| Dot 02| Dot 03
01| 52,44| 80,40| 44,57
02| 76,45| 54,68| 45,87
03| 66,47| 51,64| 48,87
04| 76,47| 43,70| 54,88
05| 72,41| 51,68| 45,89
06| 75,45| 51,70| 46,88
07| 69,43| 51,72| 56,92
08| 65,47| 43,68| 60,86
09| 66,41| 48,72| 56,88

Use these exact coordinates for the three shopping dots on each model.

---

6. MODEL AND PRODUCT IMAGE ASSETS

Use this exact image CDN base:

"https://d8j0ntlcm91z4.cloudfront.net/user_38xzZboKViGWJOttwIXH07lWA1P/"

Every image must pass through this image wrapper:

"px(file, w) = https://images.higgs.ai/?default=1&output=webp&url=ENCODED_CDN_IMAGE_URL&w=WIDTH&q=85"

Do not introduce other image hosts.

Nine model cut-outs

1. "hf_20261108_190717_6580d844-f3b0-4240-8b4a-239355685fc9.png"

2. "hf_20261111_034030_a9171bb1-0b34-4468-9a9e-f451d79b8429.png"

3. "hf_20261111_034045_5a78f1ff-8dea-4054-85bc-60a28a4cc434.png"

4. "hf_20261111_034059_24eecc7c-e8b7-4b9c-b58c-b862b1261e87.png"

5. "hf_20261111_034112_5aa3a76f-7e92-48bb-b93d-ec3a35be2494.png"

6. "hf_20261111_034123_ce28dc23-bd91-40ba-95e6-7a09442a865f.png"

7. "hf_20261111_034137_abed307a-bcb4-4192-82e9-6ec122a80820.png"

8. "hf_20261111_034150_fc1776ff-a8d6-4060-a8af-1afedfdfc563.png"

9. "hf_20261111_034202_62b7ffb7-14f5-4dfc-87fe-83c6d9ee6134.png"

For each model:

- Main image width: 914px.
- Small image width: 571px.
- Transparent PNG cut-outs.
- Object-fit: contain.
- Object-position: 50% 100%.
- Preserve the original aspect ratio.
- Apply the individual foot offset.

Product contact sheets

Use these exact three sheets:

1. "hf_20261108_190756_3f427fdd-ba34-433e-bc55-eb9b03d2e1c6.png"

2. "hf_20261108_190758_785127d3-ef7d-4831-976b-14540a7188aa.png"

3. "hf_20261108_190800_4db1daba-ebb1-436f-857a-91dfab40f4b7.png"

Load each sheet through "px(file, 600)".

Each sheet contains a 3×3 product grid:

- Row = look position within its group of three.
- Column = item number (0, 1, 2).
- Sheet index = "floor((lookNumber - 1) / 3)".
- Row index = "(lookNumber - 1) % 3".

Use background-size "300% 300%".

Use exact background positions of 0%, 50%, and 100%.

Do not generate unrelated replacement product thumbnails when the supplied contact sheets are available.

---

7. COMPLETE PRODUCT CATALOGUE

Every look contains exactly three products.

Use the following data exactly.

LOOK 01 — SOMEWHERE ELSE

1. Ribbed Tank Top — Top — $36 — S, M, L, XL.
2. Striped Open Shirt — Top — $74 — S, M, L, XL.
3. Braided Belt — Accessory — $32 — One size.

Subtotal: $142
Whole fit −10%: −$14.20
Total: $127.80.

LOOK 02 — DIAL-UP

1. Corduroy Trucker — Outerwear — $142 — S, M, L, XL.
2. Pleated Shorts — Bottom — $64 — S, M, L, XL.
3. Suede Moccasin — Shoes — $118 — 40, 41, 42, 43, 44, 45.

Subtotal: $324
Whole fit −10%: −$32.40
Total: $291.60.

LOOK 03 — LONG WALKS

1. Polar Fleece Zip — Top — $92 — S, M, L, XL.
2. Nylon Hike Shorts — Bottom — $58 — S, M, L, XL.
3. Mesh Trainers — Shoes — $124 — 40, 41, 42, 43, 44, 45.

Subtotal: $274
Whole fit −10%: −$27.40
Total: $246.60.

LOOK 04 — LOW BATTERY

1. Yellow Anorak Shell — Outerwear — $128 — S, M, L, XL.
2. Fleece Joggers — Bottom — $72 — S, M, L, XL.
3. Chunky Sandals — Shoes — $84 — 40, 41, 42, 43, 44, 45.

Subtotal: $284
Whole fit −10%: −$28.40
Total: $255.60.

LOOK 05 — NO REPLY

1. Navy Rollneck Knit — Top — $118 — S, M, L, XL.
2. Wool Trousers — Bottom — $106 — S, M, L, XL.
3. Leather Mary Janes — Shoes — $134 — 40, 41, 42, 43, 44, 45.

Subtotal: $358
Whole fit −10%: −$35.80
Total: $322.20.

LOOK 06 — ANALOG

1. Corduroy Blazer — Outerwear — $156 — S, M, L, XL.
2. Black Slim Jeans — Bottom — $98 — S, M, L, XL.
3. Desert Boots — Shoes — $146 — 40, 41, 42, 43, 44, 45.

Subtotal: $400
Whole fit −10%: −$40
Total: $360.

LOOK 07 — REWIND

1. Faded Black Hoodie — Top — $86 — S, M, L, XL.
2. Carpenter Trousers — Bottom — $94 — S, M, L, XL.
3. Retro Court Sneaker — Shoes — $116 — 40, 41, 42, 43, 44, 45.

Subtotal: $296
Whole fit −10%: −$29.60
Total: $266.40.

LOOK 08 — OUT OF OFFICE

1. Linen Camp Shirt — Top — $76 — S, M, L, XL.
2. Pleated Bermuda — Bottom — $68 — S, M, L, XL.
3. Leather Slides — Shoes — $62 — 40, 41, 42, 43, 44, 45.

Subtotal: $206
Whole fit −10%: −$20.60
Total: $185.40.

LOOK 09 — PAPER MAPS

1. Rugby Top — Top — $88 — S, M, L, XL.
2. Tapered Khakis — Bottom — $84 — S, M, L, XL.
3. Suede Low-Tops — Shoes — $122 — 40, 41, 42, 43, 44, 45.

Subtotal: $294
Whole fit −10%: −$29.40
Total: $264.60.

Use the exact prices and item names everywhere: homepage, product detail, look drawer, receipt, bag and checkout.

Format money using:

- Whole numbers without decimals.
- Fractional amounts with two decimal places.
- True minus character "−" for discounts.

---

8. LOOK DETAILS — INTERACTIVE 3D FOCUS MODE

When the customer clicks a model, a product dot, or "Shop this fit":

Open a full-screen focus experience.

Model transition

Use FLIP animation:

- Capture the model's original bounding rectangle.
- Move the selected look into the focus viewer.
- Animate translation, scale, and position.
- Preserve the model image without distortion.
- Use a smooth premium transition.
- Return it to its original position when closing.

The selected model should appear much larger and centred.

Add three numbered shop dots at the exact coordinates from the lookbook data.

Shopping dots

Each dot:

- Displays its product number.
- Has a dashed circular outline.
- Turns black on hover.
- Uses a subtle spring scale animation.
- Shows a small tooltip with the item name and price.
- Opens the corresponding product detail when clicked.

The active item name should appear in italic Inter Tight.

---

9. RECEIPT-STYLE SHOPPING SLIP

Opening a look must also reveal a receipt-style panel.

Desktop:

- Width: 336px.
- Right-side position.
- Rounded left edge: 24px.
- White paper background.
- Black typography.
- Layer above the status bar.
- z-index: 70.

Drawer z-index: 80.

The receipt should print down from the top edge with a smooth vertical animation.

Receipt content

Header:
NOWHERE®
LOOK RECEIPT
VOL. 01.

Show:

- Look number.
- Look name.
- Three products.
- Product name.
- Category.
- Price.
- Size selector.
- Add button.

Receipt calculations:

- Subtotal.
- Whole fit −10%.
- Total.

Include a clear close control.

Size selector

For clothing:
S / M / L / XL.

For shoes:
40 / 41 / 42 / 43 / 44 / 45.

For one-size products:
One size.

The user must select a size before adding the product.

Show a selected-size state with a solid black pill.

Add to bag

When Add is clicked:

1. Validate the size.
2. Add the correct product and size.
3. Update bag count.
4. Animate the tally.
5. Show a small confirmation toast.
6. Preserve cart data in localStorage.

Do not add products with missing sizes.

---

10. COMPLETE E-COMMERCE PAGES

The website must include all of these functional shopping destinations.

PAGE 01 — HOME

- Premium 3D lookbook.
- Rotating nine-model circle.
- Ring/Grid control.
- Looks drawer.
- Focus mode.
- Shopping slip.
- Product dots.
- Shop this fit.
- Featured collection preview.
- Editorial introduction.
- New arrivals preview.
- Footer.

Keep the original 3D lookbook as the visual centrepiece.

PAGE 02 — SHOP ALL

Create a complete product catalogue page.

Include:

- Page heading: SHOP ALL.
- Short editorial introduction.
- Product count.
- Responsive product grid.
- Product image.
- Product name.
- Product category.
- Price.
- Quick add.
- View product.
- Sorting options.
- Category filters.

Filters:

- All.
- Tops.
- Bottoms.
- Outerwear.
- Shoes.
- Accessories.

Sorting:

- Featured.
- Price: Low to High.
- Price: High to Low.
- Alphabetical.

Use the 27 supplied products as the catalogue source.

Clicking a product opens its detail page.

PAGE 03 — COLLECTIONS

Create an editorial collection page with:

- Vol. 01 — Going Quiet.
- Nine looks.
- Nine model cut-outs.
- Look name and number.
- Three products per look.
- Shop complete look action.

The design must feel like a premium fashion magazine rather than a standard product listing.

PAGE 04 — PRODUCT DETAIL

Every product must have its own functional detail view.

Include:

- Large product image using the correct contact-sheet crop.
- Product name.
- Category.
- Exact price.
- Product number.
- Size selector.
- Quantity selector.
- Add to bag button.
- Product information.
- Shipping information.
- Return information.
- Related products.
- Back to shop.

The selected size and quantity must be reflected correctly in the cart.

Do not invent product specifications, material descriptions, or stock levels. Only display verified supplied information.

PAGE 05 — SHOPPING BAG

Create a premium shopping bag page or side drawer.

Include:

- Added products.
- Product thumbnail.
- Product name.
- Selected size.
- Quantity.
- Unit price.
- Line total.
- Remove product.
- Increase/decrease quantity.
- Subtotal.
- Discount, when applicable.
- Final total.
- Continue shopping.
- Proceed to checkout.

Cart must persist after refresh.

Whole-look discount

When a complete three-item look is purchased together, calculate the 10% whole-fit discount.

Apply the discount only once per qualifying complete look.

Do not accidentally apply the discount to unrelated products or multiple times.

Show the discount clearly in the receipt and bag.

PAGE 06 — CHECKOUT

Build a complete checkout interface.

Include:

Customer details:

- Full name.
- Email.
- Phone.

Delivery:

- Address.
- City.
- Postal code.
- Country.

Order summary:

- Products.
- Sizes.
- Quantities.
- Subtotal.
- Discount.
- Total.

Payment options:

- Cash on Delivery.
- Online payment placeholder, clearly marked as requiring payment integration.

Add:

- Form validation.
- Required-field messages.
- Order confirmation screen.
- Order reference generated for the demo.
- Empty-cart protection.

Do not claim a successful real-world transaction without an actual payment provider.

PAGE 07 — SEARCH

Add a working search interface.

Search products by:

- Name.
- Category.
- Look name.

Display matching products and a clear empty state.

PAGE 08 — ABOUT NOWHERE

Create a minimal editorial brand page.

Brand heading:

NOWHERE®

Tagline:

Stay out of the loop.

Description:

Vol. 01. Nine looks for going quiet.

Use restrained editorial typography, spacious layouts, grayscale visuals, and subtle scroll animations.

Do not invent company history, founder details, sustainability claims, or manufacturing facts.

---

11. NAVIGATION SYSTEM

Build a consistent navigation experience.

The main navigation should contain:

- Home
- Shop
- Collections
- About
- Search
- Bag

Use a minimal navigation drawer on mobile.

Navigation must work without a full page reload.

Use browser history correctly so Back and Forward navigation work.

Maintain the same visual identity between all pages.

---

12. 3D ANIMATION SYSTEM — IMPORTANT

This is a major requirement, not an optional decoration.

The website must feel interactive and dimensional.

A. Homepage 3D ring

Use actual trigonometric positioning:

- "STEP = 2π / 9".
- Position controlled by continuous spring variable.
- Elliptical X/Y positioning.
- Depth-based scale.
- Front-model enlargement.
- Back-model reduction.
- Depth-based blur.
- Dynamic z-index.

Preserve the original supplied ring layout mathematics.

B. 3D model interaction

- Mouse-based subtle parallax.
- Touch-friendly interaction.
- Smooth spring rotation.
- Model hover lift.
- Smooth FLIP transitions.
- Depth-aware shadows.
- Soft ambient lighting.

C. Product card animation

On hover:

- Product image gently moves forward.
- Image scale increases slightly.
- Shadow changes subtly.
- Product information moves upward by a few pixels.
- Quick add control appears smoothly.

On mobile, use tap interactions instead of hover-only controls.

D. Scroll animation

As the customer scrolls:

- Editorial text fades into view.
- Product images reveal gradually.
- Collection cards enter with staggered movement.
- Background remains consistent.
- Subtle parallax adds depth.
- Section transitions feel cinematic.

Use IntersectionObserver for scroll-triggered animations.

E. Button interactions

Every primary button must have:

- Hover state.
- Press state.
- Smooth transition.
- Arrow movement where appropriate.
- Clear keyboard focus state.

Use the supplied spring curve for playful micro-interactions and the soft ease-out curve for most transitions.

F. Performance

- Use requestAnimationFrame for the ring animation.
- Avoid unnecessary DOM updates.
- Use ResizeObserver for layout measurements.
- Pause or reduce expensive motion when the page is hidden.
- Respect "prefers-reduced-motion".
- Do not create animation loops that continue unnecessarily.
- Avoid excessive blur and large GPU-heavy effects.

The 3D animations must remain smooth on ordinary mobile devices.

---
13. DESIGN SYSTEM AND UI COMPONENTS

Use consistent reusable CSS classes.

Main pill

- Inline-flex.
- Centre aligned.
- Minimum height: 36px.
- Horizontal padding: 16px.
- White background.
- 1px dashed black border.
- Fully rounded.
- Uppercase 12px typography.
- On hover: black background, white text, solid border.

Buttons

Primary:

- Black background.
- White text.
- Rounded pill shape.

Secondary:

- White background.
- Dashed black border.

Disabled:

- Reduced opacity.
- No pointer interaction.

Product cards

- Clean studio-grey background.
- Product imagery on a light neutral surface.
- Small uppercase category.
- Product name.
- Italic price.
- Minimal product controls.

Receipt

- White background.
- Thin black separators.
- Monospaced-looking receipt layout is NOT required; use Inter Tight.
- Strong price hierarchy.
- Dashed separators.
- Print-down entrance animation.

---

14. RESPONSIVE DESIGN

The website must work professionally at:

- Large desktop: 1440px and above.
- Standard desktop: 1024px–1439px.
- Tablet: 810px–1023px.
- Mobile: 375px–809px.

Desktop

- Full circular 3D experience.
- Floating navigation.
- Side receipt.
- Large product grid.
- Spacious editorial layout.

Tablet

- Scale the circular arrangement.
- Preserve all nine models.
- Adapt receipt positioning.
- Reduce unnecessary visual spacing.

Mobile

- Status bar height: 64px.
- Hide battery and Low signal text.
- Compact bag button.
- Ring must remain usable.
- Touch drag must work.
- Look drawer becomes a mobile-friendly panel.
- Receipt becomes a full-width or near-full-width overlay.
- Product grids use two columns where space permits.
- All buttons must have comfortable touch targets.
- No horizontal overflow.
- Avoid text clipping.
- Preserve image proportions.

Do not simply shrink the desktop layout. Create an intentional mobile experience.

---

15. ACCESSIBILITY AND INTERACTION

Implement:

- Semantic buttons and links.
- Keyboard-accessible controls.
- Focus-visible rings.
- ARIA labels.
- Live announcements when the active look changes.
- Escape key to close overlays.
- Arrow keys to rotate the ring.
- Enter to open the active look.
- Proper modal focus management.
- Alt text for model and product images.
- Reduced-motion support.

The stage must have:

- "role="region"".
- "aria-roledescription="carousel"" in Ring mode.
- "aria-roledescription="grid of looks"" in Grid mode.

---

16. ORIGINAL STATUS BAR DETAILS

Preserve the original status bar behaviour:

- Clock initially displays "06:00", then switches to live local time.
- Re-tick exactly at the next minute boundary.
- Four signal bars with heights 4px, 6px, 9px, and 12px.
- All bars grey at 20% opacity.
- Text: Low signal.
- Centre logo: NOWHERE®.
- Battery: 12%.
- Bag button: Bag (0).
- Bag count animates upward on every addition.

---

17. PERFORMANCE AND ERROR HANDLING

The website must be fully functional, not just visually complete.

Implement:

- Image lazy loading except the first hero model.
- Correct image decoding.
- Image fallbacks if CDN images fail.
- Safe localStorage parsing.
- Cart persistence.
- Empty cart state.
- Invalid size prevention.
- Quantity validation.
- Search empty state.
- Product-not-found state.
- Checkout form validation.
- Responsive resize handling.
- Proper event cleanup.
- No console errors.
- No broken buttons.
- No duplicate event listeners.

Use a single central product data structure so product names, prices, sizes, images, and look relationships remain consistent across all pages.

---

18. FINAL QUALITY REQUIREMENTS

Before completing the website, verify all of the following:

1. Homepage loads with the correct NOWHERE® brand identity.
2. The background remains "#ececec".
3. All nine supplied model images appear.
4. All nine models are positioned around the circular ring.
5. The ring rotates using spring physics.
6. The nearest model becomes active.
7. Ring/Grid toggle works.
8. Dragging works on mouse and touch.
9. The Looks drawer opens and closes.
10. Clicking a model opens focus mode.
11. FLIP animation works.
12. All 27 product records are available.
13. All product dots appear at the specified coordinates.
14. The receipt opens correctly.
15. Size selection works.
16. Add to bag works.
17. Bag count updates.
18. Cart survives page refresh.
19. Whole-fit discounts calculate correctly.
20. Shop All filtering works.
21. Product search works.
22. Product detail pages work.
23. Checkout validation works.
24. Mobile navigation works.
25. All layouts are responsive.
26. Animations are smooth and not excessively heavy.
27. Reduced-motion preference is respected.
28. No placeholder buttons remain.
29. No invented product names, prices, or claims appear.
30. No broken image URLs or JavaScript errors remain.

---

19. FINAL CREATIVE DIRECTION

The final website should look like a real premium independent fashion label.

Think of a luxury fashion editorial photographed inside a minimalist grey studio, transformed into a digital 3D shopping experience.

The homepage must immediately communicate the identity of NOWHERE®.

The circular lookbook should be the memorable centrepiece.

The rest of the website should provide a complete, easy-to-use shopping experience without losing the original artistic direction.

Do not simplify the design into a generic e-commerce template.

Do not remove the original nine-model circular lookbook.

Do not replace the supplied assets with unrelated stock images.

Do not use a dark background.

Do not sacrifice working functionality for visual effects.

Build the entire website, connect every interaction, test the shopping flow, and deliver the finished experience.

The final result must feel premium, cinematic, interactive, responsive, and production-quality.

END OF MASTER PROMPT
