<h2 align="center" id="title">CS50's Web Programming with Python and JavaScript : Project 0 <br> Google Search Interface Clone</h2>

<p id="description">This project is a faithful recreation of the user interface for Google Search, Google Image Search, and Google Advanced Search, built using HTML and CSS to meet the specifications of CS50's Project 0.</p>

<h2>Project Files</h2>

*   `index.html` : Google Standard Search Page
*   `image.html` : Google Image Search Page
*   `advanced.html` : Google Advanced Search Page
*   `styles.css` : All CSS styling and responsive design rules

<h2>Implementation Details and Specifications Met</h2>

<p>The following sections detail how each requirement of the specification was addressed :</p>

<h3>1. Core Functionality (GET Parameters)</h3>

| Specification | Technical Implementation |
| :--- | :--- |
| **Standard Search** | The form uses `action="https://www.google.com/search"` and the search input is correctly named `name="q"`. |
| **"I'm Feeling Lucky"** | Implemented using a submit button with the required parameter: `<input type="submit" name="btnI">`. |
| **Image Search** | Achieved by including the critical hidden input field: `<input type="hidden" name="tbm" value="isch">`. |
| **Advanced Search** | All four required fields are implemented using Google's specific GET parameters: `name="as_q"`, `name="as_epq"`, `name="as_oq"`, and `name="as_eq"`. |

<h3>2. Aesthetics and Layout</h3>

| Specification | Technical Implementation |
| :--- | :--- |
| **Google Aesthetics (Overall)** | The layout is achieved using **Flexbox** on the `body` and a **negative top margin** on the main content wrappers (`.main-content`, `.search-wrapper-image`). This accurately replicates the centered-but-offset vertical alignment of the official Google search pages. |
| **Search Bar Styles** | Input bars feature the correct `border-radius`, realistic `width`, and a subtle `box-shadow` on hover. |
| **Multicolor Logo** | The logo is constructed using individual `<span>` tags, each styled with its corresponding color class (e.g., `.g-color-blue`). Letter spacing is corrected with a minor negative margin for a compact appearance. |
| **Advanced Search Alignment** | The four criteria fields are aligned precisely using **CSS Grid** (`display: grid; grid-template-columns: [values]`) to ensure all text input fields start at the same left margin, fulfilling the stacking and alignment requirements. |
| **Advanced Search Button** | Styled according to specification with the blue background and white text: (class `.advanced-submit-button`). |

<h3>3. Navigation and Structure</h3>

| Specification | Technical Implementation |
| :--- | :--- |
| **Page Navigation** | Links are present on all three pages, positioned at the top-right corner using `position: absolute;` on the `.nav-links` container for fixed placement. |

<h3>4. Responsive Design (Mobile Support)</h3>

| Specification | Technical Implementation |
| :--- | :--- |
| **Mobile Adaptability** | A dedicated **Media Query** (`@media (max-width: 650px)`) is used for all mobile adjustments. |
| **Element Scaling** | Search bar widths are reduced of the viewport width. Font sizes for the main logo are reduced and the image logo. |
| **Advanced Search Stacking** | On mobile, the CSS Grid layout collapses to a single column (`grid-template-columns: 1fr`) to ensure form labels and inputs stack vertically for readability. |
| **Button Sizing** | Button padding and margins are reduced to prevent horizontal overflow and ensure proper scaling on small screens. |

<h2> Video Demonstration Checklist</h2>

| Feature | Time Stamp |
| :--- | :--- |
| 1. Standard Google Search (index.html) | 0:01 |
| 2. Image Search Functionality (image.html) | 0:42 |
| 3. Advanced Search Functionality (all four fields) | 1:22 |
| 4. "I'm Feeling Lucky" Button | 2:26 |
| 5. Aesthetics (Centering, Rounded Corners, Google Logo) | 3:17 |
| 6. Navigation between the three pages | 3:33 |
| 7. Responsive Design (Demonstrate window resizing) | 3:51 |
