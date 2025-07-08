
Overview
The OCR Search Engine is a web-based tool designed to perform Optical Character Recognition (OCR) on PDF files. It enables users to search for specific sentences within multiple PDF documents, view the matching results, and export the results to an Excel file.

 Features
-	PDF Upload		: Upload one or multiple PDF files for processing.
-	Sentence Search		: Enter a sentence to search for within the uploaded PDFs.
-	Search Results		: View detailed search results, including document name, page 
  number, the matching sentence, and a screenshot of the match.
-	Zoom Feature		: Enlarge screenshots to inspect the matching area in detail.
-	Export to Excel		: Export the search results to a `.xlsx` file for further analysis.

Achievement
Integrated an efficient search mechanism that performs OCR (written or picture) on multiple PDF documents and identifies sentences containing the search term.

Business Impact
Increased Efficiency: Automates the process of searching through large volumes of PDF documents, significantly reducing the time and effort required to find relevant information.

Enhanced Accuracy: Ensures precise identification of relevant text by utilizing OCR technology, thereby minimizing manual errors in document review.

Better Data Management: The ability to export results into an `.xlsx` file improves data management, reporting, and decision-making processes.

Scalability: The tool can handle multiple PDF files simultaneously, making it scalable for businesses with extensive document processing needs.

 Tools and Technologies
-	HTML, CSS, JavaScript: Used for building the front-end interface, ensuring a responsive and user-friendly design.
-	PDF.js: A powerful library for rendering PDF files in the browser, enabling text extraction and page rendering.
-	FileSaver.js: Utilized for saving files on the client-side, specifically for exporting search results to an `.xlsx` file.
-	XLSX.js: A JavaScript library used to create and manipulate Excel files directly in the browser.
-	Docxtemplater.js: Included for any potential future enhancements involving document generation and templating.
-	JSZip: Used in conjunction with XLSX.js for handling file compression when creating Excel files.

 How to Use
 1. Upload PDF Files
-	Click the "Choose File" button or the file input box.
-	Select one or more PDF files from your device.
-	The selected files will be ready for OCR processing.

 2. Enter the Sentence to Search
-	In the "Enter sentence to find" textbox, input the exact sentence you want to search for within the PDFs.
Note: The search is case-insensitive, meaning it does not differentiate between uppercase and lowercase letters.

 3. Perform the Search
-	Click the "Search" button to start the OCR process.
-	Status Update: A message indicating "Searching..." will appear while the files are being processed.
-	The tool will extract text from each PDF page, search for the entered sentence, and display any matches found.

Result Table: 
-	Matches will be displayed in a table with columns for SLNO (serial number), Document Name, Page Number, the full sentence containing the match, and a screenshot of the page where the match was found.

 4. View Search Results
a. Results are displayed in a table with the following columns:
   - SLNO: Sequential number of the result.
   - Document Name: Name of the PDF file.
   - Page No: The page number where the sentence was found.
   - Match Text Full Sentence: The full sentence containing the searched sentence.
   - Screenshot: A small image of the page section where the match was found.
b. If no matches are found in a document, it will indicate "No Match Found".

 5. Zoom In on Screenshots
-	Click on a screenshot in the results table to enlarge it.
-	The enlarged image will appear in a modal (popup) window.
-	Click the "X" button or outside the modal to close the enlarged image.

 6. Export Results to Excel
-	Once the search is complete, click the "Export to .xlsx" button.
-	The results table will be converted to an Excel file named `result.xlsx`, which will be downloaded automatically.
-	The Excel file includes all the data from the table, with an additional column containing the image URLs of the screenshots.

 Troubleshooting
-	No PDFs Uploaded: Ensure that you have selected one or more PDF files before clicking the "Search" button.
-	No Sentence Entered: Make sure you enter a sentence in the search textbox before starting the search.
-	No Matches Found: If no matches are found, consider adjusting your search sentence for more common phrases or check the PDFs for possible OCR errors.
-	Search Errors: If the search process fails, an error message will be displayed in the status area. Try reloading the page and repeating the process.

 Technical Requirements
a.	Browser: Modern web browser with JavaScript enabled (e.g., Chrome, Firefox, Safari, Edge).
b.	File Types: Only accepts PDF files for upload.
c.	JavaScript Libraries Used:
o	pdf.js: For rendering and extracting text from PDF files.
o	FileSaver.js: For saving files locally.
o	xlsx.full.min.js: For creating and exporting Excel files.
o	jszip: For handling zip files.
o	docxtemplater: (Version mentioned but not utilized in this context).

Note
This tool works entirely in the browser, with no server-side processing, ensuring that your data remains secure and private on your local machine.
