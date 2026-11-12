# GTA VI-Inspired Promotional Website

## 1. Project Theme
This project is a multi-page promotional website inspired by the Grand Theft Auto VI marketing aesthetic. It focuses on immersive layouts, vibrant media presentation, full-screen canvas scroll animations, and a sleek, responsive dark-mode design. The overarching theme highlights the fictional state of Leonida, Vice City, and protagonists Jason and Lucia.

## 2. Technologies Used
- HTML5
- CSS3
- Vanilla JavaScript (utilized for scroll-scrubbing canvas animations, responsive menu toggling, interactive FAQ accordions, dynamic video players, and form state handling)

## 3. Website Pages

### Home Page — `index.html`
Introduces the game with a bold hero section, a launch trailer video modal, pre-order call-to-actions, and interactive scroll-driven canvas animations.

### Only in Leonida Page — `only-in-leonida.html`
Explores the characters, factions, and locations of Leonida using a sleek glassmorphic bento-box grid layout, sticky chapter navigation, and character-specific inline video modals.

### Pre-Load Now Page — `pre-load-now.html`
A news and announcement article layout detailing pre-load information, featuring a 16:9 dynamic hero video player and a grid of clickable related trailers that load seamlessly into the hero section.

### Support Page — `support.html`
A Rockstar-style knowledge base clone with a search hero, glowing help categories, an interactive FAQ accordion, and a stylized "Get in Touch" contact form with real-time feedback simulation.

### Gallery Page — `gallery.html`
Presents a visual archive of selected artwork, wallpapers, and character portraits featuring the people and places of Leonida.

### Music Page — `music.html`
Highlights the sounds of Leonida by featuring a grid of in-game radio stations, such as Cocoteo and Flash FM, alongside links to the official album.

## 4. Project Structure
- `index.html` — The main landing page
- `only-in-leonida.html` — Character and destination showcase
- `pre-load-now.html` — News article and video grid
- `support.html` — Knowledge base and contact page
- `gallery.html` — The artwork and wallpapers gallery
- `music.html` — The radio stations and music showcase
- `styles.css` — Core website styling for the home page and global footer
- `media-pages.css` — Shared styling specifically tailored for the Gallery, Music, and global transparent headers
- `leonida.css` — Dedicated styling for the bento-box grids and Only in Leonida page components
- `pre-load.css` — Dedicated styling for the news article format and video grids
- `support.css` — Dedicated styling for the help desk, FAQ accordions, and contact forms
- `frames/` & `frames2/` — Directories containing the sequential image frames for the canvas scroll animations
- `README.md` — Project documentation

## 5. AI Usage Log
AI assistance was used during development, bug fixing, and functionality optimization. The following entries describe the types of assistance requested:

| Task | AI Assistance Requested | How the Assistance Was Used |
|---|---|---|
| **Global Responsiveness** | Help making the whole website responsive. | Used to rewrite and condense CSS media queries (using fluid `clamp()` functions) to ensure the entire website scales flawlessly across all device sizes. |
| **Interactive JavaScript** | Help with scroll-scrubbing canvas animations and responsive menu toggling. | Used to structure and refine the Vanilla JavaScript required for the scroll-bound image sequences and the mobile hamburger menu interactions. |
| **Video Overlay Modal** | Help implementing and styling the video overlay. | Used to build and troubleshoot the CSS and layout logic for the launch trailer pop-up modal, ensuring it displays correctly over the page content. |
| **Bento-Box Layouts** | Help designing character grids and contact sections. | Used to structure complex CSS Grid layouts for character profiles and contact forms, balancing imagery with typography and ensuring mobile responsiveness. |
| **Dynamic Video Players** | Help swapping static images with YouTube iframes. | Used to write JavaScript that reads data attributes from clicked cards, hides static hero images, and dynamically injects autoplaying video URLs into iframes. |
| **Form State Management** | Help creating instant UI feedback for the contact form. | Used to write JS logic that validates empty fields, triggers neon error states, and mimics a successful transmission state without page reloads. |

## 6. How to Run the Project
1. Clone or download the project folder to your local machine.
2. Open `index.html` in any modern web browser.
3. Use the top navigation links or the hamburger menu overlay to navigate seamlessly between all 6 pages.

## 7. Customization
- Edit the HTML files to update text, release dates, and trailer embed links.
- Edit `styles.css` and the page-specific stylesheets (`leonida.css`, `support.css`, etc.) to change the global layout, colors, and font families.
- To customize the scroll animations, replace the `.jpg` sequence files in the `frames/` and `frames2/` folders and adjust the `frameCount` variable in the respective HTML scripts.

## 8. Notes
- Ensure all static images, such as `launch-image.png` and `gta6-logo.png`, are placed in the correct directory relative to the HTML files.
- The newsletter subscription and support contact forms are for visual presentation and UI feedback simulation only; they require external backend integration to process real submissions.
- The canvas scroll animation strictly requires sequential images named in the format `frame_001.jpg`, `frame_002.jpg`, etc., to render correctly on scroll.