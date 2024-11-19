# Django HTMX Calculator - Practical Test - Guidelines for the candidate

_Fabrizio Nastri, Nov 2024_

### Description

This repo provides the scaffolding for a simple app designed to test your knowledge of:

- Django,
- Django templating,
- HTMX.

This tech stack is a potential solution for the FlexUp MVP project, prioritizing basic functionalities while minimizing the front-end development workload. The UI/UX may be enhanced in later phases.

The purpose of this test is to assess your proficiency with the mentioned technologies and your ability to work with a simple front-end application. Please aim to complete the test within 4 hours.

### App specifications / coding exercise

The root folder contains a simple stand-alone `calculator.html` page, in which the user can enter a product with the name, price and tax information. The unique feature of this page is that users can provide any two of the three numerical values (price excluding tax, price including tax, and tax rate), and the JavaScript will automatically calculate the third value.

Your task is to build a Django application based on this page. The app should allow users to:

- Store products in a database
- Display the stored products in a list
- View, edit, and delete products

### User stories / features:

1. Create a new product.
2. List all products.
3. View a product's details.
4. Edit a product.
5. Delete a product.

### Requirements:

- The Django app has a single page, that contains:
  - A header titled "Tax Calculator".
  - A form for entering product details.
  - A table listing all products (you will need to create this table).
- The same form should be used for creating, viewing, and editing a product.
- When the user submits the form:
  - The product should be saved to the database.
  - The product list should update dynamically.
  - The form should reset (cleared)
- The list of all products should be on the same page, as table, under the form, and contain the following columns:
  - Name
  - Price Excluding Tax
  - Tax Rate
  - Price Including Tax
  - A "View/Edit" button
  - A "Delete" button
- The user should be able to:
  - Click "View/Edit" to populate the form with a product's details. The header and list should remain unchanged.
  - Click "Delete" to remove the product from the database and update the table. The header and form should remain unchanged.
- Column headers should be in "Title Case"
- The page should never reload or redirect to another page.
- Use HTMX for dynamic updates:
  - When a product is added, updated, or deleted, only the affected row should update in the table.
  - The header and form should remain static.
- Use the default Django SQLite database

## Submission Instructions

1. Clone or fork this repository to start working on your solution.
2. Implement the required features.
3. Push your changes to your own GitHub repository.
4. Make your repository private and invite me (`fabrizionastri`) as a collaborator.
5. Send me an email to let me know that you have completed the test with a link to your repository.

## Additional Notes:

- Time Management: Aim to complete the test in less than 4 hours. Focus on functionality rather than design.
- Best Practices: Follow Django conventions for code organization and use HTMX effectively for a seamless user experience.
- Update the README.md file with any changes & additional information you think is relevant.
- Structure the project in a way that is clean and easy to understand, following best practices. Make sure to include the required files (e.g. `requirements.txt`, `.gitignore`, etc.).
