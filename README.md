#  <div align="center"> Contradictory-My Dear Watson </div>

# About
This project is a part of Kaggle Challenge <a href="https://www.kaggle.com/c/contradictory-my-dear-watson">Contradictory - My Dear Watson</a> in which I classified a phrase into 3 classes on the basis of its context. Classes:-
1. Neutral
2. Entailment
3. Contradictory

# Tech Stack Used
<ul>
<li>Numpy</li>
<li>Pandas</li>
<li>NLP</li>
<li>Matplotlib</li>
<li>Keras</li>
<li>Re</li>
<li>NLTK</li>
<li>string</li>
<li>pickle</li>
<li>Tensorflow</li>
<li>Pytorch</li>
<li>Glove Embeddings</li>
<li>Cosine Similarity</li>
</ul>

# Model Structure
<pre>
(NLP)                                                      (NLP)
Input (456,50)                                            Input (34,50)
  |                                                        |
  |                                                        |
LSTM (output_dim = 256,512)                          LSTM (ouput_dim=256,512)
  |                                                        |
  |                                                        |
Flatten                                                 Flatten
  |_________________________      __________________________|
                           |     |
                           |     |
                        Cosine Similarity
                             |
                             |
                           Dense
                             |
                             |
                           Dense (3)
                          (output)
</pre>
