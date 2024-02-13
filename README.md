<h1>Sentiment Analysis of Restaurant Reviews</h1>

<p>This project demonstrates sentiment analysis on a dataset of restaurant reviews using various machine learning models and the VaderSentiment library. The goal is to classify reviews into positive or negative sentiments based on the review text.</p>

<h3>Prerequisites</h3>

<ul>
  <li>Python</li>
  <li>Pandas</li>
  <li>Scikit-learn</li>
  <li>VaderSentiment</li>
</ul>

<h3>Dataset</h3>

<p>The dataset used is <code>restaurant_reviews_az.csv</code> containing restaurant reviews with columns for review text, stars rating, and others. The dataset undergoes preprocessing to remove neutral reviews (3 stars), and a new binary <code>Sentiment</code> column is created indicating positive (1) or negative (0) sentiment.</p>

<h2>Implementation</h2>

<h3>Data Preprocessing</h3>

<ol>
  <li><strong>Filtering Reviews</strong>: Neutral reviews (3 stars) are removed from the dataset.</li>
  <li><strong>Sentiment Column</strong>: A binary <code>Sentiment</code> column is created to indicate positive or negative sentiment.</li>
</ol>

<h3>Feature Extraction</h3>

<ol>
  <li><strong>Count Vectorizer</strong>: Converts the collection of text documents to a matrix of token counts.</li>
  <li><strong>TF-IDF Vectorizer</strong>: Converts the collection of text documents to a matrix of TF-IDF features.</li>
</ol>

<h3>Models</h3>

<ol>
  <li><strong>Naive Bayes</strong>: Both Count Vectorizer and TF-IDF Vectorizer features are used to train a Naive Bayes classifier.</li>
  <li><strong>Support Vector Machine (SVM)</strong>: SVM models are trained using both Count Vectorizer and TF-IDF Vectorizer features.</li>
  <li><strong>VaderSentiment</strong>: The VaderSentiment library is used to predict the sentiment of reviews based on the compound score.</li>
</ol>

<h3>Evaluation</h3>

<p>The models are evaluated using accuracy score and classification report metrics.</p>

<h2>Results</h2>

<ul>
  <li>The SVM model with TF-IDF features showed the highest accuracy among the models tested.</li>
  <li>VaderSentiment provided a quick and effective way to analyze sentiments without the need for training.</li>
</ul>
