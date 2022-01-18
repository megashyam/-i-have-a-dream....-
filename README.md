# -i-have-a-dream....-
Text genration using LSTM's of some of the most famous speeches of all time

## _what are LSTM's and how are they better than RNN's?_

Sequence prediction problems have been around for a long time. They are considered as one of the hardest problems to solve in the data science industry. These include a wide range of problems; from predicting sales to finding patterns in stock markets’ data, from understanding movie plots to recognizing your way of speech, from language translations to predicting your next word on your iPhone’s keyboard.

LSTMs have an edge over conventional feed-forward neural networks and RNN in many ways. This is because of their property of selectively remembering patterns for long durations of time.  The purpose of this article is to explain LSTM and enable you to use it in real life problems.  Let’s have a look!


Take an example of sequential data, which can be the stock market’s data for a particular stock.
In the conventional feed-forward neural networks, all test cases are considered to be independent. That is when fitting the model for a particular day, there is no consideration for the stock prices on the previous days.

![view](https://cdn.analyticsvidhya.com/wp-content/uploads/2017/12/05231650/rnn-neuron-196x300.png)

### _Limitations of RNN_

Recurrent Neural Networks work just fine when we are dealing with short-term dependencies. That is when applied to problems like:

![view](https://cdn.analyticsvidhya.com/wp-content/uploads/2017/12/10015332/b2_9.png)

RNNs turn out to be quite effective. This is because this problem has nothing to do with the context of the statement. The RNN need not remember what was said before this, or what was its meaning, all they need to know is that in most cases the sky is blue. Thus the prediction would be:

![view](https://cdn.analyticsvidhya.com/wp-content/uploads/2017/12/10015342/b2_10.png)


However, vanilla RNNs fail to understand the context behind an input. Something that was said long before, cannot be recalled when making predictions in the present. Let’s understand this as an example:

![view](https://cdn.analyticsvidhya.com/wp-content/uploads/2017/12/10015352/b2_11.png)

Here, we can understand that since the author has worked in Spain for 20 years, it is very likely that he may possess a good command over Spanish. But, to make a proper prediction, the RNN needs to remember this context. The relevant information may be separated from the point where it is needed, by a huge load of irrelevant data. This is where a Recurrent Neural Network fails!

The reason behind this is the problem of Vanishing Gradient



