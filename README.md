# Biyase Tech Website

Student: Melokuhle Ziqubu · Student number: ST10526097  
Module: Web Development (WEDE5020) · Year: 2026

## Project overview

A responsive website for Biyase Tech, a digital solutions provider serving individuals, businesses and educational institutions. It describes the organisation, its services, sample work, pricing approach and ways to contact the organisation.

## Pages and files

- `index.html` — home page
- `about.html` — organisation, mission and vision
- `services.html` — searchable service descriptions
- `portfolio.html` — image gallery with a lightbox
- `pricing.html` — quotation information
- `blog.html` — searchable and filterable articles
- `FAQ.html` — interactive accessible accordion
- `enquiry.html` — project/service enquiry with a contextual next-step message
- `contact.html` — general contact form and map
- `js/site.js` — shared interactions and form validation/submission
- `css/styles.css` — shared responsive styling
- `robots.txt`, `sitemap.xml`, `_headers` — crawler guidance, sitemap and Netlify security headers

## Functionality

The site uses JavaScript for FAQ accordions, service search, blog search and topic filtering, an accessible image lightbox, enquiry guidance, and HTML constraint validation with clear asynchronous form status messages. Both forms are configured for Netlify Forms and submit asynchronously on Netlify. The contact form and project enquiry are separate forms with different purposes. Honeypot fields provide basic spam filtering.

The enquiry result describes what information needs confirmation; it does not invent prices or promise availability. Biyase Tech must confirm both.

## Forms and email notifications

The form endpoints require deployment on Netlify. In the Netlify site dashboard, enable form detection and add an email notification for each form (`contact` and `enquiry`) using the organisation's approved recipient address. No recipient address was included in the supplied project, so none has been invented. The form action points to `thank-you.html` as its non-JavaScript fallback. The JavaScript submits using Netlify's form endpoint and announces success or failure on the page.

## SEO and deployment setup

The pages include descriptive titles, descriptions, semantic headings, alt text, internal links, mobile layouts and canonical URLs. Before publishing:

1. The site is deployed at https://sprightly-mermaid-7daa3b.netlify.app.
2. The canonical page links, `robots.txt` and `sitemap.xml` use this Netlify address. If you later add a custom domain, update these URLs and redeploy.
3. Submit `/sitemap.xml` in Google Search Console and check `/robots.txt`.
4. Configure the two Netlify form email notifications with the organisation's confirmed recipient address.
5. Replace illustrative portfolio imagery with approved project images and continue building relevant backlinks/social profiles as the organisation's real presence is established.

The contact page map currently shows South Africa as a general location because no verified street address was supplied. Update its map query if Biyase Tech has an approved public address. The page canonical URLs and sitemap now use the deployed Netlify address. Update them if you later choose a custom domain.

`_headers` supplies baseline browser security headers on Netlify. Keep dependencies minimal and use appropriately sized WebP/AVIF images when approved optimized assets are available. HTTPS is provided by the hosting platform after deployment.

## Local preview

Open `index.html` in a browser for a basic preview. For form submission and Netlify headers, deploy to Netlify; submissions cannot be delivered from a local file preview.


## Changelog

### Part 3 — 27 October 2026
- Reworked the existing HTML pages into a consistent semantic structure using the existing navy and teal visual direction, responsive layout, descriptive page titles and meta descriptions.
- Added `enquiry.html` for service, volunteer and sponsor enquiries, with required fields, HTML validation and service-specific next-step guidance that does not claim unverified pricing or availability.
- Rebuilt `contact.html` as a separate general message form with contact details, message type and message fields; configured both forms for Netlify Forms, asynchronous submission, status/error messaging and honeypot spam filtering.
- Added JavaScript interactions: FAQ accordion, searchable services, searchable/filterable blog posts, portfolio lightbox and form handling.
- Added `robots.txt`, `sitemap.xml`, Netlify `_headers`, canonical links, descriptions, semantic headings, image alt text, internal links and responsive styles. Updated canonical URLs, `robots.txt` and `sitemap.xml` to the deployed Netlify address.
- Corrected source-level Part 2 issues: normalized page markup and styles, fixed the portfolio filename and navigation labels, and corrected heading semantics. Specific lecturer feedback was not supplied with the project archive.
- Deployment update (2 November 2026): set the homepage canonical to the site root, updated `sitemap.xml` to the live Netlify URL, and renamed `_headers.txt` to `_headers` so Netlify can apply the security headers. Configure form email notifications with Biyase Tech's confirmed recipient address.

### Version 2.0 — Part 2
- Added website content, navigation, styling and initial project documentation.

### Version 1.0 — Initial release
- Created the project structure, HTML pages, navigation, company information and service descriptions.

## References

- MDN Web Docs, HTML forms and constraint validation: https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation
- MDN Web Docs, Fetch API: https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API
- Google Search Central, SEO Starter Guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- Netlify Docs, Forms setup: https://docs.netlify.com/forms/setup/
- Netlify Docs, custom headers: https://docs.netlify.com/manage/routing/headers/


