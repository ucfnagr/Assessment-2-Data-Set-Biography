# Data Biography

## Student Number: 20181467

---

### 1. Who collected the data?

Murray Cox prepared the data, cleaned, analyzed and aggregated it

---

### 2. Why did they collect it?

Murray Cox prepared the dataset which allows to explore how Airbnb is being used in cities around the world to compete with the residential housing
market. For this purpose, several filters and key metrics were added.

---

### 3. How was it collected?

The data utilizes public information, which was verified, cleaned, analyzed and aggregated. The data was anonymized (location for a listing in the data will
be from 0-450 feet of the actual adress), that adds a noise to the data. The data is a snapshot of listings, made in the past, so it may be not actual for the
current moment. Inside Airbnb takes neighborhood names from the geographical coordinates but not from Airbnb neighborhood names.[1]

[1] http://insideairbnb.com/about.html

---

### 4. What useful information does it contain?


For listing offers there is a price "price", a text description "description", the name and text description of the neighbourhood "neighborhood_cleansed", "neighborhood_overview", geolocation "longitude", "latitude", type of house that is rented out "property_type", accommodation conditions, which include the number of "accommodations" and the number of bathrooms and bedrooms "bathrooms, bedrooms, a lot of information about the host, information about the conditions and possibilities of booking, as well as information on review



---

### 5. What useful information is it missing?

Fields "license", "bathrooms", "calendar_updated", "neghbourhood_group_cleansed" contain "NaN", field "scrape_id" has the same value for all entries, so
no useful infromation can be extracted. Entries 3559 and 29990 are structured incorrectly (they seem to be shifted), so few of abovementioned fields
contain different values, which also do not provide useful information.

---

### 6. To what extent is the data 'complete'?

We can see, that the set of useful fields we listed in the 4th question partially intersects with the missing information we listed in the 5th question.
Therefore, the potential amount of important patterns we can extract from this dataset decreases. From the figure 1 [2] we can see that more than a third
entries are NaN values in 20 dataset fields, some of which we have also called useful in the 4th question. It slightly complicates the process of analysys, but
still much data remains. From the figure 2 [3] we can see that almost 50000 dataset entries contain less than 10 NaN values. The small area under the curve
supports the statement that we have enough data to explore.

[2]https://github.com/ucfnagr/Assessment-2-Data-Set-Biography/blob/main/Figure1
[3]https://github.com/ucfnagr/Assessment-2-Data-Set-Biography/blob/main/Figure2
---

### 7. What kinds of analysis would this support?

_Your answer here_

---

### 8. What kinds of analysis would it _not_ support?

_Your answer here_

---

### 9. Which of the uses presented in Q.7 and Q.8 are _ethical_?

_Your answer here_

 
