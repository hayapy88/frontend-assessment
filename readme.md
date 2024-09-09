# Frontend Technical Assessment

## Introduction

---

Thank you for reviewing my submission for the frontend technical assessment. This project focuses on showcasing my ability to build responsive and high-quality software while following best practices and coding guidelines. The primary technologies used are Vue.js, Tailwind CSS, and SCSS.

## Exercises

### Exercise 1: Responsive Page

Objective: Build a responsive page based on the provided designs.

#### Skills used for Exercise 1

- HTML
- SCSS (BEM methodology)
- Tailwind CSS
- Vue.js
- Webpack
- Responsive Web Design

##### Requirements

1. Match the designs exactly.
2. Needs to be responsive.

##### Designs

- exercise1-desktop.png
- exercise1-mobile.png

##### Assets

- Desktop banner - https://via.placeholder.com/1920x650
- Mobile banner - https://via.placeholder.com/600x600
- Content images - https://via.placeholder.com/400x300

### Exercise 2: Tabs and Accordion

Objective: Display data from a JSON file as tabs on desktop and an accordion on mobile.

#### Skills used for Exercise 2

- HTML
- SCSS (BEM methodology)
- Tailwind CSS
- Vue.js
- Webpack
- Responsive Web Design

##### Requirements

1. Display data in tabs on desktop.
2. Display data in an accordion on mobile.
3. Only 1 accordion/tab should be open at a time.
4. Open the first accordion/tab on load.
5. If the open accordion is selected, close it.

###### Bonus points

- Improve the user experience with meaningful animations/transitions. -> Completed
- Design and styling. -> Completed
- Explain why the result of `('b' + 'a' + + 'a' + 'a').toLowerCase()` is `banana`.
  The result of ('b' + 'a' + + 'a' + 'a').toLowerCase() is banana. Here's why:
  'b' + 'a' results in 'ba'.
  The expression + 'a' attempts to convert 'a' to a number. However 'a' is not a valid number. So it returns NaN.
  Thus, 'ba' + NaN results in 'baNaN'.
  And then 'baNaN' + 'a' results in 'baNaNa'.
  Finally, toLowerCase() converts 'baNaNa' to 'banana'.

## Setup Instructions

### Exercise 1

1. Clone the repository:
   git clone https://github.com/hayapy88/frontend-assessment
   cd frontend-assessment/exercise1
2. Install dependencies:
   npm install
3. Run the project:
   npm start
   (The project page will open in your web browser at: http://localhost:8000)

### Exercise 2

1. Install dependencies:
   cd ../exercise2
   npm install
2. Run the project:
   npm start
   (The project page will open in your web browser at: http://localhost:8001)

## Contact

For any questions or feedback, please contact me at hayatoyokoi.work@gmail.com.
