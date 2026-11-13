# Team Name: UNDERTAKERS

**Live site:**

## Team

| Name | Registration no. | GitHub username |
|---|---|---|
| Joseph Wachira Buyama | COM/3449/26 | juniorjonzz6-creator |
| Eugene Michael Ochieng | COM/3499/26 | eugene123-dev |

## Who drove each part

- Parts 0, 2, and 4: Joseph Wachira Buyama
- Parts 1 and 3: Eugene Michael Ochieng

## Personalisation

- **Our colours:** Purple (`#4C1D95`) and deep purple (`#2E1065`) in the light theme; lavender (`#C4B5FD`) and light lavender (`#A78BFA`) in the dark theme.
- **Projects we added:** Expense Tracker, Quiz App, and the UNDERTAKERS Team Website.
- **Extension challenges completed:** 1, 2, and 3.

## Technical Questions and Answers

1. **Why use a `<button>` for the menu toggle instead of a clickable `<div>`?**  
   A `<button>` is keyboard-operable by default, including with Enter and Space, and it receives focus in the normal tab order; a clickable `<div>` provides neither behavior without extra code. This would make the menu harder to use for keyboard users and people relying on assistive technologies.
2. **What could happen if `defer` were removed from the script in the `<head>`?**  
   Without `defer`, the browser would execute the script as soon as it encounters it in the `<head>`, pausing HTML parsing before the page body is built. The script's queries for page elements could return `null`, so features such as the menu, theme toggle, and project list might not initialize.
3. **Why use `textContent` instead of `innerHTML` for project titles?**  
   If visitor-provided project titles were inserted with `innerHTML`, the browser would parse them as markup instead of displaying them as plain text. A malicious title could inject unwanted elements or scripts, creating a cross-site scripting risk; `textContent` displays the title safely as text.
4. **Why must the server validate form data even when JavaScript checks it?**  
   Browser-side JavaScript validation can be bypassed or changed, so it cannot be trusted to protect submitted data. The server must validate the data independently before accepting or storing it.
5. **Why might the saved theme not carry over from a double-clicked file to Live Server?**  
   The browser stores `localStorage` data by origin, which includes the scheme, host, and port. A page opened as a local file and the same page served from Live Server have different origins, so the theme saved in one may not be available in the other.
6. **What is duplicated across the HTML pages, and how could that be improved?**  
   The header navigation and footer are repeated across our HTML pages, so updating them requires editing each copy and can lead to pages becoming inconsistent. A shared template or reusable component could keep these common sections in one place.

## Reflection

1. We learned to use semantic HTML to organize content and connect several pages with consistent navigation.
2. We learned how shared CSS styles and design variables help keep a website consistent, while responsive layouts make it usable on different screen sizes.
3. We practised using JavaScript to make pages interactive, including project search and filtering, mobile navigation, and a theme preference saved in the browser.
4. We learned that a good experience includes accessibility and clear feedback—not just appearance. Labels, keyboard focus styles, and helpful form validation all matter.
5. We saw how dividing responsibilities and using version control can help a team work together, but changes still need to be communicated and integrated carefully.
6. As developing programmers, we should keep practising, testing our work, learning from feedback, and writing accessible, maintainable code. A useful next step for this project would be connecting the contact form to a real service.
