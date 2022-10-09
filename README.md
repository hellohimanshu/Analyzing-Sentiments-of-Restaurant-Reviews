
# Restaurant Review Classifier
This is a simple NLP project based on the [NLP section of A-Z Machine Learning Course on Udemy](https://www.udemy.com/machinelearning/learn/v4/t/lecture/6085634?start=0)

The objective of this exercise is to identify the best model for classifying the review comments of a restaurant. We clean the dataset and make vectors out of them according to the bag of words model.

## Index
#### 1. [Preprocessing](#preprocessing)
#### 2. [Word Cloud](#WC)
#### 3. [Feature Engineering](#FE)
#### 4. [Model Building](#RFC)
#### 5. [Evaluation](#predictor)
#### 6. [Conclusion](#conclusion)

<a id='preprocessing'></a>
### Preprocessing

##### Dataset

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Review</th>
      <th>Liked</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Wow... Loved this place.</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Crust is not good.</td>
      <td>0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Not tasty and the texture was just nasty.</td>
      <td>0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Stopped by during the late May bank holiday of...</td>
      <td>1</td>
    </tr>
    <tr>
      <th>4</th>
      <td>The selection on the menu was great and so wer...</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>



The dataset contains the review string followed by a binary flag indicating wheather the user liked it or not.

##### steps taken
- Removal of punctuations and symbols
- Removing the stop words
- Tokenizing after stemming the different words.
- Building the vectors from the induvidual reviews.



<a id='gnb'></a>

### Conclusion 

In conclusion, we can say that none of these methods do a perfect job in classifying the reviews perfectly. However we can say that the best result was obtained for Random Forest Classifier. And even better result was obtained from the predictor function which aggregates the three classifiers. Another one factor we need to consider is that this model was built on only very limited dataset and has its limitations. Altogether we are able to get fairly good results for a basic implementatio on a web 

### Video Link

