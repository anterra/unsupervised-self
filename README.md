### Metis Project 4: NLP & Unsupervised Learning

# The Unsupervised Self

## East Meets West and New Meets Old: A Machine Learning Approach to the Mind-Body Problem

### Anterra Kennedy

## Context and Goal

The development of Artificial Intelligence brings renewed interest to an ages old question -- the nature of consciousness. In answering the 'hard' problem of consciousness, the western world and neuroscience leans pretty heavily toward physical monism -- that mind is simply derived from brain, no more.

However, the 20th century breakthroughs in quantum mechanics created a paradigm shift in how we concieve of reality and, indeed, consciousness. I wanted to investigate whether these quantum metaphysical implications of consciousness could be correlated to descriptions of the same as found in Eastern religion and philosphy.

I believe that a convergence of those descriptions could provide new insight and a direction of future investigation, and that Machine Learning can be used to find these correlations.

## Methodologies

I used natural language processing and unsupervised learning as an approach to the mind-body problem and the nature of consciousness.

Workflow:

- Gather documents (PDFS, HTML and TXT files)
  - Both primary (such as the Upanishads, the Tao te Ching, the Vedas) and secondary documents (such as interpretations of the Abhidhamma as it relates to consciousness, articles on implications of quantum theory on consciousness by quantum physicists)
- Strip text from documents
- NLP pre-processing:
  - removal of non-english words
  - count-vectorizing: best to maintain importance of commonly used words such as "consciousness", so I decided to forgo TF-IDF after trying it.
  - SpaCy lemmatization (most effective out of all tried)
  - stop_words and min_df (min_df set to 0.02 yielded best topics)
- Topic Modeling
  - LSA/NMF as baseline
  - CorEx with anchoring to see how same terms (i.e. "consciousness") were used in different contexts
  - Best Model: LDA, optimized it
- Visualization
  - pyLDAvis for visualizing topic similarity and most important terms
  - Document Type similarity with PCA and t-SNE

## Findings, Implications and Conclusions

With these methods, I derived strong correlations between the descriptions of consciousness and Self as described in very Eastern Religion/Philosophical texts, and interpretations of Quantum Mechanics.

Further more, I found that the words used within those common topics tended toward monistic idealism, the idea that the only thing that exists is pure (non-physical) consciousness.

This could have huge future implications. As we further develop AI and quantum computing, the issue of consciousness could become very important, and if we integrate Eastern Teachings into our approach to quantum theory, (if as seen here they are indeed so similar), we could perhaps see huge innovation.

## Deliverables

Sequentially:

- [Stripping Text from Documents](https://github.com/anterra/unsupervised-self/tree/master/Creating%20Documents)
- [Machine Learning & Analysis](https://github.com/anterra/unsupervised-self/blob/master/analysis.ipynb)
- [Presentation Slides](https://github.com/anterra/unsupervised-self/blob/master/The%20Unsupervised%20Self.pdf)
- Interactive pyLDAvis: download and open vis_data.html

## Project Team

- [Anterra Kennedy](https://www.linkedin.com/in/anterrakennedy/)

## Technologies Used

- NLTK
- Gensim
- SpaCy
- CorEx
- pyLDAvis
- t-SNE
- Jupyter Notebook
- Python
- Pandas
- Scikit-learn
- Matplotlib
- pyPDF2
- textract

## Skills Demonstrated

- Natural Language Processing
- Unsupervised Learning
- Dimensionality Reduction
- Topic Modeling
- Clustering
- Visualization

## Resources

Texts used for analysis:

- "The Abhidhamma in Practice", NKG Mendis
- "The Brahma Sutras", Sage Vyasa
- "The Finer Scale of Consciousness: Quantum Theory", Tianwen Li et al., _US National Library of Medicine_
- "Mind and Consciousness in Yoga - Vedanta: A Comparative Analysis with Western Psychological Concepts", H.R. Aravindu Prabhu and P.S Bhat, _US National Library of Medicine_
- "A Comprehensive Manual of Abhidhamma: The Philosophical Psychology of Buddhism", Bhikkhu Bodhi, _Buddhist Publication Society_
- "Brahma Sutras: Translation and Commentary", Sri Swami Sivananda
- "The Four Vedas", Sage Vyasa
- "Consciousness, Mind and Matter in Indian Philosophy", Syamali Hari, _Journal of Consciousness Exploration & Research, 2010, Vol 1, Issue 6_
- "Information-Consciousness-Reality", James B. Glattfelder, _Springer Open_
- "Process of Consciousness and Matter", Bhaddanta Dr. Rewata Dhamma, (Companion to A Comprehensive Manual of Abhidhamma)
- "Quantum Physics in Consciousness Studies", Dirk K. F. Meijer and Simon Raggett (Review &Literature Compilation of 20 different studies by different authors), _Quantum Mind UK, University of Groningen_
- "Selfhood and Identity in Confucianism, Taoism, Buddhism, and Hinduism: Contrasts with the West", David Y. F. Ho, _Journal for the Theory of Social Behaviour, Vol. 25, Issue 2_
- "The Tao Te Ching", Lao Tzu
- "The Universe, Quantum Physics, and Consciousness", Subhash Kak, _Journal of Cosmology, 2009, Vol 3_
- "108 Upanishads", Unknown/Ambiguous/Attributed to Multiple Authors
- "Quantum Approaches to Consciousness", Harald Atmanspacher, _The Stanford Encyclopedia of Philosophy_
- "The Yoga Sutras of Patanjali" - Sage Patanjali
