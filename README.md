
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
}

table.DTFC_Cloned thead, table.DTFC_Cloned tfoot {
    background: none !important; 
}
</style>

<table border="1" class="dataframe cell-border compact">
  <thead>
    <tr>
      <th>name</th>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
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
