Homework 8: Text
================

Shakespearean sentiment
-----------------------

<img src="../figs/hamlet-sentiment.jpg" alt="https://static-secure.guim.co.uk/sys-images/Guardian/Pix/pictures/2013/3/28/1364485957230/Hamlet-002.jpg" height="250" width="410">

### Exercise 1

Which character, Lady Macbeth or Macbeth, uses more words with a negative sentiment? Answer this two ways: using the `bing` positive/negative lexicon and using the `afinn` numerical lexicon.

### Exercise 2

Create a plot that illustrates the overall positive/negative tone of the play Macbeth as it progresses. This should be a time series with line number on the x-axis and sentiment on the y-axis. I recommend using `geom_col()`. If you average the sentiment of the words within each line, it might be very erratic, so consider smoothing the grent by averaging within some larger text bin (say, every 5 or 10 lines). Create a second plot that does the same for the play that you studied in activity 8.

A Shakespeare Machine of your own
---------------------------------

### Exercise 3

Watch [this](http://vimeo.com/54858820) (background on the project is [here](http://www.artnews.com/2012/10/16/ben-rubin-shakespeare-machine/)).

Using the complete works of William Shakespeare (access via `gutenbergr` or <https://www.gutenberg.org/files/100/100-0.txt>), use regular expressions to find all of the hyphenated words used by the Shakespeare Machine. How many are there? Does your list contain all of the hypthenated words that appear at 00:46 of the clip? What are the top five most-used hyphenated words?

<img src="../figs/shakespeare-hyphenated.jpg" height="225" width="350">

### Exercise 4

Use regular expressions to extract all of the phrases (insults?) that are of the form shown below. What are the the top five most-used of these phrases?

<img src="../figs/shakespeare-you.jpg" height="520" width="300">

### Exercise 5

Using the list from exercise 4, create your own Shakespeare Machine. Run the following boring Alphabet Machine code below to see how to build a simple machine in R, then adapt it for your needs. Note: set `eval = FALSE` in your R chunk when submitting this homework.

``` r
word_list <- letters
it <- 8
for (i in 1:it) {
  print(sample(word_list, size = 8))
  Sys.sleep(5)
}
```
