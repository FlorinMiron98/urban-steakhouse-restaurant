# Urban Steakhouse Restaurant website - Testing Details

[Main README.md file](https://github.com/FlorinMiron98/urban-steakhouse-restaurant/blob/main/README.md)

## Table of Contents
1. [Validator Testing](#validator-testing)
2. [Performance, Accessibility and Best Practices Testing](#performance-accessibility-and-best-practices-testing)
3. [Manual Testing](#manual-testing)
4. [Testing Client Stories From UX](#testing-client-stories-from-ux)
5. [Functional Testing](#functional-testing)

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
      ![w3c - markup validator](https://github.com/user-attachments/assets/408ad642-8a9a-412e-b618-3be891a7663c)
2. [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
   - The CSS file was validated and is used across all HTML pages.
     **Results**:
     - The result for the CSS file checking is _"Congratulations! No Error Found."_
     ![w3c - css validator](https://github.com/user-attachments/assets/b54a1655-1e2d-430a-9a4a-2222342358d3)
### Performance, Accessibility and Best Practices Testing
Google Lighthouse Testing Results
   - **Overview**
     Google Lighthouse was used to evaluate the performance and quality of the Urban Steakhouse Restaurant project.
   - **Results by Page**
     - **Home page**(index.html)
       - **Performance**: Score 99/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
         
     ![index html - performance scores](https://github.com/user-attachments/assets/ccadd438-9e79-488d-b0c4-1d938f33a92f)

     - **Menu page**(menu.html)
       - **Performance**: Score 100/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
         
     ![menu html - performance scores](https://github.com/user-attachments/assets/bcf76cac-6108-42bc-967f-7241d5b55ee5)

     - **Reservation page**(reservation.html)
       - **Performance**: Score 99/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
         
     ![reservation html - performance scores](https://github.com/user-attachments/assets/26c30b63-b9ac-4aa6-bdb6-3201d930b928)

     - **About page**(about.html)
       - **Performance**: Score 100/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 100/100
         
     ![about html - performance scores](https://github.com/user-attachments/assets/81ffd2e9-a29a-49fb-bb1c-43769701954d)

     - **Contact page**(contact.html)
       - **Performance**: Score 100/100
       - **Accessibility**: Score 100/100
       - **Best Practices**: Score 78/100
         
       ![contact html - performance scores](https://github.com/user-attachments/assets/ea1f82b0-0c8f-4177-8c00-820e5660c4bd)

       - **Notes**:
         The 'Best Practices' score is below 80 because this page uses third-party cookies from [Google Maps](https://www.google.com/maps/dir/?entry=wc)
### Manual Testing
Conducting manual testing for the steakhouse website to ensure optimal user experience and functionality.
- **Desktop testing:** Verified compatibility using Chrome, Firefox, Microsoft Edge as well as Safari through [Playwright](https://playwright.dev/) on a Windows computer.
- **Mobile Testing (Android):** Checking responsiveness and functionality with Chrome and Firefox browsers on an Android device.
- **Link Verification:** All manually tested links, both internal and external, have been verified and successfully confirmed to function correctly, ensuring seamless navigation.
- **Form Validation:** All forms on the website have undergone thorough validation testing to ensure that users receive appropriate feedback for any input errors. Each form accurately checks for required fields and correct formatting.
### Testing Client Stories From UX
1. As a Regular Customer, I want to be able to book a table, using a simplified form and receive feedback when the form submission is complete.
   | **Test Description** | **Outcome** | **Status** |
   | -----------------| ------- | :----: |
   | Verify that the reservation form is displayed | Form should be visible on the page | Passed |
   | Test form submission with invalid full name format | Error message indicating the requested format | Passed |
   | Test form submission with empty full name input | Error message indicating required field should show | Passed |
   | Test form submission with invalid email address | Error message for invalid email should be displayed | Passed |
   | Test form submission with empty email address input input | Error message indicating required field should show | Passed |
   | Test form submission with invalid phone number format | Error message indicating the requested format | Passed |
   | Test form submission with empty phone number input | Error message indicating required field should show | Passed |
   | Test form submission with empty date input | Error message indicating required field should show | Passed |
   | Test form submission with empty hours select | Error message indicating required field should show | Passed |
   | Test form submission with empty number of guests input | Error message indicating required field should show | Passed |
   | Submit the form with valid data | Success message confirming reservation should be displayed | Passed |
2. As a Regular Customer, I want to sign up for newsletters, so I can stay informed about upcoming events.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Verify that the newsletter signup form is displayed | Form should be visible on the page | Passed |
   | Test form submission with an empty email field | Error message indicating the email field is required | Passed |
   | Test form submission with an invalid email address | Error message for invalid email should be displayed | Passed |
   | Test form submission with an empty text(full name) field | Error message indicating the text field is required | Passed |
   | Submit the form with a valid email address and text input | Success message confirming subscription should be displayed | Passed |
3. As a First Time Customer, I want the menu to be easily accessible and to be able to see images and read a short description about each dish.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Load the menu page | The menu page should be displayed correctly | Passed |
   | Check if all menu items are displayed | All menu items should be visible on the menu | Passed |
   | Verify that each menu item has an image | Each menu item should display an associated image | Passed |
   | Verify that each dish has a description | Each menu item should display a short description | Passed |
   | Test for responsiveness | The menu should be responsive and on all screen sizes | Passed |
   | Check for readability of descriptions | Descriptions should be legible and easy to read | Passed |
   | Ensure images are loading correctly | All images should load without errors | Passed |
   | Verify navigation to the menu from homepage | Users should be able to navigate to the menu easily | Passed |
4. As a Prospective Customer, I need to find essential information such as location, contact details, and opening hours clearly and concisely, so that I can plan my visit accordingly.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Load the contact information page | The contact information page should display correctly | Passed |
   | Verify display of location | The restaurant location should be clearly displayed | Passed |
   | Check for visibility of contact details | The contact details should be clearly visibile | Passed |
   | Check visibility of opening hours | Opening hours should be clearly displayed and easy to read | Passed |
   | Test for accessibility on mobile devices | Information should be accessible and readable on mobile | Passed |
5. As a Customer, I want to contact the restaurant easily through a contact form, so that I can ask questions or provide feedback.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Load the contact form page | The contact form should be displayed correctly | Passed |
   | Test form submission with invalid full name format | Error message indicating the requested format | Passed |
   | Test form submission with empty full name input | Error message indicating required field should show | Passed |
   | Test form submission with invalid email address | Error message for invalid email should be displayed | Passed |
   | Test form submission with empty email address input input | Error message indicating required field should show | Passed |
   | Test form submission with invalid phone number format | Error message indicating the requested format | Passed |
   | Test form submission with empty phone number input | Error message indicating required field should show | Passed |
   | Test form submission with empty textarea message | Error message indicating required field should show | Passed |
   | Submit form with valid data | Success message confirming reservation should be displayed | Passed |
6. As a Customer, I want to read reviews and ratings from other customers, so that I can gauge the quality of the restaurant.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Load the reviews page | The reviews page should be displayed correctly | Passed |
   | Verify display of customer reviews | All customer reviews should be visible | Passed |
   | Test for readability of reviews | Each review should be easy to read | Passed |
7. As a First-Time Visitor, I need easy navigation and a user-friendly design, including a responsive layout for my device, so I can find information quickly and efficiently without frustration.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Load the home page | The homepage should display correctly with all elements | Passed |
   | Verify navigation menu functionality | All links in the navigation menu should work correctly | Passed |
   | Test responsiveness | The layout should adapt and be user-friendly on all devices | Passed |
   | Ensure quick access to essential information | Key information (location, menu, contact) should be easy to find | Passed |
   | Check for consistent design elements | Fonts, colors, and buttons should be consistent throughout the site | Passed |
8. As a Potential Customer, I want to know who the restaurant's chefs are so that I can feel confident in the quality and creativity of the food.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Verify display of chef profiles | All chef profiles should be visible on the page | Passed |
   | Check for images of each chef | Each chef profile should display an associated image	| Passed |
   | Verify descriptions of chefs | Each chef should have a brief description about their experience | Passed |
   | Ensure consistent layout for chef profiles | All profiles should follow a consistent design format | Passed |
   | Check for readability of text | Text descriptions should be legible and easy to read | Passed |
   | Verify responsiveness on all devices | The chefs' section should be accessible and user-friendly on all devices | Passed |
9. As a Potential Customer, I want to watch a small video that showcases the ambience of the restaurant, so that I can get a feel for the atmosphere and overall dining experience before deciding to visit.
   | **Test Description** | **Outcome** | **Status** |
   | -------------------- | ----------- | :--------: |
   | Load the video modal | The video modal should be displayed correctly | Passed |
   | Verify video playback functionality | The video should play without errors when clicked | Passed |
   | Test for pause and play controls | Users should be able to pause and resume the video | Passed |
   | Verify video controls are visible | Play, pause, and volume controls should be present | Passed |
   | Check responsiveness on all devices | The video should display and play correctly on all devices | Passed |
### Functional Testing
| **Test Description** | **Expected Result** | **Status** |
| -------------------- | ------------------- | :--------: |
| Click on the "Home" link or logo in the navigation | The home page should load | Passed |
| Click on the "Menu" link in the navigation | The menu page should load | Passed |
| Click on the "Reservation" page in the navigation | The reservation page should load | Passed |
| Click on the "Subscribe" navigation from each page | The "Events Signup" from home page should be displayed | Passed |
| Click on the "About" page in the navigation | The about page should load | Passed |
| Click on the "Contact" page in the navigation | The contact page should load | Passed |
| Fill out each form with invalid inputs | Error messages should be displayed indicating invalid input | Passed |
| Fill out each form with valid inputs and submit it | A confirmation page should be displayed indicating successful submission | Passed |
| Press each prev and next buttons of Events and Testimonials carousel | The carousel should play | Passed |
| Move the cursor outside of Events and Tesimonials carousel | The carousel should autoplay | Passed |
| Click on the social media links in the footer | The respective social media pages should open in a new tab | Passed |
| Click on the "open-video-modal" button from the "About" page | The video modal should open | Passed |
| Play the video on the modal from the about page | The video should play | Passed |
| Pause the video on the modal from the about page | The video should pause | Passed |
| Click on each "View Details" button from the "Meet Our Chefs" section | A modal containing each chef's short description should open | Passed |
