# Developer Documentation

# -ST10470949_WEDE5020_PART2
10.References:
• Chaffey, D. & Ellis-Chadwick, F., 2019. Digital Marketing: Strategy, Implementation and 
Practice, 7th edn. Harlow: Pearson. Available at: 
https://books.google.com/books/about/Digital_Marketing.html?id=PcP_vQEACAAJ
(Accessed: 13 August 2025).
• Garrett, J.J., 2010. The Elements of User Experience. Berkeley, CA: New Riders. Available 
at: 
https://books.google.com/books/about/The_Elements_of_User_Experience.html?id=6z
VbQgAACAAJ (Accessed: 13 August 2025).
• Norman, D.A., 2013. The Design of Everyday Things, revised edn. Cambridge, MA: MIT 
Press. Available at: https://mitpress.mit.edu/9780262525671/the-design-of-everyday-
things/ (Accessed: 13 August 2025).
• Krug, S., 2014. Don’t Make Me Think, Revisited: A Common Sense Approach to Web 
Usability, 3rd edn. New Riders. Available at: 
https://books.google.com/books/about/Don_t_Make_Me_Think_Revisited.html?id=qah
pAgAAQBAJ (Accessed: 13 August 2025).


## Project Overview
This project is a responsive website developed as part of coursework.  
It demonstrates the use of semantic HTML, external CSS styling, responsive layouts, and testing across devices (desktop, tablet, and mobile).  

The project highlights:  
- Use of external stylesheets (`css/style.css`).  
- CSS variables for consistent styling.  
- Responsive typography and layouts.  
- Evidence of testing with screenshots.  

---

## Part 2 Summary
In Part 2, the focus was on **styling and responsiveness**.  
Key tasks included:  
- Linking all pages to a central external stylesheet.  
- Defining CSS variables for color palette and font styles.  
- Adding responsive typography with heading and body text scaling.  
- Building layouts using CSS Grid (desktop: 2-column, mobile: stacked).  
- Testing responsiveness in DevTools and capturing screenshots.  

---

## Screenshots

- **Desktop View**  
  ![Desktop Screenshot](screenshots/screenshot-desktop.png)  
  *File: `screenshot-desktop.png` – Tested at 1920×1080 in Google Chrome.*

- **Tablet View**  
  ![Tablet Screenshot](screenshots/screenshot-tablet.png)  
  *File: `screenshot-tablet.png` – Tested at 712×1138 (Galaxy Tab S4 simulation) in Google Chrome.*

- **Mobile View**  
  ![Mobile Screenshot](screenshots/screenshot-mobile.png)  
  *File: `screenshot-mobile.png` – Tested at 430×932 (iPhone 14 pro max simulation) in Google Chrome.*

---

## Breakpoints
The following breakpoints were implemented in `css/style.css`:  

```css
/* 3.1 Breakpoints: Desktop, Tablet, Mobile */
@media (max-width: 1200px) {
    .content, section {
        padding: 2rem;
    }
    header, footer {
        padding: 1rem 0;
    }
    .content img, section img, aside img {
        width: 80%;
        height: auto;
    }
}

@media (max-width: 900px) {
    .content, section {
        padding: 1.5rem;
    }
    nav {
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;
        justify-content: center;
    }
    .content img, section img, aside img {
        width: 100%;
        height: auto;
    }
}

@media (max-width: 600px) {
    body {
        font-size: 1rem;
    }
    header h1 {
        font-size: 1.5rem;
    }
    .content, section {
        padding: 1rem;
    }
    nav {
        flex-direction: column;
        align-items: center;
    }
    .btn, button {
        padding: 0.75em 1.5em;
        font-size: 1em;
    }
    .content img, section img, aside img {
        width: 100%;
        height: auto;
        border-radius: 6px;
    }
    footer {
        font-size: 0.9em;
        padding: 0.5em 0;

    }
}

  /* Desktop styles */
}
