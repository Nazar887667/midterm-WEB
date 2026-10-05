# Nomadica Event Travel Planning

Nomadica is a responsive, multi-page travel-planning website for people travelling to concerts, festivals, sports events, business events, and city breaks. It helps visitors outline their trip, compare sample flights and accommodation, plan transfers and event-day buffers, and find places around the destination.

The site uses plain HTML, custom CSS, and Bootstrap 5.3.8 through its CDN. It has no JavaScript, framework, build system, API, database, or backend. The sample fares and routes are for layout demonstration and are not live search results.

## Pages

- home.html — overview of the event travel planning flow and trip purposes
- plan.html — native HTML form for event and travel details
- routes.html — sample flight and accommodation comparison table
- timeline.html — sample itinerary with travel, transfers, and event time
- discover.html — nearby food, culture, nature, nightlife, and shopping ideas
- about.html — concept description and contact form
- sitemap.html — links and outline of the trip-planning flow

All seven pages use the same header, navigation, and footer. The active navigation link is marked with aria-current. Three SVG destination illustrations are stored in images/.

## Course concepts used

- Weeks 1–2: HTML document structure; headings, paragraphs, lists, links, images, forms, inputs, buttons, a table, semantic tags, div, and span.
- Week 3: CSS selectors, colors, fonts, spacing, alignment, classes, IDs, and responsive styling.
- Week 4: Flexbox, CSS Grid, relative and absolute positioning, a fixed back-to-top link, and centering with Bootstrap containers.
- Week 5: Bootstrap containers, responsive grid columns, typography, buttons, and spacing utilities.
- Responsive design: custom tablet and mobile media queries, plus Bootstrap responsive grid classes.

## View locally

Open home.html in a web browser. An internet connection is needed for Bootstrap CSS from the CDN. The local CSS and SVG images are included in this folder.

The forms use native HTML validation and submit fields in the browser. They are demonstrations only; the site does not save or send submissions.

## Publish with GitHub Pages

1. Create a GitHub repository for the project and upload all files and the images folder.
2. In the repository, open Settings, then Pages.
3. Under build and deployment, choose Deploy from a branch, select the main branch and root folder, then save.
4. Open the published address and check the navigation and page links.
5. Add the public address to your course submission.

Because the homepage is named home.html, include /home.html at the end of the GitHub Pages address. Netlify is configured to serve home.html at the site root. In a VS Code launch.json, set the file field to home.html in the workspace folder.

The live publication step is not included in this local project handoff. Add the final public URL here when published: [Add published site URL].

## Structure of the code

- Flexbox: styles.css uses #main-nav for wrapping header links, .footer-links for footer links, and .brand to align the logo mark and name.
- Grid: styles.css uses .timeline to place each day beside its itinerary text. The mobile media query changes it to one column.
- Positioning: #main-header is relative; .hero is relative and .hero::after is absolute; .back-top is fixed on wider screens and returns to normal flow on smaller screens.
- IDs: shared shell IDs are #main-header, #main-nav, #main-content, and #site-footer. Page IDs include #route-table in routes.html, #trip-form in plan.html, #contact-form in about.html, and #timeline-list in timeline.html. The #top anchor remains on every page.
- Media queries: styles.css has tablet rules at max-width 991.98px and mobile rules at max-width 575.98px. Bootstrap .row, .col-md-*, and .col-lg-* classes provide responsive columns. The route table uses .table-responsive for horizontal scrolling on small screens.
