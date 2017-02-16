
## NLP Tools Comparison

### Table


<link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/v/dt/jq-2.2.4/dt-1.10.13/fc-3.2.2/fh-3.1.2/datatables.min.css"/>
<script type="text/javascript" src="https://cdn.datatables.net/v/dt/jq-2.2.4/dt-1.10.13/fc-3.2.2/fh-3.1.2/datatables.min.js"></script>
<script>
    $(document).ready(function() {
        $('table').DataTable({
            "paging":   false,
            "fixedColumns": true,
            
            "fixedHeader": false,
            "scrollX": true,
            "scrollY": '80vh',
            "class": "display"
        });
    } );
</script>

<style>
table.dataTable tbody tr {
    background: none !important;
    height: 150px !important;
}

table.DTFC_Cloned thead, table.DTFC_Cloned tfoot {
    background: none !important; 
}
</style>

<table border="1" class="dataframe cell-border compact">
  <thead>
    <tr>
      <th>name</th>
      <th>Meta</th>
      <th>Corpora</th>
      <th colspan="7" halign="left">Text processing</th>
      <th colspan="3" halign="left"></th>
      <th colspan="2" halign="left">Annotation</th>
      <th colspan="5" halign="left">ML</th>
      <th>visualization</th>
      <th colspan="2" halign="left">Multilanguage</th>
    </tr>
    <tr>
      <th></th>
      <th>github</th>
      <th></th>
      <th>Splitting</th>
      <th>Parsing</th>
      <th>Coreference resolution</th>
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
      <th>Language Identification</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href='https://textblob.readthedocs.io/en/dev/'>TextBlob</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/sloria/textblob.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAAftJREFUeJzt3LtOG0EYBeCztvEiyw6RpRRpEgoo8gJISCkWpPAieRh36SjoUkRJmZLKAleLjEQJDRcBkYIlx5Zvm73OpFhIbJnCEotmZnO+xtIUntPs0a/f1lpSSgkiIgUKqgMQ0f+LBZSRxv4ZPnxqqY5BZJSS6gB5sde6VB2ByDhGTkC7B+f4+PlYdQwieiIjC6gz9HFy01cd41FxIlRHIDKGkQVUtUsYBzF0/AHPixLVEYiMYWYBLZcQJRJBrN+04QUsIKJFGVlANTvdnY/8WHGSeV6oXyYiXRlZQNXltIDGgX4PuxdyAiJalJkFZC8BAMYaTkATDUuRSFdGFlDtfgIaBZHiJKlE/FuGcwlNtDgjC6h6vwPSZQKa3vtwCU1acV2g0Ug/NWTkP6Frmu2Afk/tfZ5jCS2lhJBAsWDNnCdCzp0R/eW6iLa2UYhCFGwbVrMJbG6qTjXDyAJ6mIC+HF3DvfilOA0wmSqdr+0btK96mX7/6c8huuMA79de4aFvYiHRPOvg3esXeFOvZHof5cPW92/YCUMUpQDCEDg8ZAFl4WWljI3VOn70PdwNfNVxAABv6xUM/QidgY9OxpliIRHGAu5Fd+ZcArjtebjteZneR/kwWFnHdmkJRRHDKpcBx1EdaY7F9wER5ZjrppOP42g3/QAsICJS6A+blrgxjxvcPAAAAABJRU5ErkJggg=="/></div></td>
      <td></td>
      <td>NLTK-tokenizers</td>
      <td>based on `pattern`</td>
      <td></td>
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
      <td><a href='http://textacy.readthedocs.io'>textacy</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/chartbeat-labs/textacy.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAAmxJREFUeJzt28tqE1Ecx/HvmZlcGmtJq7jwQi1050ooQtdd+xr6GuKmD+ALuHXhxq0UiopBqmAXdiFY01IrYnOhZpLM9e8iKelUWww0mYn9fzaTMJmZ/zlwfjlzkjEiIiilVAqstAtQSl1cGkBj8OjFJ+4/eZN2GUpljpN2ARfB07fVtEtQKpN0BqSUSo0G0Bjper9SSRpAY+SFcdolKJUpGkBj1PGjtEtQKlM0gMbI9cO0S1AqUzSAxqitMyClEjSARiyOBwvPGkBKJWkAjVg3HIRO29NbMKWO0wAaMdcbBJCrMyClEjSARuz4L1/t/2QRuhtEPP+wd2Z74lh4X60TRvrXg1RVKrC62ttmkJnEp+Gfbezybrv+5w6TfBtGQssLKeYsSnkHERD6zRWOXvGrG2IMzBRz1FyPrz9dlm7PYZ08XyxsfT9k8do0Uzk7se+0XjzsBrzc+gHA0vwsC1cvDdna9NRdn1LBQUTwwxg/ivGCmMp2DYA712e4UZ6iE0SUS3nytoUgiMBeo81GtcG9hTluzk4BYDAYc9YV1Xma/7zJw8cPcMIAq1CAtTVYXk67rISJfBasWmuzsdMPIElsEmxjmC46dIIILxh8Ex8NAmN6g6LgWFgGWv3bpViEypeDv17bsS0+7jaHqnf+SolWN2S/2WG/2RnqWOi1bZTj9rTzF3M2QRSTsy1yjkWhv717q8zmXpNWN2Sn3qboWFQPXGLp96mBgm1zueiw3+zwrZFss4hgJiCJBMEM0fMnPz/s8edt8fUrrCDAkhh8H9bXMxdAEzkDUkr9g0oFVlZ64ZPPZ3IGpAGklErNb64g8WWt5f+BAAAAAElFTkSuQmCC"/></div></td>
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
      <td></td>
    </tr>
    <tr>
      <td><a href='http://www.clips.ua.ac.be/pages/pattern-en'>pattern</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/clips/pattern.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAAV9JREFUeJzt271Kw1AAhuGvf7aWBrvVv1kHoXsXCS4i2CvwDkTQyQsR78DFobcgZIsIguIiuKh00iJIrLRpbByKU9Sp9pzG97mCd/qSc0IycRzHAgADsqYDAPxfDBCQVr6vsFjSRzYnlcuS75suSmCAgLTyPOUGA+XioRSGkueZLkpggIC0cl1F+cLoDWhmRnJd00UJGS6hgfTa3TvWVudWzf0dqdEwnZOQNx0A4O9czK+qurGuZqNuOuVbHMGAFAt6kSqlgumMHzFAQEqF0VD9aCinZO9BhwECUqrbjyRJlSIDBGDCgt5ogBwGCMCkBf2BJHEEG7eT8wcdtq5NZwBW+3oDqjBA4/Uc9NW6bOsp6JlOAaz11rP/Dsjesl9s1xd0dHang9MrLVVnTecAVnp8eZckORZ/hp/KAVqpOdpcq+mm/ar7Ttd0DmCt+vKcFi1+SPMrBgBjpvIOCEA6fAJYcFdr2lk5IwAAAABJRU5ErkJggg=="/></div></td>
      <td>contains API's (Google, Gmail, Bing, Twitter, Facebook, Wikipedia, Wiktionary, DBPedia, Flickr, ...), a robust HTML DOM parser and a web crawler.</td>
      <td></td>
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
      <td><a href='http://pymorphy2.readthedocs.io/en/latest/'>pymorphy2</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/kmike/pymorphy2.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAAi5JREFUeJzt3L9rE2Ecx/F37prEWC3WFqkV0XYQFdShiwXB6NjBWUR06D/gHyF0dhIXFyf/BaFwIhoR7aYotFYLYqpJL01y+XGXu8fhAiI1BDHlSZ77vpbbHj7c8OH7fOEupZRSCCGEBpbuAEKI5DKugF6tl1h68IJWEOqOIoTow7gCWtty+fC9yna1pTuKEKIP4wrIbQQAlD1fcxIhRD/GFVClW0A7dSkgIYadgQUUF89OQwpIiGFnXgE1uxOQXMGEgEIBVlbi5xAa0x1g0Nxu8UgBicQrFAiuXccKfOxsFlZXYXFRd6o/GDsBlWUHJJLOcbB8HzuKwPfBcXQn2sOoAlJKsdstIFd2QCLp8nkCO01o2ZDJQD6vO9EeRhVQrd0hjOIvS8r1tuY0QujlXlzg1s37vFu+N5TXLzBsB1Tx4unHSskOSIjNssfaiXPs3rkN52d0x/kroyagSjMundkjOX7W2zT8juZE/67WCtgseXTCSHcUMeK+lDwA5qbHNSfpbSQnoEfPN3j9uYxtWdgWTBxIA/CjFl+7blya5aGzwd3Hbzg9tb8v3/M7NP2QqUNZUv95VqgUz95vU293mJ8eZ+HU5EAyimT6WKxhpeDk5EHdUXoayQICKFZbhJEijBRN//eHp2dnDrN8ZY6JXJonha98c5v7miMzZpHL2Hwq1gZy3uX5o1w9c4ynb7d4uV4ayJkiuZYuHCebtnXH6Ckl/wMSQuhi1A5ICDFafgFp2MIpMxdPhAAAAABJRU5ErkJggg=="/></div></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>for Russian: singularize, pluralize, lemmatize</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>for Russian: morphology</td>
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
      <td><a href='http://pynlpl.readthedocs.io/en/latest/'>PyNLPl</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/proycon/pynlpl.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAAoBJREFUeJzt279u00AcB/Dv2UkcahEKLQplQaVISB0YEAMdmCox8SBMPAAPQAbeAImFAfEEHZAqVSAakaoDMFTQKmmiokDzv4lTJ25yDGncRFS1Aw52yvez+CSfTr+zfN/cWYqQUkoQEflA8bsAIvp/MYDIc+s7RSw8XUGp0fK7FAo4BhB57vnbr+h0Jb79bPhdCgUcA4g896Nm+l0CTQgGEHkufxxARuvI50oo6BhANDZGmwFEZ2MAkadMq2O3jVbnjJ5EDCDyWLVp2W0ewcgJA4g8VWm27XaDAUQOGEDkqcEA4g6InDCAyFNDRzB+hCYHDKBTHJgWnq1soW5azp1pSD+AtJCCBj9CkwMG0Clevs/gxbs0XiWzfpcycfpHsLlLUR7BgiCZBBKJ3jWAxCT+G/5NKoePmTIUIbBfNzGjR1Ay2hBCQBXA9FQEihDIlgx82qvi/s0ZxGNR1+Nv7JaRLTUxP6vj3o3LY5zJ+fPlew2ZooHFuRj2qod4cGv25KYABASEcD/eKG+nxEidUWi0oEdCmNLU4/J6hfXrG6HMvyYBbOUPcEWPIB6LQsqB+Qxc+su11x66DSkHnoAE5rc/40niMUJHFhRNA1ZXgaWlfzIft0J+F/AncuUmNrMVdLoSuqYiXTCgayoUIRBSBbb3G5ASiIYVPLpzHZvZCtIFw/X4EhILV3Uctjv4sFMc40zOp4eLcdy+dhGvUzmkdssQordY7AUjJYTLFJKQdjC4MUq4TV8II18zYVqd34LOj99lLayibjaH3lU7DO1QFEMB2X+O9rTFSfvuxjpUy4Iiu0C7DaytBS6AJnIHREQuJJPA8nIvfCKRQO6AGEBE5JtfbHL3aAiCQqoAAAAASUVORK5CYII="/></div></td>
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
      <td></td>
    </tr>
    <tr>
      <td><a href='https://github.com/JonathanRaiman/glove'>glove</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/JonathanRaiman/glove.svg?style=social'/> </div></td>
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
      <td>glove</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td><a href='https://github.com/mit-nlp/MITIE'>MITIE</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/mit-nlp/MITIE.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAABGNJREFUeJzt219oW1UAx/HvvblJ26zr2nXa2c2tE8GpzCrinw3Bh4qCoCA4UPRloDBBBEUfKvggg1aQMkGQWtSCbA+lgvpg1XVtt7KZ/atr1zmb2Xbr2q1t0jZpm783957rQ9csof9nsyT2fCAk988595xD+N1z700Uy7IsJEmS0kBNdwMkSVq7ZADdAW98c4oPG7vS3QxJyjgygO6Ak73j/NAxlO5mSFLGkQEkSVLayACSJCltZAClmBDyIaMkLUQGUIoFdSPdTZCkjCUDKMUC0VsBJH9yJUnJ1nwA/XZxhF5PIGX1BxMCKKSbKTuOJGWjNR1AQljsP9TB8wePp+wY05FbAZQ4G5KkVKk54qbN7Ul3M5ZlTQbQiX/G0A2BNxAFIJX3iRNDJ9sC6OzVCcJy1pZVoobJl6297Ks/m+6mLMuaC6COAR9vfnuag0cvc20iFF+feH9GNwRVTX9z3R9ecf0xUyTVlXgJFohkTwAN+ULsrXXx8Y/dANS19/Fr9/CqHsMUFlFj6YAb8oXYV3+GsZsnjMVEDfN/8+TRH9JpvjS64PYb/jAD48GkdQPjoQX2zkxrLoC6Bv0AnL/mYzAhgMaDevxzm9tDXXs/HzV28d2JK/hD+px65hOJmTxd1cKOyiZerf0Dy7KSLsGCWTQD6hjwAfD7XyOc7B2jqqmHdw7/uWiZth4PXYN+BidCvFbn4uvjfYvu/8nPF9lT3UrMFPSMTPFBQyeT4dic/b461keb20vD2cFF6wtGDR79tJmaZvcSvcsO7zd08vb35+Jj88XRy0nb93zWyrOfH0sK3MT7maawwOWC6uqZ9wykZOO/4Q+fHsDVN47DpqKqCsoKynZc89HvDVKYZ2dbsZMLQ5MA3LdpHSUFucSEIBAx6BmZjpfZuXk9u7ZsWLLu0eko7Ze98eUXd23mzBVf/Mz9zP2buGdD7gpamz7d1yeTxmDWK49tQVPnjnhQN2jqHgFmxmu27EvlpeRq85/nGm/+PaVi592cH/QzEdR5smwj24udSfud7Bvjhj9CWbGTJ8o2zltXzBT81Hkjvrz38a3L6GXq+UI6uXYbeXbbisvOjs8DJetxj86M53MPllDktCf194WHS3BoNkwh6PcG42P/bp6X96r2oxkx1JwcaGmB3btXqWerIysDqOaIm18uDKOb4ram28X5OUwEdSzL4pGthbxcXkptex9T4RiqohCJmRTk2QlEDVRFwRTWsh+h2zWV/ByNqXAMU1goikL5vYVcGQswGZp7ds9k24vXUeS0s+OufHo90/R7gwvO4hRFoaQgl6hhMhWO8fpT2zh31UfP8NSC9Ts0FWGBYQo028y4zTvbVKAwz7HkTLTQ6UA3BDFz5pUJnA4N3RQYt9Eem6qQo9kI6QZbi5w8VFpA86XR+HfRoakoioIhBJqqoqkKNlWhyOnAMx1hb/Mh3jpSj2YJsNngwAGorFztLv4nWRlAkiQtg8sFFRWg6+BwyBmQJElSon8B/4oAN7woBUEAAAAASUVORK5CYII="/></div></td>
      <td></td>
      <td>tokenizer</td>
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
      <td>- "bunch of different types of binary relation detector"</td>
      <td>yes</td>
      <td>yes</td>
      <td></td>
      <td></td>
      <td>pretrained word_feature_extractor</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td><a href='https://radimrehurek.com/gensim/'>gensim</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/RaRe-Technologies/gensim.svg?style=social'/> </div></td>
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
      <td>tf, tf-idf, word2vec</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td><a href=''>NLTK</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/nltk/nltk.svg?style=social'/> </div></td>
      <td></td>
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
      <td><a href='https://stopwords.readthedocs.io/en/latest/'>stopwords</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/astuanax/stopwords.svg?style=social'/> </div></td>
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
      <td></td>
    </tr>
    <tr>
      <td><a href='https://proycon.github.io/colibri-core/'>colibri-core</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/proycon/colibri-core.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAAkdJREFUeJzt2r9rE3EcxvH3JW1Sk9pKsdJ2EAeHVhB0UKguAXEQp+5O4qyIo67+C87qqIPQUZQEh2awS5BiIxaEYomJLZom1+R+OlQFTZUWL/km5/Pabvo8XMLnnvtyVhiGISIiBiRMBxCR/5cWkEhcFYs46RH8RBIyGSgWTSfqoAUkEleFAknXJRkG4DhQKJhO1EELSCSucjm8oeHdBpRKQS5nOlEHS4fQIvF16+YDcpUVFm5fg/l503E6DJkOICLdszwzS/LiBRbmz5iOsie9gonEmO14ZNP92zO0gERirOn4ZNNJ0zH+SAtIJKZcP8DxAjIpNSAR6TG77QOQTakBSYRq223TEWQANB0PgIzOgCQqS2ufOXf/BS/ffjIdRfqc/X0BqQFFrNH2WN+yf1432x71lmskSy8/o1rfsnm+srt4Xr2r9Wzufr2vNrj+8DWbDTU0k/KrVR4tfaDx4xWsjxtQ/yb7i7vP3lAo17g0d4yEZZFfreL6AZdPTZGwop1Vqbc4PDJEdo+DvJYXUChXOX9igolsKtrBvwmBxdIGjhcAkC/XsJ+WujrzoJbWNvn4ZYcbj5c5OTlqOk7XhMBqpc7R0TSTo2nTcX7R9gIWSxsAnD1+BKDr/81/MZBfQq/VGtx5UqJabwGw2XRw/YCpsZHIZ6WHk7h+QBDsfZtsxyfTo4pba7SZHj9Efcft2cyD2vjaYmY8+t+h71hgYfW0Ae/X7PQYYRhSrmxz5fQ0967OYVkRP5kjMpALSETiYSDPgEQkHr4BJfPG/9ubsFYAAAAASUVORK5CYII="/></div></td>
      <td></td>
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
      <td><a href='https://spacy.io/'>spaCy</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/spaCy/.svg?style=social'/> </div></td>
      <td></td>
      <td>- Non-destructive tokenization<br/>- Syntax-driven sentence segmentation</td>
      <td>"fast and accurate syntactic dependency parser"</td>
      <td></td>
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
      <td><a href='https://research.fb.com/projects/fasttext/'>fastText</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/facebookresearch/fastText.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAA4dJREFUeJzt299rW2Ucx/H3c5IlTduU9Ed0mHbrOkYnou5iTssQlILghTcDES8UJmX+DQWvtoteCOqNP27EeaFeeeHNnMXohDXFDabVtetCprU/bNqmaX41aU5Oz+NF2tjgtIsIZyd+XzffcJ7n4ptD+OT7HDhKa60RQggHGE43IIT4/2qKALoxv8Fzb39HoWw53YoQogHNEUC/bRBfKTCX2nS6FSFEA5oigFIFc6eWHe5ECNGIpgig9Z3gWctLAAnhJk0RQOnN3QnIdLgTIUQjmiKAdo9ecgQTwl2aIoDWN+UZkBBu1BwBJA+hhXAlVwZQtljhx4UMAEXTolTZBuQhtBBu48oAeuOLm4x8fB3b1rXpx+81/jGAfl7MyoQkxH3GlQE0fPwBUgWTqcVMLVQGwm1kShWsbfsv++fXi5x5f4JXP7xG5S7rQghnuDKAnhkM41GK6K3V2gR0NNyO1jCfLtbt1Vrz5vhtbA0zyznGLs2y9/3bb2ZXeGv8Nls7x7i/o7Umlkjx/S/rmNa9hVgskeLFD2LcWSs0+A3/W4WyRWLV2R6EQyYnYWysWu9Dyq1vw595b4L5dJG+rlZ+mM8w+vxxxr6cxVDweF+IeDLPY70hPIbiaiLF2dP95EoVPr+xxKORDg51taHRXL6ZxNbQ2xng5OFOvJ5qJqcKZa7/muZkfxfhoJ/lbImJxDoAkVCAoaPdqH16vDydJL9l0dsZ4KmBbnbvtKb2oVbyWxaGgmDLATQarauhZ+vquq01Wlev27Va3fPnerWalk2rz0N3ux+t4WpijZVcmWcHw2xVbGaTOU4d6aKj5cC/vv+ZUoWFdJFjDwbxe135P9b0DseneP38ObxWBcPvh2gUhoacbquOawPo0k/LvBONU7Zsetr9fDLyJNO/5/h6ZoUr8VUGD3Yws5SlWNnm5VOHOPf0AErBxdgcX00nSW+a2BoePhjkhRMP8dm1Be7smRJ8XoMTfSGmFjOUKzYeQ/HSE330d7dyMTbH0kZp3x57gn5eO32Ed79NUDTrJyyl6murz4u2NYWyhWEolAJDKQylUDv7DKX21Op1wwADBbvXd3rPb1lkiiZKKSKhAI9EOojeWiXY4mWgp42pxexdj6v3qsXnIRIKMJfaxHblL6j5vXLlU0bGP8KrbfB44MIFGB11uq06rg0gIcQ+JidheBhME3w+mYCEEGKvPwBrb5gSWGfLyAAAAABJRU5ErkJggg=="/></div></td>
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
      <td>yes</td>
      <td></td>
      <td></td>
      <td>skipgram, cbow</td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td><a href='https://www.tensorflow.org/tutorials/syntaxnet'>SyntaxNet</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/master/syntaxnet.svg?style=social'/> </div></td>
      <td></td>
      <td>tokenizer</td>
      <td>"transition-based dependency parser"</td>
      <td></td>
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
      <td><a href='https://github.com/saffsd/langid.py'>langid</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/nan.svg?style=social'/> </div></td>
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
      <td>pre-trained for 97 languages</td>
    </tr>
    <tr>
      <td><a href='http://stanfordnlp.github.io/CoreNLP/'>CoreNLP</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/nan.svg?style=social'/> </div></td>
      <td></td>
      <td>tokenizer</td>
      <td>yes</td>
      <td>"multi-pass sieve coreference resolution"</td>
      <td>lemmatize</td>
      <td>Pattern-based entity extraction</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td>POS</td>
      <td>- NER with "CRF sequence models"<br/>- "Open information extraction"<br/></td>
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
      <td><a href='https://github.com/BLLIP/bllip-parser'>bllip-parser</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/BLLIP/bllip-parser.svg?style=social'/> <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAASCAYAAAD7RgOSAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAABE9JREFUeJztmktv41QYhl/fj2OnTpNSkil/gQXL2c38G5as2fIT+AVs2LJmMdKwGcEgISF2CAkJkmmh09opiR1fDwtf4pNLNYG4iTvfI1knjuPIluzH7/cdS5xzDoIgiAMgH/oACIJ4f1EPfQAEQfw/pkGMiRtg4gWYuD4mXoCxG8D+6Ud88eVn0NIYCjOAFy+Ap08PfbgCJCCCOGI457iZRxi7QSEZv5LN2M2XWZgI+xiqjKHD8OnvP0PLYig8A6IIePmSBEQQxJI04/jrblGkl1IsfiWcN9MAizgT9rENFUOHYeQwfHzhYNRjGJ4wjBwTQ4fhtKNBkiRon0iQv/0KPIog6Trw7NlhTvIepDY2oedhAk2RoavUwiKOmyjJcDkNKqGMvWWSGbsBrqYLJJl4C552tEomQ4dhdFKMPYbRiQmbvXtu0F5/j9PXryA9f3506QdoqYA+/+YXfP3DH+gyFQNLx8A20Ld0nNk6+paOvmUU3+frAyvfTsIi9o0fJZVYlmVS0YtxA/w9C1G/w2QJOLONKsGUohk5eYoZOgxMU/Z6jOddA5Ik7fU/90UrBfTdr9d49dtb3M4juH4Ez4+r0fNjpFtOqcvUQki5pJbCymVViqoUl6Hu90Ig2gXnHNMgzsXi1eWSl0kTL4Drx8I+qizlyaVMLWWKcUyMHIbzrgFVedgHIQmoAd7OQqTZ+qFnnOOfRQJ3RU6uH8NbGV0/wtSP1yJwiW0shTWw81TVt/Vauiq+K5Z9P7mIZuGc43oWFkIJ1vowEy/APEyFfZgmF2nFrORSF82ZbUA+spudBNQA2wS0K7wU1qqcagLz/Bi3fgSvWN8mLMtQqhR1bzlYSIyE1SxJmuHqbiEkl+XskY830wWiRGzwnjC1kkrZ2B3VJOOY2tHezNsgATXAvgS0K5xzzMIE7jxeSVjrAiu3bRWWrlTp6azoY1UJqyaqcjsJS2QRp7icLvK0Ui+PivHqbrF2jQwsXUgu9dmjocNgG49vYpgE1ACHEtCucM4xD9MqQVWS2iCw8nOcbj6vTiGseuN9UzlY9rNMvd3CmoWJ8O7LuD6L5Aa4noXC72UJOO8yYfZo1Cs/m/jQMd7Lvh4JqAHaIqBd4ZxjHqVCgqqXgJsEFqXZxv8yNaUmpEJStVRVF9fA1tHRH+7pzzmH55cNXn9DDybANBAbvJoiVTIRei+FaD7oGlBlmulchQTUAI9VQLvCOYcfpWIJeE+68vwYYbJZWEyT83KvKP+E0nC1GW/p6OjK1gs7y/IG77je1F2RjB+JDd6OrtTKIrE0GjkMfUs/ugZvGyABNQAJ6L9RCutd05XrR1uFZaiykK4cU8PNPMSftwEup8FaKemYmvC+y+q7MCdMPdobpc2QgBqA5PMwlMK6nUfVcjMPcVNfn+XjXRCjb+l40jPx0amJi56JJ8V40TNhPcIGbxtQ5OOUD9BiAREE0X6oY0cQxMH4FzVHSqsyXln/AAAAAElFTkSuQmCC"/></div></td>
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
      <td></td>
    </tr>
    <tr>
      <td><a href='http://www.clips.ua.ac.be/pages/MBSP'>MBSP</a></td>
      <td><div style='margin: 0 auto;'><img src='https://img.shields.io/github/stars/nan.svg?style=social'/> </div></td>
      <td></td>
      <td>Regex-based segmentation<br/>Regex-bases tokenization</td>
      <td></td>
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
