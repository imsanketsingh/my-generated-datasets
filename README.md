
# Description of Each Dataset and the Respective Code

## Dataset 1: Company_Job_Dataset

#### **Dataset Description:**
This dataset contains close to 8k companies with various useful information such as *Tags(Domains in which the company work), Type of Company(Private or Public), Location(Headquarter + no. of other locations, Rating of the company, Total no. of reviews about the company, How old the company is, no. of working employees, About the company)*.

The dataset is created by scraping the famous job searching website AmbitionBox (*ambitionbox.com*)

#### **Code Description:**
Python libraries used: requests, BeautifulSoup, pandas

There was a total of 333 pages in the website containing information about the comapnies, hence the outer loop runs from 1 to 333.

For few of the companies, some of the values in a container were missing and there was no way to know which of the value is present and which is missing, hence I left those companies (happily they were relatively very low in number).

The lines 54 prints those companies having missing values.

Finally I converted the list of list into a dataframe using pandas library and exported it to a csv file.





Thanks for Reading!

## Authors

- [@imsanketsingh](https://www.github.com/imsanketsingh)




## Contributing

Contributions are always welcome!




## Feedback

If you have any feedback, please reach out to me at imsanketsingh@gmail.com


