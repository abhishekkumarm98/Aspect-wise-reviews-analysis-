We have implemented Aspect wise reviews analysis and in order to do it, We have used YELP API to collect informations like ratings, address, latitude-longitude, categories and Urls.
With urls of restaurants, we collected reviews of all pages for each restaurant. 


We have used following modules to alleviate the task and fulfill our objective.

re:  A regular expression (or re) specifies a set of strings that matches it; the functions in this module let you check if a particular string matches a given regular expression or if a given regular expression matches a particular string. I have used it to fetch all name of restaurants and their latitude and longitude under patina group.

os:  It offers users to interact with operating system and I have used when I ran my entire code on google colab to reach the path of my drive.

folium: It is a powerful Python library that helps users to create several types of Leaflet maps. The fact that the Folium results are interactive makes this library very useful for dashboard building and the reason for I have used to point all restaurants within globe with the help of latitude and longitude.

codecs: It defines base classes for standard Python codecs (encoders and decoders) and provides access to the internal Python codec registry which manages the codec and error handling lookup process and I have employed it to decode the image while making mask, which has been passed as an argument in word cloud object.

base64: It encodes the bytes-like objects using Base64 and return a bytes object. The reason to use it to encode the image while making mask.

imageio: It provides an easy interface to read and write a wide range of image data, including animated images, volumetric data, and scientific formats. I used this to read the decoded image during making mask for word cloud.

nltk: It works with human language data and provides easy-to-use interfaces to over 50 corpora and lexical resources such as WordNet, along with a suite of text processing libraries for classification, tokenization, stemming, tagging, parsing, and semantic reasoning, wrappers for industrial-strength NLP libraries. I have used it for various purposes for removing stop words, lemmatizing and sentiment finding.

matplotlib: It is a plotting library for the Python programming language and its numerical mathematics extension NumPy. It provides an object-oriented API for embedding plots into applications using general-purpose GUI toolkits like Tkinter, wxPython, Qt, or GTK+ and majorly I have used for plotting.

mplcursors: It provides interactive data selection cursors for Matplotlib. It is inspired from mpldatacursor, with a much simplified API and I have employed this when I was making interactive plot with rating versus number of reviews.

json: It is a lightweight data interchange format inspired by JavaScript object literal syntax and I used it while pointing name of restaurant to encompass the USA map on a globe.

spacy: It is a free, open-source library for advanced Natural Language Processing (NLP) in Python and offers to load statistical models to predict linguistic annotations – for example, whether a word is a verb or a noun. Spacy currently offers statistical models for a variety of languages. I have used it for loading pre-trained statistical models for English and used that model to collect noun chunks from reviews.

gensim: It is a Python library for topic modelling, document indexing and similarity retrieval with large corpora. With the help of it, I have imported model and loaded the input-hidden weight matrix from the original C word2vec-tool format. In this, I have used "word2vec-GoogleNews-vectors" which is a pre-trained Google News corpus (3 billion running words) word vector model (3 million 300-dimension English word vectors). After the model is prepared then I used it to find cosine similarity between aspects and word collections.

requests: It is a Python HTTP library and its core purpose is to make HTTP requests simpler and more human-friendly and I have used it to get response by initiating a GET request from url of patina group.

pandas: It is a free software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series and I have used it for the same.

numpy: It is a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays and I have used it for the same.

seaborn: It is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics and I have used it to plot bar graph.

collections: This module implements specialized container datatypes providing alternatives to Python’s general purpose built-in containers, dict, list, set, and tuple. I have used it to get counts for repetition of words.

Itertools: This module implements a number of iterator building blocks inspired by constructs from APL, Haskell, and SML. Each has been recast in a form suitable for Python. I have used it while collecting counts for repetition of words.

bs4: It is a Python library for pulling data out of HTML and XML files. It works with your favorite parser to provide idiomatic ways of navigating, searching, and modifying the parse tree and I have used it while fetching details of all restaurant from content of response.

textblob: It is a Python library for processing textual data and provides a simple API for diving into common natural language processing (NLP) tasks such as part-of-speech tagging, noun phrase extraction, sentiment analysis, classification, translation, and more. I have used it for finding part-of-speech and sentiment analysis.

dash: It is a Python framework for building analytical web applications and does not require javascript and built on top of Plotly.js, React and Flask. It ties modern UI elements like dropdowns, sliders, and graphs directly to your analytical python code. I have used it for building dashboard for showing data insight.

plotly: It provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python, R, MATLAB, Perl, Julia, Arduino, and REST. I have used it to plot bar and pie chart with an association of dash.

