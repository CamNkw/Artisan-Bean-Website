THE ARTISAN BEAN COFFEE ROASTERY — WEBSITE PROJECT
Part 3: Enhancing Functionality and SEO

STUDENT INFORMATION
Student Name: Mihlali Nkwanyana
Student Number: ST10540880
Group: Group 1
Subject: WEDE5020
Project: The Artisan Bean Coffee Roastery

1. PROJECT OVERVIEW
The Artisan Bean is a fictional specialty coffee roaster based in Cape Town, South Africa. This website presents the business, its coffee range, workshops and contact information. Part 3 builds on the original five-page Part 1/Part 2 website by adding JavaScript interactions, form validation, SEO improvements, an interactive map, performance improvements and deployment configuration.

2. WEBSITE PAGES
- Home.html — brand introduction, hero image, featured coffees and workshop calls to action.
- About Us.html — company history, mission, vision and team profiles. Mission and vision use an accessible JavaScript accordion.
- Products.html — four coffee products with live text search, category filtering, price sorting and image lightbox.
- Enquiry.html — workshop, wholesale and corporate enquiry form.
- Contact.html — business contact details, two locations, interactive Leaflet map and contact form.

3. PART 3 FUNCTIONALITY IMPLEMENTED
JavaScript and interaction (js/site.js)
- Responsive mobile navigation with an accessible expanded/collapsed state.
- Mission and vision accordion on the About page.
- Reusable image lightbox on product imagery; close button, backdrop click and Escape key are supported.
- Product search checks product names and descriptions as the user types.
- Product category filter (single origin / blend).
- Product price sorting (low-to-high and high-to-low).
- Live result count for the product catalogue.
- Client-side form validation, including required fields, email format, phone format, and field length constraints.
- Clear validation/submission feedback using an accessible status region.
- Current year in the footer.

Interactive map (js/maps.js)
- Leaflet 1.9.4 and OpenStreetMap tiles display two location markers with pop-up address information.
- Map markers are approximate neighbourhood positions based on the addresses in the supplied Part 2 website. Exact premises coordinates should be confirmed before the website is used by real customers.

4. FORMS AND SUBMISSION
Both forms use HTML5 validation and JavaScript validation. They are marked as Netlify Forms (`data-netlify="true"`) and submit asynchronously after deployment on Netlify. Netlify must have form detection enabled. After the first successful deployment, check the Netlify Forms dashboard and configure an email notification to hello@artisanbean.co.za (or the real business recipient) under Site configuration / Notifications. The fictional domain and recipient in the original project have not been independently verified.

When the site is opened directly from a local file (file://), or hosted somewhere other than Netlify, there is no server to receive form submissions. In that case the script displays a clear message rather than pretending that the message was sent. Client-side validation still works. A real hosted form service or backend is required for production submissions.

5. SEARCH ENGINE OPTIMISATION
- Unique page titles and meta descriptions on all five pages.
- Open Graph title and description metadata.
- Semantic page landmarks, one main page heading per page, descriptive image alt text and descriptive internal links.
- Internal navigation links corrected to match the actual case-sensitive filenames.
- `robots.txt` allows normal crawling and points to the sitemap.
- `sitemap.xml` lists the five main pages.
- Images resized and recompressed as JPEG to reduce transfer size; below-the-fold images use lazy loading and the homepage hero image has high fetch priority.
- Responsive layout, keyboard focus indicators, skip link, reduced-motion support and accessible form status messages.


6. FILE AND FOLDER STRUCTURE
Artisan Bean Website/
|-- Home.html
|-- About Us.html
|-- Products.html
|-- Enquiry.html
|-- Contact.html
|-- README.txt
|-- robots.txt
|-- sitemap.xml
|-- netlify.toml
|-- css/
|   `-- styles.css
|-- js/
|   |-- site.js
|   `-- maps.js
`-- images/
    |-- hero-coffee-beans.jpg
    |-- about-roastery.jpg
    |-- product-colombia.jpg
    |-- product-ethiopia.jpg
    |-- product-brazil.jpg
    |-- product-houseblend.jpg
    |-- contact-cafe-interior.jpg
    |-- map-hq.jpg
    `-- map-cafe.jpg

7. CHANGELOG
Version 1.0.0 — 17 August 2026 — Part 1 foundation
- Created the five original HTML pages, shared CSS stylesheet, navigation, product cards, team section, contact details and initial forms.

Version 1.1.0 — Part 3 enhancement release — 2 November 2026
Added:
- Added shared JavaScript for responsive navigation, accessible accordion behaviour, image lightbox, product search, product category filtering, product sorting, live result count and dynamic footer year.
- Added JavaScript client-side validation and accessible status feedback to the enquiry and contact forms.
- Added Netlify Forms attributes and asynchronous form submission support for deployment.
- Added Leaflet/OpenStreetMap interactive map with two location markers and pop-up address information.
- Added unique SEO titles, meta descriptions, Open Graph metadata, descriptive image alternative text, sitemap.xml and robots.txt.
- Added Netlify deployment configuration and baseline security/cache response headers.
- Added keyboard focus styling, skip navigation link, mobile navigation, reduced-motion support and responsive catalogue controls.
- Resized and recompressed large JPEG images to improve page loading performance.

Changed:
- Corrected homepage links that used lowercase filenames and did not match the case-sensitive page filenames.
- Updated README to document Part 3 functionality, deployment instructions, known limitations and the changelog.
- Preserved the original five-page structure, Artisan Bean branding, coffee colour palette, page content and supplied imagery.

8. TESTING CHECKLIST
[✅] Open Home.html and follow all five navigation links.
[✅] Test the mobile menu at a narrow screen width.
[✅] Open About Us.html and expand/collapse Mission and Vision using mouse and keyboard.
[✅] Open Products.html; search for a tasting note, filter blends, and sort prices both ways.
[✅] Click a product image, then close the lightbox using its button, backdrop and Escape key.
[✅] Submit each form empty and confirm required-field validation appears.
[✅] Enter invalid email/phone values and confirm validation feedback.
[✅] Deploy to Netlify, enable form detection, submit test forms and confirm they appear in Netlify Forms.
[✅] Confirm map tiles and both markers load while connected to the internet.
[✅] Replace placeholder sitemap domain and check deployed robots.txt and sitemap.xml.
[✅] Test the site on desktop and mobile and run Lighthouse/PageSpeed before final submission.

9. REFERENCES / THIRD-PARTY RESOURCES
- MDN Web Docs — HTML forms and constraint validation: https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Form_validation
- MDN Web Docs — Fetch API: https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API
- Leaflet documentation: https://leafletjs.com/reference.html
- OpenStreetMap copyright and attribution: https://www.openstreetmap.org/copyright
- Netlify Forms documentation: https://docs.netlify.com/forms/setup/
- Google Search Central — sitemap guidance: https://developers.google.com/search/docs/crawling-indexing/sitemaps/overview
- Google Search Central — robots.txt guidance: https://developers.google.com/search/docs/crawling-indexing/robots/intro
- W3C Web Accessibility Initiative: https://www.w3.org/WAI/standards-guidelines/wcag/

END OF README


