
### NLP Tools Comparison
### Table

<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="min-width: 200;"></th>
      <th style="min-width: 200;">name</th>
      <th style="min-width: 200;">Corpora</th>
      <th colspan="6" halign="left"style="min-width: 200;">Text processing</th>
      <th colspan="3" halign="left"style="min-width: 200;"></th>
      <th colspan="2" halign="left"style="min-width: 200;">Annotation</th>
      <th colspan="5" halign="left"style="min-width: 200;">ML</th>
      <th style="min-width: 200;">visualization</th>
      <th colspan="2" halign="left"style="min-width: 200;">Multilanguage</th>
    </tr>
    <tr>
      <th style="min-width: 200;"></th>
      <th style="min-width: 200;"></th>
      <th style="min-width: 200;"></th>
      <th style="min-width: 200;">Splitting</th>
      <th style="min-width: 200;">Parsing</th>
      <th style="min-width: 200;">Word inflection</th>
      <th style="min-width: 200;">Pattern Matching</th>
      <th style="min-width: 200;">X-grams</th>
      <th style="min-width: 200;">Spelling correction</th>
      <th style="min-width: 200;">WordNet</th>
      <th style="min-width: 200;">stopwords</th>
      <th style="min-width: 200;">statistics</th>
      <th style="min-width: 200;">Tagger</th>
      <th style="min-width: 200;">NER</th>
      <th style="min-width: 200;">Sentiment analysis</th>
      <th style="min-width: 200;">Classification</th>
      <th style="min-width: 200;">Clustering</th>
      <th style="min-width: 200;">Topic Modelling</th>
      <th style="min-width: 200;">Vectorization (including embeddings)</th>
      <th style="min-width: 200;"></th>
      <th style="min-width: 200;">Translation</th>
      <th style="min-width: 200;">Language Detection</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th style="min-width: 200;">0</th>
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
      <td>1) POS based on `pattern`\n2) POS based on NLTK‘s TreeBank tagger\n3) NP based on Shlomi Babluki’s implementation\n4) NP uses the CoNLL 2000 corpus to train a tagger</td>
      <td></td>
      <td>PatternAnalyzer (based on the `pattern`)\nNaiveBayesAnalyzer (an NLTK classifier trained on a movie reviews corpus)</td>
      <td>Naive Bayes, Decision Tree</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>powered by the Google Translate API</td>
      <td>powered by the Google Translate API</td>
    </tr>
    <tr>
      <th style="min-width: 200;">1</th>
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
      <th style="min-width: 200;">2</th>
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
      <td>POS (NN, VB, JJ, DT)\nChunks (NP)</td>
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
      <th style="min-width: 200;">3</th>
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
      <td>\n</td>
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
      <th style="min-width: 200;">4</th>
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
      <th style="min-width: 200;">5</th>
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
      <th style="min-width: 200;">6</th>
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
      <th style="min-width: 200;">7</th>
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
      <th style="min-width: 200;">8</th>
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
      <th style="min-width: 200;">9</th>
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
      <th style="min-width: 200;">10</th>
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
      <th style="min-width: 200;">11</th>
      <td><a href=''>spaCy\n</a></td>
      <td></td>
      <td>- Non-destructive tokenization\n- Syntax-driven sentence segmentation</td>
      <td>"fast and accurate syntactic dependency parser"</td>
      <td></td>
      <td>Rule-based matching</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>English and German tagging models with rule-based morphology</td>
      <td>> 10 built-in types\nStand-off format and token tags training</td>
      <td></td>
      <td>\n</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th style="min-width: 200;">12</th>
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
      <th style="min-width: 200;">13</th>
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
      <th style="min-width: 200;">14</th>
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
      <th style="min-width: 200;">15</th>
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
      <th style="min-width: 200;">16</th>
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
      <th style="min-width: 200;">17</th>
      <td><a href='http://www.clips.ua.ac.be/pages/MBSP'>MBSP</a></td>
      <td></td>
      <td>Regex-based segmentation\nRegex-bases tokenization</td>
      <td></td>
      <td>MBLEM-based lemmatization</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>POS (NN, JJ, VB)\nChunks (NP, VP)\nRelations (SBJ, OBJ)\n</td>
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