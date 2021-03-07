# Publicly available datasets 

## Dataset example:

- Link: [Google Dataset](https://www.google.com)

- Purpose (what would you use this dataset for, explain, a short paragraph): 
I would use this "dataset" (not really a dataset) to search for more details of extratestrial life. 

## Dataset 1:

- Link: [Netflix Dataset](https://www.kaggle.com/shivamb/netflix-shows)
- Purpose (what would you use this dataset for, explain, a short paragraph):
- I would use this dataset if I was a competitor of netflix to leverage my knowledge of what they do and do not have so that I can make more   intelligent decisions about what to add to my service.  One could also use it as a personal tool to better filter through possible film/tv   choices

## Dataset 2:

- Link: [Company Bankruptcy Prediction](https://www.kaggle.com/fedesoriano/company-bankruptcy-prediction)
- Purpose (what would you use this dataset for, explain, a short paragraph):
- I would use this dataset as an investment tool by having a model use it's contents in comparison with my stock portfolio to make sure that   I am not investing in companies with a high probability of bankruptcy.It could also be useful as a tool to cross check companies that I am   applying to to make sure I am not starting a position at a company facing likely bankruptcy 

## Dataset 3:

- Link: [Wall Street Bets Monitoring](https://www.kaggle.com/gpreda/reddit-wallstreetsbets-posts)
- Purpose (what would you use this dataset for, explain, a short paragraph): 
- I would also use this dataset as an ivestment tool. This subreddit is well known for posting DD and investment advice,         however it's often swarmed with bots and other irrelevant information so a dataset like this that actively logs each post can   be used to sift through the noise. By applying certain filters to the data such as account history, engagement, comapnies       you're interested in, etc. you could write a program that only notified you when relevant information was posted.

## Dataset 4:

- Link: [World Vaccination Progress](https://www.kaggle.com/gpreda/covid-world-vaccination-progress)
- Purpose (what would you use this dataset for, explain, a short paragraph): 
- I would use this dataset if I was working for one of the many industries harmed by Covid such as airlines, hotels,             restaurants, resorts, etc. By tracking the progress of world vaccination you would be able to more accurately decide when you   could plan on resuming business/ time promotions. 

## Dataset 5:

- Link: [Job Change Of Data Scientists](https://www.kaggle.com/arashnic/hr-analytics-job-change-of-data-scientists)
- Purpose (what would you use this dataset for, explain, a short paragraph): 
- I would use this dataset as a hiring tool to better sort candidates with the proper training and experience needed for the     position I am looking to fill. Because candidates entered relevant information about where they live, experience, etc it will make it much easier to sort them this way than interviewing each one.

# Dataset information


## Chosen dataset: ***dataset1***


```python
import pandas
```


```python
# You will now proceed with a serious of commands in the next cell(s) that demonstrate some level of manipulation of the dataset that you are interested, in my case dataset1

# As you enter and execute commands leave the outputs so that I can read the manipulation that you did. Use all of your python skills here that you wish

# As an example I am providing some commands that have absolutly nothing to do with a dataset but just to illustrate the capture in my Jupyter notebook

# Once done, you can save this Jupyter notebook as a markdown and this is what I want you to commit to your private repo. Once you have your assignment ready, invite me to your private repo
```


```python
list1 = range(1,11)
```


```python
for member in list1:
    print(f'{member}) Are we having fun yet? YES!')
```

    1) Are we having fun yet? YES!
    2) Are we having fun yet? YES!
    3) Are we having fun yet? YES!
    4) Are we having fun yet? YES!
    5) Are we having fun yet? YES!
    6) Are we having fun yet? YES!
    7) Are we having fun yet? YES!
    8) Are we having fun yet? YES!
    9) Are we having fun yet? YES!
    10) Are we having fun yet? YES!



```python
list1[3:-6]
```




    range(4, 5)




```python

```



```python
import pandas as pd
import numpy as np
```


```python
data = pd.read_csv(r"C:\Users\Isaiah\Desktop\netflix_titles.csv")
```


```python
data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>show_id</th>
      <th>type</th>
      <th>title</th>
      <th>director</th>
      <th>cast</th>
      <th>country</th>
      <th>date_added</th>
      <th>release_year</th>
      <th>rating</th>
      <th>duration</th>
      <th>listed_in</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>s1</td>
      <td>TV Show</td>
      <td>3%</td>
      <td>NaN</td>
      <td>João Miguel, Bianca Comparato, Michel Gomes, R...</td>
      <td>Brazil</td>
      <td>August 14, 2020</td>
      <td>2020</td>
      <td>TV-MA</td>
      <td>4 Seasons</td>
      <td>International TV Shows, TV Dramas, TV Sci-Fi &amp;...</td>
      <td>In a future where the elite inhabit an island ...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>s2</td>
      <td>Movie</td>
      <td>7:19</td>
      <td>Jorge Michel Grau</td>
      <td>Demián Bichir, Héctor Bonilla, Oscar Serrano, ...</td>
      <td>Mexico</td>
      <td>December 23, 2016</td>
      <td>2016</td>
      <td>TV-MA</td>
      <td>93 min</td>
      <td>Dramas, International Movies</td>
      <td>After a devastating earthquake hits Mexico Cit...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>s3</td>
      <td>Movie</td>
      <td>23:59</td>
      <td>Gilbert Chan</td>
      <td>Tedd Chan, Stella Chung, Henley Hii, Lawrence ...</td>
      <td>Singapore</td>
      <td>December 20, 2018</td>
      <td>2011</td>
      <td>R</td>
      <td>78 min</td>
      <td>Horror Movies, International Movies</td>
      <td>When an army recruit is found dead, his fellow...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>s4</td>
      <td>Movie</td>
      <td>9</td>
      <td>Shane Acker</td>
      <td>Elijah Wood, John C. Reilly, Jennifer Connelly...</td>
      <td>United States</td>
      <td>November 16, 2017</td>
      <td>2009</td>
      <td>PG-13</td>
      <td>80 min</td>
      <td>Action &amp; Adventure, Independent Movies, Sci-Fi...</td>
      <td>In a postapocalyptic world, rag-doll robots hi...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>s5</td>
      <td>Movie</td>
      <td>21</td>
      <td>Robert Luketic</td>
      <td>Jim Sturgess, Kevin Spacey, Kate Bosworth, Aar...</td>
      <td>United States</td>
      <td>January 1, 2020</td>
      <td>2008</td>
      <td>PG-13</td>
      <td>123 min</td>
      <td>Dramas</td>
      <td>A brilliant group of students become card-coun...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>7782</th>
      <td>s7783</td>
      <td>Movie</td>
      <td>Zozo</td>
      <td>Josef Fares</td>
      <td>Imad Creidi, Antoinette Turk, Elias Gergi, Car...</td>
      <td>Sweden, Czech Republic, United Kingdom, Denmar...</td>
      <td>October 19, 2020</td>
      <td>2005</td>
      <td>TV-MA</td>
      <td>99 min</td>
      <td>Dramas, International Movies</td>
      <td>When Lebanon's Civil War deprives Zozo of his ...</td>
    </tr>
    <tr>
      <th>7783</th>
      <td>s7784</td>
      <td>Movie</td>
      <td>Zubaan</td>
      <td>Mozez Singh</td>
      <td>Vicky Kaushal, Sarah-Jane Dias, Raaghav Chanan...</td>
      <td>India</td>
      <td>March 2, 2019</td>
      <td>2015</td>
      <td>TV-14</td>
      <td>111 min</td>
      <td>Dramas, International Movies, Music &amp; Musicals</td>
      <td>A scrappy but poor boy worms his way into a ty...</td>
    </tr>
    <tr>
      <th>7784</th>
      <td>s7785</td>
      <td>Movie</td>
      <td>Zulu Man in Japan</td>
      <td>NaN</td>
      <td>Nasty C</td>
      <td>NaN</td>
      <td>September 25, 2020</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>44 min</td>
      <td>Documentaries, International Movies, Music &amp; M...</td>
      <td>In this documentary, South African rapper Nast...</td>
    </tr>
    <tr>
      <th>7785</th>
      <td>s7786</td>
      <td>TV Show</td>
      <td>Zumbo's Just Desserts</td>
      <td>NaN</td>
      <td>Adriano Zumbo, Rachel Khoo</td>
      <td>Australia</td>
      <td>October 31, 2020</td>
      <td>2019</td>
      <td>TV-PG</td>
      <td>1 Season</td>
      <td>International TV Shows, Reality TV</td>
      <td>Dessert wizard Adriano Zumbo looks for the nex...</td>
    </tr>
    <tr>
      <th>7786</th>
      <td>s7787</td>
      <td>Movie</td>
      <td>ZZ TOP: THAT LITTLE OL' BAND FROM TEXAS</td>
      <td>Sam Dunn</td>
      <td>NaN</td>
      <td>United Kingdom, Canada, United States</td>
      <td>March 1, 2020</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>90 min</td>
      <td>Documentaries, Music &amp; Musicals</td>
      <td>This documentary delves into the mystique behi...</td>
    </tr>
  </tbody>
</table>
<p>7787 rows × 12 columns</p>
</div>




```python
shows = data.groupby(data.type)
shows_df = shows.get_group("TV Show")
shows_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>show_id</th>
      <th>type</th>
      <th>title</th>
      <th>director</th>
      <th>cast</th>
      <th>country</th>
      <th>date_added</th>
      <th>release_year</th>
      <th>rating</th>
      <th>duration</th>
      <th>listed_in</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>s1</td>
      <td>TV Show</td>
      <td>3%</td>
      <td>NaN</td>
      <td>João Miguel, Bianca Comparato, Michel Gomes, R...</td>
      <td>Brazil</td>
      <td>August 14, 2020</td>
      <td>2020</td>
      <td>TV-MA</td>
      <td>4 Seasons</td>
      <td>International TV Shows, TV Dramas, TV Sci-Fi &amp;...</td>
      <td>In a future where the elite inhabit an island ...</td>
    </tr>
    <tr>
      <th>5</th>
      <td>s6</td>
      <td>TV Show</td>
      <td>46</td>
      <td>Serdar Akar</td>
      <td>Erdal Beşikçioğlu, Yasemin Allen, Melis Birkan...</td>
      <td>Turkey</td>
      <td>July 1, 2017</td>
      <td>2016</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>International TV Shows, TV Dramas, TV Mysteries</td>
      <td>A genetics professor experiments with a treatm...</td>
    </tr>
    <tr>
      <th>11</th>
      <td>s12</td>
      <td>TV Show</td>
      <td>1983</td>
      <td>NaN</td>
      <td>Robert Więckiewicz, Maciej Musiał, Michalina O...</td>
      <td>Poland, United States</td>
      <td>November 30, 2018</td>
      <td>2018</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>Crime TV Shows, International TV Shows, TV Dramas</td>
      <td>In this dark alt-history thriller, a naïve law...</td>
    </tr>
    <tr>
      <th>12</th>
      <td>s13</td>
      <td>TV Show</td>
      <td>1994</td>
      <td>Diego Enrique Osorno</td>
      <td>NaN</td>
      <td>Mexico</td>
      <td>May 17, 2019</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>Crime TV Shows, Docuseries, International TV S...</td>
      <td>Archival video and new interviews examine Mexi...</td>
    </tr>
    <tr>
      <th>16</th>
      <td>s17</td>
      <td>TV Show</td>
      <td>Feb-09</td>
      <td>NaN</td>
      <td>Shahd El Yaseen, Shaila Sabt, Hala, Hanadi Al-...</td>
      <td>NaN</td>
      <td>March 20, 2019</td>
      <td>2018</td>
      <td>TV-14</td>
      <td>1 Season</td>
      <td>International TV Shows, TV Dramas</td>
      <td>As a psychology professor faces Alzheimer's, h...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>7767</th>
      <td>s7768</td>
      <td>TV Show</td>
      <td>Zindagi Gulzar Hai</td>
      <td>NaN</td>
      <td>Sanam Saeed, Fawad Khan, Ayesha Omer, Mehreen ...</td>
      <td>Pakistan</td>
      <td>December 15, 2016</td>
      <td>2012</td>
      <td>TV-PG</td>
      <td>1 Season</td>
      <td>International TV Shows, Romantic TV Shows, TV ...</td>
      <td>Strong-willed, middle-class Kashaf and carefre...</td>
    </tr>
    <tr>
      <th>7775</th>
      <td>s7776</td>
      <td>TV Show</td>
      <td>Zoids Wild</td>
      <td>NaN</td>
      <td>Kensho Ono, Takahiro Sakurai, Mikako Komatsu, ...</td>
      <td>Japan</td>
      <td>August 14, 2020</td>
      <td>2018</td>
      <td>TV-Y7</td>
      <td>1 Season</td>
      <td>Anime Series, Kids' TV</td>
      <td>A quest for freedom and legendary treasure beg...</td>
    </tr>
    <tr>
      <th>7777</th>
      <td>s7778</td>
      <td>TV Show</td>
      <td>Zombie Dumb</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>July 1, 2019</td>
      <td>2018</td>
      <td>TV-Y7</td>
      <td>2 Seasons</td>
      <td>Kids' TV, Korean TV Shows, TV Comedies</td>
      <td>While living alone in a spooky town, a young g...</td>
    </tr>
    <tr>
      <th>7779</th>
      <td>s7780</td>
      <td>TV Show</td>
      <td>Zona Rosa</td>
      <td>NaN</td>
      <td>Manu NNa, Ana Julia Yeyé, Ray Contreras, Pablo...</td>
      <td>Mexico</td>
      <td>November 26, 2019</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>International TV Shows, Spanish-Language TV Sh...</td>
      <td>An assortment of talent takes the stage for a ...</td>
    </tr>
    <tr>
      <th>7785</th>
      <td>s7786</td>
      <td>TV Show</td>
      <td>Zumbo's Just Desserts</td>
      <td>NaN</td>
      <td>Adriano Zumbo, Rachel Khoo</td>
      <td>Australia</td>
      <td>October 31, 2020</td>
      <td>2019</td>
      <td>TV-PG</td>
      <td>1 Season</td>
      <td>International TV Shows, Reality TV</td>
      <td>Dessert wizard Adriano Zumbo looks for the nex...</td>
    </tr>
  </tbody>
</table>
<p>2410 rows × 12 columns</p>
</div>




```python
movies = data.groupby(data.type)
movies_df = movies.get_group("Movie")
movies_df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>show_id</th>
      <th>type</th>
      <th>title</th>
      <th>director</th>
      <th>cast</th>
      <th>country</th>
      <th>date_added</th>
      <th>release_year</th>
      <th>rating</th>
      <th>duration</th>
      <th>listed_in</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>s2</td>
      <td>Movie</td>
      <td>7:19</td>
      <td>Jorge Michel Grau</td>
      <td>Demián Bichir, Héctor Bonilla, Oscar Serrano, ...</td>
      <td>Mexico</td>
      <td>December 23, 2016</td>
      <td>2016</td>
      <td>TV-MA</td>
      <td>93 min</td>
      <td>Dramas, International Movies</td>
      <td>After a devastating earthquake hits Mexico Cit...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>s3</td>
      <td>Movie</td>
      <td>23:59</td>
      <td>Gilbert Chan</td>
      <td>Tedd Chan, Stella Chung, Henley Hii, Lawrence ...</td>
      <td>Singapore</td>
      <td>December 20, 2018</td>
      <td>2011</td>
      <td>R</td>
      <td>78 min</td>
      <td>Horror Movies, International Movies</td>
      <td>When an army recruit is found dead, his fellow...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>s4</td>
      <td>Movie</td>
      <td>9</td>
      <td>Shane Acker</td>
      <td>Elijah Wood, John C. Reilly, Jennifer Connelly...</td>
      <td>United States</td>
      <td>November 16, 2017</td>
      <td>2009</td>
      <td>PG-13</td>
      <td>80 min</td>
      <td>Action &amp; Adventure, Independent Movies, Sci-Fi...</td>
      <td>In a postapocalyptic world, rag-doll robots hi...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>s5</td>
      <td>Movie</td>
      <td>21</td>
      <td>Robert Luketic</td>
      <td>Jim Sturgess, Kevin Spacey, Kate Bosworth, Aar...</td>
      <td>United States</td>
      <td>January 1, 2020</td>
      <td>2008</td>
      <td>PG-13</td>
      <td>123 min</td>
      <td>Dramas</td>
      <td>A brilliant group of students become card-coun...</td>
    </tr>
    <tr>
      <th>6</th>
      <td>s7</td>
      <td>Movie</td>
      <td>122</td>
      <td>Yasir Al Yasiri</td>
      <td>Amina Khalil, Ahmed Dawood, Tarek Lotfy, Ahmed...</td>
      <td>Egypt</td>
      <td>June 1, 2020</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>95 min</td>
      <td>Horror Movies, International Movies</td>
      <td>After an awful accident, a couple admitted to ...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>7781</th>
      <td>s7782</td>
      <td>Movie</td>
      <td>Zoom</td>
      <td>Peter Hewitt</td>
      <td>Tim Allen, Courteney Cox, Chevy Chase, Kate Ma...</td>
      <td>United States</td>
      <td>January 11, 2020</td>
      <td>2006</td>
      <td>PG</td>
      <td>88 min</td>
      <td>Children &amp; Family Movies, Comedies</td>
      <td>Dragged from civilian life, a former superhero...</td>
    </tr>
    <tr>
      <th>7782</th>
      <td>s7783</td>
      <td>Movie</td>
      <td>Zozo</td>
      <td>Josef Fares</td>
      <td>Imad Creidi, Antoinette Turk, Elias Gergi, Car...</td>
      <td>Sweden, Czech Republic, United Kingdom, Denmar...</td>
      <td>October 19, 2020</td>
      <td>2005</td>
      <td>TV-MA</td>
      <td>99 min</td>
      <td>Dramas, International Movies</td>
      <td>When Lebanon's Civil War deprives Zozo of his ...</td>
    </tr>
    <tr>
      <th>7783</th>
      <td>s7784</td>
      <td>Movie</td>
      <td>Zubaan</td>
      <td>Mozez Singh</td>
      <td>Vicky Kaushal, Sarah-Jane Dias, Raaghav Chanan...</td>
      <td>India</td>
      <td>March 2, 2019</td>
      <td>2015</td>
      <td>TV-14</td>
      <td>111 min</td>
      <td>Dramas, International Movies, Music &amp; Musicals</td>
      <td>A scrappy but poor boy worms his way into a ty...</td>
    </tr>
    <tr>
      <th>7784</th>
      <td>s7785</td>
      <td>Movie</td>
      <td>Zulu Man in Japan</td>
      <td>NaN</td>
      <td>Nasty C</td>
      <td>NaN</td>
      <td>September 25, 2020</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>44 min</td>
      <td>Documentaries, International Movies, Music &amp; M...</td>
      <td>In this documentary, South African rapper Nast...</td>
    </tr>
    <tr>
      <th>7786</th>
      <td>s7787</td>
      <td>Movie</td>
      <td>ZZ TOP: THAT LITTLE OL' BAND FROM TEXAS</td>
      <td>Sam Dunn</td>
      <td>NaN</td>
      <td>United Kingdom, Canada, United States</td>
      <td>March 1, 2020</td>
      <td>2019</td>
      <td>TV-MA</td>
      <td>90 min</td>
      <td>Documentaries, Music &amp; Musicals</td>
      <td>This documentary delves into the mystique behi...</td>
    </tr>
  </tbody>
</table>
<p>5377 rows × 12 columns</p>
</div>




```python
shows_df.sort_values(by=['release_year'])
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>show_id</th>
      <th>type</th>
      <th>title</th>
      <th>director</th>
      <th>cast</th>
      <th>country</th>
      <th>date_added</th>
      <th>release_year</th>
      <th>rating</th>
      <th>duration</th>
      <th>listed_in</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4867</th>
      <td>s4868</td>
      <td>TV Show</td>
      <td>Pioneers: First Women Filmmakers*</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>December 30, 2018</td>
      <td>1925</td>
      <td>TV-14</td>
      <td>1 Season</td>
      <td>TV Shows</td>
      <td>This collection restores films from women who ...</td>
    </tr>
    <tr>
      <th>4866</th>
      <td>s4867</td>
      <td>TV Show</td>
      <td>Pioneers of African-American Cinema</td>
      <td>Oscar Micheaux, Spencer Williams, Richard E. N...</td>
      <td>NaN</td>
      <td>United States</td>
      <td>February 1, 2017</td>
      <td>1946</td>
      <td>TV-14</td>
      <td>1 Season</td>
      <td>TV Shows</td>
      <td>This newly preserved collection features more ...</td>
    </tr>
    <tr>
      <th>6953</th>
      <td>s6954</td>
      <td>TV Show</td>
      <td>The Twilight Zone (Original Series)</td>
      <td>NaN</td>
      <td>Rod Serling</td>
      <td>United States</td>
      <td>July 1, 2017</td>
      <td>1963</td>
      <td>TV-14</td>
      <td>4 Seasons</td>
      <td>Classic &amp; Cult TV, TV Sci-Fi &amp; Fantasy</td>
      <td>Hosted by creator Rod Serling, this groundbrea...</td>
    </tr>
    <tr>
      <th>6082</th>
      <td>s6083</td>
      <td>TV Show</td>
      <td>The Andy Griffith Show</td>
      <td>NaN</td>
      <td>Andy Griffith, Ron Howard, Don Knotts, Frances...</td>
      <td>United States</td>
      <td>July 1, 2017</td>
      <td>1967</td>
      <td>TV-G</td>
      <td>8 Seasons</td>
      <td>Classic &amp; Cult TV, TV Comedies</td>
      <td>Homespun humor and easygoing Sheriff Andy Tayl...</td>
    </tr>
    <tr>
      <th>5785</th>
      <td>s5786</td>
      <td>TV Show</td>
      <td>Star Trek</td>
      <td>NaN</td>
      <td>William Shatner, Leonard Nimoy, DeForest Kelle...</td>
      <td>United States</td>
      <td>October 1, 2017</td>
      <td>1968</td>
      <td>TV-14</td>
      <td>3 Seasons</td>
      <td>Classic &amp; Cult TV, TV Action &amp; Adventure, TV S...</td>
      <td>Led by unflappable Capt. Kirk, the crew of the...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>980</th>
      <td>s981</td>
      <td>TV Show</td>
      <td>Bling Empire</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>January 15, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>Reality TV</td>
      <td>Follow LA's wildly wealthy Asian and Asian Ame...</td>
    </tr>
    <tr>
      <th>5921</th>
      <td>s5922</td>
      <td>TV Show</td>
      <td>Surviving Death</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>United States</td>
      <td>January 6, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>Docuseries, Reality TV</td>
      <td>What happens after we die? This docuseries exp...</td>
    </tr>
    <tr>
      <th>4390</th>
      <td>s4391</td>
      <td>TV Show</td>
      <td>Nailed It! Mexico</td>
      <td>NaN</td>
      <td>Omar Chaparro, Anna Ruiz</td>
      <td>Mexico, United States</td>
      <td>January 5, 2021</td>
      <td>2021</td>
      <td>TV-PG</td>
      <td>3 Seasons</td>
      <td>International TV Shows, Reality TV, Spanish-La...</td>
      <td>The fun, fondant and hilarious cake fails head...</td>
    </tr>
    <tr>
      <th>4965</th>
      <td>s4966</td>
      <td>TV Show</td>
      <td>Pretend It’s a City</td>
      <td>NaN</td>
      <td>Fran Lebowitz</td>
      <td>United States</td>
      <td>January 8, 2021</td>
      <td>2021</td>
      <td>TV-14</td>
      <td>1 Season</td>
      <td>Docuseries</td>
      <td>Wander the New York City streets and fascinati...</td>
    </tr>
    <tr>
      <th>2672</th>
      <td>s2673</td>
      <td>TV Show</td>
      <td>Headspace Guide to Meditation</td>
      <td>NaN</td>
      <td>Andy Puddicombe</td>
      <td>United States</td>
      <td>January 1, 2021</td>
      <td>2021</td>
      <td>TV-G</td>
      <td>1 Season</td>
      <td>Docuseries, Science &amp; Nature TV</td>
      <td>Headspace takes a friendly, animated look at t...</td>
    </tr>
  </tbody>
</table>
<p>2410 rows × 12 columns</p>
</div>




```python
movies_df.sort_values(by=['release_year'])
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>show_id</th>
      <th>type</th>
      <th>title</th>
      <th>director</th>
      <th>cast</th>
      <th>country</th>
      <th>date_added</th>
      <th>release_year</th>
      <th>rating</th>
      <th>duration</th>
      <th>listed_in</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4960</th>
      <td>s4961</td>
      <td>Movie</td>
      <td>Prelude to War</td>
      <td>Frank Capra</td>
      <td>NaN</td>
      <td>United States</td>
      <td>March 31, 2017</td>
      <td>1942</td>
      <td>TV-14</td>
      <td>52 min</td>
      <td>Classic Movies, Documentaries</td>
      <td>Frank Capra's documentary chronicles the rise ...</td>
    </tr>
    <tr>
      <th>6117</th>
      <td>s6118</td>
      <td>Movie</td>
      <td>The Battle of Midway</td>
      <td>John Ford</td>
      <td>Henry Fonda, Jane Darwell</td>
      <td>United States</td>
      <td>March 31, 2017</td>
      <td>1942</td>
      <td>TV-14</td>
      <td>18 min</td>
      <td>Classic Movies, Documentaries</td>
      <td>Director John Ford captures combat footage of ...</td>
    </tr>
    <tr>
      <th>7616</th>
      <td>s7617</td>
      <td>Movie</td>
      <td>Why We Fight: The Battle of Russia</td>
      <td>Frank Capra, Anatole Litvak</td>
      <td>NaN</td>
      <td>United States</td>
      <td>March 31, 2017</td>
      <td>1943</td>
      <td>TV-PG</td>
      <td>82 min</td>
      <td>Documentaries</td>
      <td>This installment of Frank Capra's acclaimed do...</td>
    </tr>
    <tr>
      <th>7342</th>
      <td>s7343</td>
      <td>Movie</td>
      <td>Undercover: How to Operate Behind Enemy Lines</td>
      <td>John Ford</td>
      <td>NaN</td>
      <td>United States</td>
      <td>March 31, 2017</td>
      <td>1943</td>
      <td>TV-PG</td>
      <td>61 min</td>
      <td>Classic Movies, Documentaries</td>
      <td>This World War II-era training film dramatizes...</td>
    </tr>
    <tr>
      <th>7679</th>
      <td>s7680</td>
      <td>Movie</td>
      <td>WWII: Report from the Aleutians</td>
      <td>John Huston</td>
      <td>NaN</td>
      <td>United States</td>
      <td>March 31, 2017</td>
      <td>1943</td>
      <td>TV-PG</td>
      <td>45 min</td>
      <td>Documentaries</td>
      <td>Filmmaker John Huston narrates this Oscar-nomi...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>7644</th>
      <td>s7645</td>
      <td>Movie</td>
      <td>Wish You</td>
      <td>Sung Do-jun</td>
      <td>Kang In-soo, Lee Sang, Soo-bin</td>
      <td>NaN</td>
      <td>January 15, 2021</td>
      <td>2021</td>
      <td>TV-PG</td>
      <td>102 min</td>
      <td>Dramas, International Movies, LGBTQ Movies</td>
      <td>Singing and dreaming together, a talented sing...</td>
    </tr>
    <tr>
      <th>1514</th>
      <td>s1515</td>
      <td>Movie</td>
      <td>Crack: Cocaine, Corruption &amp; Conspiracy</td>
      <td>Stanley Nelson</td>
      <td>NaN</td>
      <td>United States</td>
      <td>January 11, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>90 min</td>
      <td>Documentaries</td>
      <td>A cheap, powerful drug emerges during a recess...</td>
    </tr>
    <tr>
      <th>4710</th>
      <td>s4711</td>
      <td>Movie</td>
      <td>Outside the Wire</td>
      <td>Mikael Håfström</td>
      <td>Anthony Mackie, Damson Idris, Emily Beecham, M...</td>
      <td>NaN</td>
      <td>January 15, 2021</td>
      <td>2021</td>
      <td>R</td>
      <td>116 min</td>
      <td>Action &amp; Adventure</td>
      <td>In the near future, a drone pilot sent into a ...</td>
    </tr>
    <tr>
      <th>5103</th>
      <td>s5104</td>
      <td>Movie</td>
      <td>Ratones Paranoicos: The Band that Rocked Argen...</td>
      <td>Alejandro Ruax, Ramiro Martínez</td>
      <td>Juan Sebastián Gutiérrez, Pablo Cano, Pablo Me...</td>
      <td>NaN</td>
      <td>January 6, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>76 min</td>
      <td>Documentaries, International Movies, Music &amp; M...</td>
      <td>The irrepressible Ratones Paranoicos, Argentin...</td>
    </tr>
    <tr>
      <th>1355</th>
      <td>s1356</td>
      <td>Movie</td>
      <td>Chris Rock Total Blackout: The Tamborine Exten...</td>
      <td>Chris Rock</td>
      <td>Chris Rock</td>
      <td>NaN</td>
      <td>January 12, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>98 min</td>
      <td>Stand-Up Comedy</td>
      <td>In this extended cut of his 2018 special, Chri...</td>
    </tr>
  </tbody>
</table>
<p>5377 rows × 12 columns</p>
</div>




```python

```
