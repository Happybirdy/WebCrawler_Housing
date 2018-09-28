# WebCrawler_Housing

### Project Summary
This project builds a web crawler that extracts housing-for-rent information from Craigslist at SF bay area.
Target URL: https://sfbay.craigslist.org/d/apts-housing-for-rent/search/apa  
Programming language: Java  
IDE: Eclipse  
External libaray: JSoup.1.10.1.jar  

### Repository Structure
The root directory of this repo is **WebCrawler_Housing**.  
Source code is in sub-directory **housing**  
**proxylist_bittiger.csv** contains a proxy list used in the source code to query the target URL.  
**crawler_log.txt** file records log information generated in the source code.  
**crawler_output.txt** file contain the top 20 output results crawled from the target web page.  

### How to use this repo
After this repo is cloned locally, go to folder **housing**, where there is a **pom.xml** file for uses to build the project using Maven. After the project is built, run the generated jar should generate the output results.

If the Maven method doesn't work, the source code can be imported into Eclipse and run from there.

### Key logic of the code
All source code is wrapped inside one class **CraigslistCrawler** where the main functino is the entry point of the program. The program first initializes the proxy account used to get access to the target URL, then parses the target web page based on JSoup library and DOM method. Output results are finally written into output file.

