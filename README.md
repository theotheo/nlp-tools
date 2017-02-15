
## NLP Tools Comparison

### Table

<table border="1" class="dataframe">
  <thead>
    <tr>
      <th></th>
      <th>name</th>
      <th>Corpora</th>
      <th colspan="6" halign="left">Text processing</th>
      <th colspan="3" halign="left"></th>
      <th colspan="2" halign="left">Annotation</th>
      <th colspan="5" halign="left">ML</th>
      <th>visualization</th>
      <th colspan="2" halign="left">Multilanguage</th>
    </tr>
    <tr>
      <th></th>
      <th></th>
      <th></th>
      <th>Splitting</th>
      <th>Parsing</th>
      <th>Word inflection</th>
      <th>Pattern Matching</th>
      <th>X-grams</th>
      <th>Spelling correction</th>
      <th>WordNet</th>
      <th>stopwords</th>
      <th>statistics</th>
      <th>Tagger</th>
      <th>NER</th>
      <th>Sentiment analysis</th>
      <th>Classification</th>
      <th>Clustering</th>
      <th>Topic Modelling</th>
      <th>Vectorization (including embeddings)</th>
      <th></th>
      <th>Translation</th>
      <th>Language Detection</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td><a href='https://textblob.readthedocs.io/en/dev/'>TextBlob</a></td>
      <td></td>
      <td>NLTK-tokenizers</td>
      <td>based on `pattern`</td>
      <td>singularize, pluralize, lemmatize</td>
      <td></td>
      <td></td>
      <td>based on `pattern`</td>
      <td>integration</td>
      <td></td>
      <td>Word and phrase frequencies</td>
      <td>1) POS based on `pattern`<br/>2) POS based on NLTK‘s TreeBank tagger<br/>3) NP based on Shlomi Babluki’s implementation<br/>4) NP uses the CoNLL 2000 corpus to train a tagger</td>
      <td></td>
      <td>PatternAnalyzer (based on the `pattern`)<br/>NaiveBayesAnalyzer (an NLTK classifier trained on a movie reviews corpus)</td>
      <td>Naive Bayes, Decision Tree</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>powered by the Google Translate API</td>
      <td>powered by the Google Translate API</td>
    </tr>
    <tr>
      <th>1</th>
      <td><a href='http://textacy.readthedocs.io'>textacy</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>2</th>
      <td><a href='http://www.clips.ua.ac.be/pages/pattern-en'>pattern</a></td>
      <td>contains API's (Google, Gmail, Bing, Twitter, Facebook, Wikipedia, Wiktionary, DBPedia, Flickr, ...), a robust HTML DOM parser and a web crawler.</td>
      <td></td>
      <td></td>
      <td>yes</td>
      <td>by POS-tags</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>POS (NN, VB, JJ, DT)<br/>Chunks (NP)</td>
      <td></td>
      <td></td>
      <td>Naive Bayes, Perceptron, k-NN, SVM</td>
      <td>k-means, hierarchical</td>
      <td>LSA</td>
      <td>td, df, idf, tf-idf,  cosine similarity, infogain</td>
      <td>graph.js on canvas</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>3</th>
      <td><a href=''>pymorphy2</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td>lemmatization</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td><br/></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>4</th>
      <td><a href='http://pynlpl.readthedocs.io/en/latest/'>PyNLPl</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>5</th>
      <td><a href='https://github.com/JonathanRaiman/glove'>glove</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>glove</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>6</th>
      <td><a href=''>MITIE</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>7</th>
      <td><a href=''>gensim</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>tf, tf-idf, word2vec</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>8</th>
      <td><a href=''>NLTK</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>n-grams</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>9</th>
      <td><a href='https://stopwords.readthedocs.io/en/latest/'>stopwords</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>10</th>
      <td><a href=''>colibri-core</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>n-grams, skipgrams, flexgrams</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>11</th>
      <td><a href=''>spaCy<br/></a></td>
      <td></td>
      <td>- Non-destructive tokenization<br/>- Syntax-driven sentence segmentation</td>
      <td>"fast and accurate syntactic dependency parser"</td>
      <td></td>
      <td>Rule-based matching</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>English and German tagging models with rule-based morphology</td>
      <td>> 10 built-in types<br/>Stand-off format and token tags training</td>
      <td></td>
      <td><br/></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>12</th>
      <td><a href='https://research.fb.com/projects/fasttext/'>fastText</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>yes</td>
      <td></td>
      <td></td>
      <td>skipgram, cbow</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>13</th>
      <td><a href=''>SyntaxNet</a></td>
      <td></td>
      <td></td>
      <td>yes</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>POS</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>14</th>
      <td><a href=''>langid</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>pre-trained for 97 languages</td>
    </tr>
    <tr>
      <th>15</th>
      <td><a href=''>corenlp-python</a></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>16</th>
      <td><a href=''>BLLIP</a></td>
      <td></td>
      <td></td>
      <td>"8 known unified parsing models", including models for web, news, PubMed texts</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>17</th>
      <td><a href='http://www.clips.ua.ac.be/pages/MBSP'>MBSP</a></td>
      <td></td>
      <td>Regex-based segmentation<br/>Regex-bases tokenization</td>
      <td></td>
      <td>MBLEM-based lemmatization</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>POS (NN, JJ, VB)<br/>Chunks (NP, VP)<br/>Relations (SBJ, OBJ)<br/></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>
