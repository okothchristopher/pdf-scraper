# pdf-scraper
R Shiny application to scrape tables from PDFs. Uses [Tablua](http://tabula.technology/) via the [tabulizer package](https://github.com/ropensci/tabulizer) for R

The application, developed and hosted by the Natural Resource Governance Institute, allows users to scrape tables from PDFs into
structured data in their browser in a few clicks. See the hosted application [here]() or run the application in an R session.

## Background
The application was originally developed to assist in the collection of data from PDF reports filed under the ESTMA regulaions in Canada, data on payments to governments by oil, gas and mining companies. These standardized reports contained multiple pages of well structured reports whose manual transcription would have been tedious and potentially inaccurate over the hundreds of individual cases.

Upon discovering the tabulizer package from rOpenSci, a solution was imagined where the scraping and verification of data could be done side-by-side in a single environment, greatly increasing accuracy and productivity over a multi-program solution utilizing standalone Tabula and a spreadsheet program, or manual transcription.

Following that project, the application's wide-ranging applicability to those in the open-data community was realized and this tool is now available for all to use.

## Use
#### Step 1. Download PDF
![alt text](https://github.com/NRGI/pdf-scraper/blob/master/images/scraper1.gif)


#### Step 2. Scrape tables

Tables can be scraped by inserting their page number in the text field and using the `Scrape` button.

Multiple pages can be scraped simultaneously with their results combined by separating page numbers with a comma (`1,5,8`) or separating the first and last page in a series with a colon (`5:42`)
![alt text](https://github.com/NRGI/pdf-scraper/blob/master/images/scraper2.gif)

If a page contains multiple tables, the `Custom Scrape` button can be used to specficy an area of the page from which to extract the table. Must be done one page at a time.

![alt text](https://github.com/NRGI/pdf-scraper/blob/master/images/scraper3.gif)


#### Step 3. Download data

The scraped data visible in the table can be downloaded as a CSV or copy-pasted into a spreadsheet application. The table is fully editable and supports various functions available in a right-click menu.

![alt text](https://github.com/NRGI/pdf-scraper/blob/master/images/scraper4.gif)

