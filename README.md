# angel.co companies list scraping
Unfortunately official provided [API](https://angel.co/api) by angel.co was shut down.

This script allows you parse the list of the companies provided by angel.co from the page [All Companies](https://angel.co/companies)
and save it to all_companies.csv file.
Personally, I was interested only in a few columns such as `'name','desc','website','location','employees','raised','angel_url','angel_id'` however it wouldn't be hard to add or remove desirable columns.

# How to install & run the project
1. Install python 3.5 or higher
2. Clone the repo: `git clone git@github.com:iamtodor/angel.co-companies-list-scraping.git`
3. Enter into the project: `cd angel.co-companies-list-scraping`
4. Install all required libraries: `pip3 install -r pip-requirements.txt`
5. Run the command: `python3 parse.py`.
Also, you can run specific script with the specific query: `python3 parse.py -q='desired query'`. For example, the following command: ``python3 parse.py -q='computer vision'`` will parse companies from `https://angel.co/companies?keywords=computer+vision` page.

Also, I encourage to take a look at this sites, that I found pretty useful for small piece of data:
* https://www.process.st/checklist/how-to-scrape-angellist-for-investors-in-a-particular-city-using-import-io/#introduction
* https://phantombuster.com/
* https://webscraping.dexi.io/
