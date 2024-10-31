# Urban Steakhouse Restaurant website - Testing Details

[Main README.md file](https://github.com/FlorinMiron98/urban-steakhouse-restaurant/blob/main/README.md)

## Testing
### Validator Testing
1. [W3C Markup Validator](https://validator.w3.org/)
   - **Pages validated**:
     - index.html
     - menu.html
     - reservation.html
     - about.html
     - contact.html
     - subscribe-confirm.html
     - reservation-confirm.html
     - contact-confirm.html
   - **Results**:
     - The result for all pages checking is _"Document checking completed. No errors or warnings to show."_
2. [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
   - The CSS file was validated and is used across all HTML pages.
     **Results**:
     - The result for the CSS file checking is _"Congratulations! No Error Found."_
### Performance, Accessibility and Best Practices Testing
3. Google Lighthouse Testing Results
   - **Overview**
     Google Lighthouse was used to evaluate the performance and quality of the Urban Steakhouse Restaurant project.
   - **Results by Page**
     - **Home page**(index.html)
       - **Performance**: Score 98/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
     - **Menu page**(menu.html)
       - **Performance**: Score 98/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
     - **Reservation page**(reservation.html)
       - **Performance**: Score 99/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
     - **About page**(about.html)
       - **Performance**: Score 99/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
     - **Contact page**(contact.html)
       - **Performance**: Score 100/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 78/100
       - **Notes**:
         The 'Best Practices' score is below 80 because this page uses third-party cookies from [Google Maps](https://www.google.com/maps/dir/?entry=wc)
## Testing client stories from UX
1. As a Regular Customer, I want to be able to book a table, using a simplified form and receive feedback when the form submission is complete.
   | **Test Description** | **Outcome** | **Status** |
   | -----------------| ------- | :----: |
   | Verify that the reservation form is displayed | Form should be visible on the page | Passed |
   | Test form submission with empty fields | Error message indicating required fields should show | Passed |
   | Test form submission with invalid email address | Error message for invalid email should be displayed | Passed |
   | Submit the form with valid data | Success message confirming reservation should be displayed | Passed |
3. As a Regular Customer, I want to sign up for newsletters, so I can stay informed about upcoming events.
4. As a First Time Customer, I want the menu to be easily accessible and to be able to see images and read a short description about each dish.
5. As a Prospective Customer, I need to find essential information such as location, contact details, and opening hours clearly and concisely, so that I can plan my visit accordingly.
6. As a Customer, I want to contact the restaurant easily through a contact form, so that I can ask questions or provide feedback.
7. As a Customer, I want to read reviews and ratings from other customers, so that I can gauge the quality of the restaurant.
8. As a First-Time Visitor, I need easy navigation and a user-friendly design, including a responsive layout for my device, so I can find information quickly and efficiently without frustration.
9. As a Potential Customer, I want to know who the restaurant's chefs are so that I can feel confident in the quality and creativity of the food.
10. As a Potential Customer, I want to watch a small video that showcases the ambience of the restaurant, so that I can get a feel for the atmosphere and overall dining experience before deciding to visit.
