# Salary Calculator

A web-based application for calculating and managing salary entries. This tool is designed to help track income from general services, calculate totals, and generate summaries and invoices.

## Features

- **Salary Entry Management:** Add, view, and delete salary entries.
- **Automatic Calculations:** Calculates total salary based on service type, location, and additional services.
    - **Cleaning Service:** Pricing based on the number of futons and location.
    - **General Cleaning:** Pricing based on hourly rates.
- **Monthly Overview:** View entries filtered by month.
- **Cumulative Totals:** Tracks and displays cumulative salary for the selected month.
- **Search Functionality:** Easily find specific entries.
- **Data Persistence:** Entries are saved in the browser's localStorage.
- **Export Options:**
    - Copy a summary of entries to the clipboard.
    - Generate a PDF invoice for the selected month.
- **Theme Customization:** Switch between light, dark, and system themes.
- **Responsive Design:** Adapts to different screen sizes.

## Technologies Used

- **HTML:** Structure of the web page.
- **CSS (Tailwind CSS):** Styling and layout.
- **JavaScript (Vue.js):** Application logic and interactivity.
- **html2pdf.js:** For generating PDF invoices.
- **Tippy.js:** For custom tooltips.

## How to Use

1.  **Open `index.html`:** Open the `index.html` file in a web browser.
2.  **Select Month:** Choose the year and month for which you want to manage entries.
3.  **Add New Entry:**
    *   Fill in the "New Entry" form with details:
        *   **Date:** Select the date of the service.
        *   **Calculation Method:** Choose between "Cleaning Service" or "General Cleaning".
        *   **Location:** Select the service location (e.g., SAKURAYA, Tsuzumi).
        *   **Service Specifics:**
            *   For "Cleaning Service": Enter the number of futons, laundry fee, tax amount, and transport fee.
            *   For "General Cleaning": Enter the hours worked and transport fee.
        *   **Additional Services:** Check any applicable additional services like "Lost Item Handling," "Letter Pack Plus," or "Coin Laundry Drying." You can also add a custom "Other Service" with a reason and price.
    *   The "Total Amount" will be calculated automatically.
    *   Click "Add Entry" to save the record.
4.  **View Entries:** Added entries will appear in the "Salary Entries" table, sorted by date.
5.  **Search Entries:** Use the search bar above the table to filter entries by date, location, or details.
6.  **Clear Data:** Click the "Clear Data" button to remove all entries for the selected month (a confirmation will be required).
7.  **Copy to Clipboard:** Click the "Copy to Clipboard" button to copy a text summary of all entries for the selected month.
8.  **Generate Invoice:** Click the "Generate Invoice" button to download a PDF invoice containing all entries for the selected month.
9.  **Switch Theme:** Use the theme toggle buttons (sun, moon, desktop icons) at the top right of the header card to switch between light, dark, and system-default themes.

## Data Storage

Salary entries are stored locally in your web browser's localStorage. This means your data will persist across sessions on the same browser and computer. Clearing your browser's cache or site data for this page may remove the stored entries.

## Setup

This is a single-file web application. No special setup or build process is required. Simply download the `index.html` file and open it in a modern web browser that supports JavaScript.

## Supporting Documents

`Price and other details.pdf`: This PDF file may contain important information regarding pricing structures, service details, or other rules relevant to salary calculation. Please refer to it for accurate data input.

