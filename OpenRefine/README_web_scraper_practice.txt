Web Scraper Practice

watch on youtube:
https://youtu.be/FEUpiOOH0Jk

The prerecorded video demonstrates setting up a sitemap to collect data from the MET Museum collection. To keep the recording manageable, the scrape was narrowed down to the European Paintings collection filtered by Paper medium.


Note on the Click selector: The video includes a case that deviates from the standard Click selector setup. Normally, the Element Click selector is configured this way:
Selector — the container holding the data you want to extract
Click Selector — the element to click to reveal that content
In this specific case, the provenance content container is too generic for the scraper to reliably target using the standard approach. As a workaround, two separate selectors were used instead: an Element Click selector to open the Provenance tab, and a child Text selector to extract the text from within it. This is not the typical setup — in most cases the standard configuration will work.

Note on the exported data: The video shows an early export — the scraper had not finished collecting all records at the time of export. In practice, always wait until the scraper completes before exporting to ensure you have the full dataset.


Note on data loss:
Data loss is also a common occurrence. Websites are not always consistent — the same data point may be structured differently across pages, what works for most records may not work for exceptions, resulting in empty cells or missing values in your exported data. This is normal. After exporting, review your data for gaps, return to the sitemap if needed, and reconfigure the affected selectors to handle the exceptions.