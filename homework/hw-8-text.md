Homework 8: Text
================

### Shakespearean sentiment

<img src="../figs/hamlet-sentiment.jpg" alt="https://static-secure.guim.co.uk/sys-images/Guardian/Pix/pictures/2013/3/28/1364485957230/Hamlet-002.jpg" height="250" width="420">

1.  Which character, Lady Macbeth or Macbeth, uses more words with a negative sentiment? Answer this two ways: using the `bing` positive/negative lexicon and using the `afinn` numerical lexicon.
2.  Create a plot that illustrates the overall positive/negative tone of the play Macbeth as it progresses. This should be a time series with line number on the x-axis and sentiment on the y-axis. I recommend using `geom_col()`. If you average the sentiment of the words within each line, it might be very erratic, so consider smoothing the grent by averaging within some larger text bin (say, every 5 or 10 lines). Create a second plot that does the same for the play that you studied in activity 8.
3.  Watch [this](http://vimeo.com/54858820). Using the complete works of William Shakespeare (access via `gutenbergr` or <https://www.gutenberg.org/files/100/100-0.txt>), use regular expressions to find all of the hyphenated words used by the Shakespear Machine. How many are there? Does your list contain all of the hypthenated words that appear at 00:46 of the clip? What are the top three most-used hyphenated words?
