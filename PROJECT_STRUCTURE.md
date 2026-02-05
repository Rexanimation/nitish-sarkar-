# Project Structure & Architecture

This document outlines the file structure of the `frontend` directory and maps key files to the application's pages and features.

## 📂 Frontend Directory Overview

The `frontend/` directory contains all client-side assets, including HTML pages, CSS stylesheets, JavaScript files, and media assets.

### 📌 Key Pages & Entry Points

| Page / Feature | File Path | Description |
| :--- | :--- | :--- |
| **Home Page** | `index.html` | The main landing page of the application. |
| **Packages Listing** | `packages.html` | Displays available travel and hotel packages. |
| **Login / Sign Up** | `newLogin.html` | Authentication page for user login and registration. |
| **Plan a Trip** | `plantrip.html` | Form interface for users to plan their custom trips. |
| **Map / View** | `mapa.html` | Interactive map or view page. |
| **About Us** | `about.html` | Company information and story. |
| **Contact Us** | Linked in Home | Contact form section (often within `index.html` or footer). |
| **Payment** | `payment.html` | Checkout and payment processing interface. |
| **User Feedback** | `feedback.html` | Form for collecting user ratings and feedback. |
| **Membership** | `membership.html` | Details on membership tiers and benefits. |

### 📂 Sub-Directories

*   **`dedicated-destinations/`**: Contains specific landing pages for individual destinations.
    *   Example: `dedicated-destinations/paris/start.html`
    *   Example: `dedicated-destinations/santorini-aegean-sea/start.html`
*   **`topdeals/`**: Contains the "Top Deals" page and related assets (`topdeals.html`).
*   **`Blog/`**: Contains blog posts and blog listing pages.
*   **`Image-Gallery/`**: Stores gallery specific styles and HTML.
*   **`img/`**: General image assets.
*   **`packages images/`**: Images specific to travel packages.

### 📝 Support & Legal Pages

*   `faq.html`: Frequently Asked Questions.
*   `tnc.html`: Terms and Conditions.
*   `privacy.html`: Privacy Policy.
*   `Licensing.html`: Licensing information.

### 🎨 Core Styles & Scripts

*   **Styles**:
    *   `style.css`: Main global stylesheet.
    *   `styles.css`: Additional core styles.
    *   `navLinks.css`: Navigation bar styling.
    *   `footer.css`: Footer component styling.
*   **Scripts**:
    *   `index.js`: Primary application logic.
    *   `Theme.js`: Theme toggling logic (Dark_Mode handling).
    *   `navbarToggle.js`: Mobile navigation toggling.

## 🔍 Detailed File Mapping

### Navigation Links
The main navigation bar (in `index.html` and others) links to:
1.  **Home**: `index.html`
2.  **About**: `about.html`
3.  **Services**: anchors within `index.html` (#Destinations, #trip, etc.)
4.  **Top Deals**: `topdeals/topdeals.html`
5.  **Packages**: `packages.html`
6.  **Testimonial**: anchor `#testimonial`
7.  **Rate Us**: `feedback.html`
8.  **Contact Us**: anchor `#cnt-form`
9.  **Login**: `newLogin.html`
10. **View Map**: `mapa.html`

### Auth Flow
*   **Login/Signup**: Users are directed to `newLogin.html`.
*   **Forgot Password**: `forgotPassword.html` serves the password recovery flow.

## ⚠️ Notes on Duplicate/Legacy Files
*   `package.html` vs `packages.html`: Both exist. `packages.html` appears to be the main one linked in navigation. `package.html` might be a legacy or alternate version.
*   `Signup.html` & `login/`: There is a root `Signup.html` and a `login/` folder which might contain older iterations. The current active auth page seems to be `newLogin.html`.
