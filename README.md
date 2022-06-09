# MINDS_Kanika_Jindal
MINDS project submission by Kanika Jindal.

To run the code:
Run the .ipynb file. I worked on Google colab, so the environment is Google colab environment.

The two attached png's contain the diagrams. 

Results:
1) Collected the data from the given source. 
2) Created data.json from the data where key is the "article title" and value is the "article paragraph".
3) I started by doing preprocessing on the title and the paragraphs separately. 
4) For preprocessing the pipe used is:
  convert to lower case -> remove urls -> remove backslashes -> remove html -> remove non-english cahracters -> remove whitespaces and join words such as kanika's become kanikas -> remove stopwords -> remove common nouns
5) I used off-the-shelf library to produce sentiment analysis report. 
6) Used NLTK to get polarity scores using Nltk's SentimentIntensityAnalyzer.

The results suggest that most of the articles collected are neutral. On analysing further, it can be seen that use of words such as "extends" increase the positive score.

RESULT ON PARAGRAPHS:
The score for "floods happening month torrential rains killed people kwazulu natal province".... article paragraph is: {'neg': 0.164, 'neu': 0.768, 'pos': 0.068, 'compound': -0.9816}, 

The score for "recent years southern africa suffered repeated devastating cyclones scientists believe".... article paragraph is: {'neg': 0.346, 'neu': 0.642, 'pos': 0.012, 'compound': -0.9933}, 

The score for "new ministers named reshuffle president nyusi mozambique president nyusi appointed".... article paragraph is: {'neg': 0.073, 'neu': 0.87, 'pos': 0.057, 'compound': -0.304}, 

The score for "lack infrastructure capacity could hurt continents plan supply gas europe".... article paragraph is: {'neg': 0.054, 'neu': 0.822, 'pos': 0.123, 'compound': 0.9913}, 

The score for "least people killed struck madagascar mozambique malawi authorities scrambling repair".... article paragraph is: {'neg': 0.297, 'neu': 0.638, 'pos': 0.065, 'compound': -0.9957}, 

The score for "regional body says progress made rebels cabo delgado province since".... article paragraph is: {'neg': 0.069, 'neu': 0.76, 'pos': 0.171, 'compound': 0.946}, 

The score for "start takes big news stories breaks down world complicated news".... article paragraph is: {'neg': 0.329, 'neu': 0.63, 'pos': 0.04, 'compound': -0.9873}, 

The score for "rwandan president says countrys force help secure rebuild cabo delgado".... article paragraph is: {'neg': 0.163, 'neu': 0.732, 'pos': 0.106, 'compound': -0.9887}, 

The score for "mocimboa da praia home one africas biggest natural gas projects".... article paragraph is: {'neg': 0.096, 'neu': 0.781, 'pos': 0.122, 'compound': 0.5859}, 

The score for "government kigali says deployment request mozambican authorities aimed restoring state".... article paragraph is: {'neg': 0.2, 'neu': 0.688, 'pos': 0.111, 'compound': -0.9915}, 
