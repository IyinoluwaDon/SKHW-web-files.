# She Knows Her Worth

She Knows Her Worth is a static website for a girls' empowerment initiative serving secondary-school-aged girls in underserved communities in Lagos, Nigeria.

The website communicates the initiative's work across three pillars:

- Menstrual dignity
- Identity and empowerment
- Safety and emotional well-being

## Website features

- Responsive multi-page website for desktop and mobile screens
- Vision and mission information
- Programme overview and session details
- School and community registration
- Sponsorship and organisational partnership enquiries
- School-supply donations, including:
  - School bags
  - Mathematics sets
  - Notebooks
  - Socks and school shoes
  - Calculators
  - Stationery
  - Sanitary and personal-care products
- Separate monetary donation form
- Contact and volunteer information
- Accessible navigation, skip links, focus states, and reduced-motion support

## Project structure

```text
.
├── index.html
├── about.html
├── programs.html
├── register.html
├── sponsor.html
├── donate.html
├── contact.html
└── assets/
    └── css/
        └── styles.css
```

All pages use the shared stylesheet at `assets/css/styles.css`. The stylesheet contains the site's design tokens, typography, layout helpers, responsive behavior, form styles, navigation, cards, animations, and page-specific utility classes.

## Running the site locally

This is a static HTML site and does not require a build step or package installation.

From the repository root, start any local static server. For example, with Python:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a browser.

You can also open `index.html` directly, although a local server is recommended for consistent browser behavior.

## Forms and integrations

The forms currently use placeholder endpoints and simulate a successful submission when no backend endpoint is configured. Before launch, replace the placeholder values with the organisation's chosen form or payment service:

- Partnership, sponsorship, supplies, monetary-gift, and volunteer information in
  `partnership.html`
- Registration form embedded in `register.html`
- Contact and enquiry links in `contact.html`

Payment processing is not currently connected. The monetary donation form captures the donor's intent until a live payment provider is configured.

## Editing guidelines

- Keep page content in the relevant HTML file.
- Add shared visual rules to `assets/css/styles.css` instead of using inline styles.
- Preserve semantic HTML, accessible labels, and keyboard focus states.
- Update navigation and footer links consistently across all pages when adding or renaming a page.
- Keep organisation contact details and form endpoints up to date before deployment.

## Licence

No licence has been specified for this project.
