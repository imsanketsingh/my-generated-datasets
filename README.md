<div align="center">
  <h2>My Hacktoberfest 2022 Holopin Badges</h2>
</div>

[![@imsanketsingh's Holopin board](https://holopin.me/imsanketsingh)](https://holopin.io/@imsanketsingh)

# Description of Each Dataset and the Respective Code

## Dataset 1: Company_Job_Dataset

### **Dataset Description:**
This dataset contains close to 8k companies with various useful information such as *Tags(Domains in which the company work), Type of Company(Private or Public), Location(Headquarter + no. of other locations, Rating of the company, Total no. of reviews about the company, How old the company is, no. of working employees, About the company)*.

The dataset is created by scraping the famous job searching website AmbitionBox (*https://ambitionbox.com*)

### **Code Description:**
Python libraries used: requests, BeautifulSoup, pandas

There was a total of 333 pages in the website containing information about the comapnies, hence the outer loop runs from 1 to 333.

For few of the companies, some of the values in a container were missing and there was no way to know which of the value is present and which is missing, hence I left those companies (happily they were relatively very low in number).

The lines 54 prints those companies having missing values.

Finally I converted the list of list into a dataframe using pandas library and exported it to a csv file.

##
## Dataset 2: Country_Info_Dataset

### **Dataset Description:**
This dataset contains information about a total of 226 countries in the world.

The total no. of columns are 38.

The columns are as follows: *{name, population, region, life_expectancy_male, unemployment, imports, exports, currency, iso2, employment_services, employment_industry, urban_population_growth, secondary_school_enrollment_female, employment_agriculture, capital, co2_emissions, forested_area, tourists, homicide_rate, life_expectancy_female, post_secondary_enrollment_female, post_secondary_enrollment_male, primary_school_enrollment_female, infant_mortality, gdp_growth, threatened_species, sex_ratio, urban_population, secondary_school_enrollment_male, gdp, pop_growth, surface_area, pop_density, internet_users, gdp_per_capita, fertility, refugees, primary_school_enrollment_male}*.

The dataset is created by pulling data from an API provided by API Ninjas (*https://apininjas.com*).

### **Code Description:**

Python libraries used: requests, pandas

We first needed to have a list of all the countries we want to fetch the data for.

For this, I had a list of all the recognised countries in the world. The total number of countries present in the ```list_countries.xlsx``` are 243.

The total number of countries that successfully had been fetched are 226.

There was a need of column arrangement to have a better look at the data. So I did that as well.

##
## Dataset 3: All_Planets_Dataset

### **Dataset Description:**
This dataset contains information about a total of 822 Planets found till date in the our observable universe.

The total no. of columns are 9.

The columns are as follows: *{name, mass, radius, period, semi_major_axis, temperature, distance_light_year, host_star_mass, host_star_temperature}*.

The dataset is created by fetching each and every planet discovered till date (through scraping a website named: http://www.openexoplanetcatalogue.com) and then pulling available data from an API provided by API Ninjas (*https://apininjas.com*).

### **Code Description:**

Python libraries used: requests, pandas, BeautifulSoup

We first needed to have a list of all the planets we want to fetch the data for. So the first portion of code is dealing with that thing.

Here I am scraping a famous website named ```openexoplanetcatalogue``` to get the name for all planets found till date.

The website had a lot of data and names, but our API has limited data. It didn't had the data for all Planets. So I put a check to know whether the data for current planet is available or not.

##
**The Parameters of the Dataset are given below:**


```name -> The name of the planet.```

```mass -> Mass of the planet in Jupiters (1 Jupiter = 1.898 × 1027 kg).```

```radius -> Average radius of the planet in Jupiters (1 Jupiter = 69911 km).```

```period -> Orbital period of the planet in Earth days.```

```semi_major_axis -> Semi major axis of planet in astronomical units (AU).```

```temperature -> Average surface temperature of the planet in Kelvin.```

```distance_light_year -> Distance the planet is from Earth in light years.```


##
## API Reference

```http
Headers
X-Api-Key (required) - API Key associated with your account.
```

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |



## Contributing

Contributions are always welcome!



## Authors

- [@imsanketsingh](https://github.com/imsanketsingh)


## Feedback

If you have any feedback, please reach out to me at imsanketsingh@gmail.com
### Thanks for reading♥!
