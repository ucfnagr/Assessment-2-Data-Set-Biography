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

Reference:
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

References:
[2]https://github.com/ucfnagr/Assessment-2-Data-Set-Biography/blob/main/Figure1
[3]https://github.com/ucfnagr/Assessment-2-Data-Set-Biography/blob/main/Figure2
---

### 7. What kinds of analysis would this support?

We can use several fundamental types of analysis.
We can use descriptive analysis together with quantitative methods to analyze numerical data: for instance, we can find the median values of prices and their standard deviation for different property types.
We can use exploratory data analysis to visualize distributions and dependencies and assume the mechanics of price and availability
Specifically, we can use geospatial analysis to visualize the distribution of houses/apartments over the London territory using the values from "longitude" and "latitude" fields.
We can use predictive analysis together with textual analysis methods: particularly, we can approximate the dependece of the frequency of rentals (using "availability" fields) on the "description" content.
It is also intresting that we can use a computer vision methods for a broad range of questions for this dataset, since there are many links, mapped to images, in this dataset.

---

### 8. What kinds of analysis would it _not_ support?

Although all the abovementioned types of analyzes are possible, there are some restrictions to them:
The analysis of fields, mentioned in the 5th answer will not give any useful information.
For the geospatial analyzis of the small territory we will probably get a very noisy result which cannot be interpreted. That happens due to the mentioned in the 3rd answer anonymization of the data: the point presented in the dataset is situated on the distance of 150 meters from the real location

---

### 9. Which of the uses presented in Q.7 and Q.8 are _ethical_?

Firsty, all methods that are not exactly ethical must be excluded. The last point about computer vision is not recommended for analysis, as well as any other method that uses the data. In article 1 [4], the author states "the choices offered to people can be In ways that closely involve them to consent" by tweeting. It would be logical to assume that, due to the specifics of the Airbnb platform, its the users (meaning the hosts) also have to share private information which they do not wish to share, which means that to use it unethically.
We consider other methods to be ethical. For the sake of proof, we will consider the six main ethical issues mentioned in article 2 [5] and show that they are not are related to the remaining methods:
1. Autonomous machines are threat to free will and responsibility
We are not going to build a autonomous machine, so the problem is irrelevant.

2. Bias, discrimination and exclusion
We do not use data to assess any person or group of people, so these concepts are not applicable. It can be argued that we will evaluate groups formed on the basis of geoposition, but since this will be the meaning of the study, bias will make sense and will not bring disparity.

3. Algorithmic profiling
Not one of the four methods cannot lead to a large personal benefit with no collective benefit, this problem is also irrelevant.
 
4. Preventing massive files while enhancing AI: seeking a new balance
We do not use a significant amount of data for any of the methods, and there is no indication that some methods will require an increase in data volume. The problem is irrelevant

5. Quality, quantity, relevance: the challenges of datacurated for AI
We recognise the potential for discrimination (it should be noted that this is no longer a question of discrimination as in the second paragraph, but rather that the data may be shifted in some direction), so we take this into account when we draw the conclusion.

6. Human identity before the challenge of artificial intelligence 
Not one of the methods is so powerful as to reduce human identity.

References:
[4] Kate Crawford & Megan, Finn The limits of crisis data: analytical and ethical challenges of using social and mobile data to understand disasters, GeoJournal, 01 November 2014
https://link.springer.com/article/10.1007%252Fs10708-014-9597-z#Sec7

[5] Ursula Garzcarek & Detlef Steuer, Approaching Ethical Guidelines for Data Scientists, Last updated January 16, 2019 
https://arxiv.org/pdf/1901.04824.pdf
