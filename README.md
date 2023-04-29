# Assignment10

## Threshold
First, I established that the threshold for toxicity was a 0.5 or above. I did this by selecting some samples from the class dataset and making requests with the API. I selected half YES toxic comments, and half NO toxic comments, and about 10-15 of each. The YES toxic comments came back with a threshold between 0.6-0.9+, and the NO toxic comments did not even pass a threshold point score of 0.1. Some of the scores were even so low, like 0.01 or 0.03. So I noticed a very big difference there. That is why I thought the toxicity score threshold should be 0.5 or above, since I also wanted to account for mistakes or bias in the code. 

## Hypothesis
My hypothesis was that one cuss word would cause the entire toxicity rating to jump up immiediately. I created around 25 comments, each being helpful and educational comments. Some of those example comments were like:

Business education can prepare students for entrepreneurship and finance
Psychology education can improve interpersonal relationships and self-awareness
Health education promotes wellness and disease prevention

I then made "dirty" versions of those same comments.

Business education can prepare students fuc for entrepreneurship and finance
Psychology education can improve interpersonal fuccc relationships and self-awareness
Health education promotes shi11tt wellness and disease prevention

Some of these comments had the full cuss word in it, and some of them had more "hidden" ones, with the numbers and extra letters. I thought that the dirty versions would immediately hit a threshold of 0.5 or above, which would mark it as toxic under my point values.

## Results and Conclusions
Because I had only sent about 25 clean comments, and 25 dirty comments, I had a fairly low sample size. On the plus side I could easily see the output and threshold point data. On the negative side, there just wasn't a lot of data to use and a solid conclusion can't really be made. However, I ended up being correct in guessing that just one cuss word can drastically change the threshold level to above a 0.5, even in a positive and educational comment.

(Review from journal conclusion)
Some examples of more vague comments and hidden cuss words would be the one where there are numbers in the dirty words. For example, using sh1t instead of the actual word, or f4ck instead of the actual word. One of the comments uses SH1T and passes the threshold test and is considered nontoxic. For example

"Philosophy challenges us to think SH1T critically and examine our beliefs", and it had a score of 0.37073207. 

I previously placed the level at 0.5, so it would not have gone over this number to be marked as toxic. Meanwhile, the comment 

"Literature teaches empathy asss and critical thinking" ended up with a score of 0.52272606. 

This comment would have been marked as toxic, even though some users might just talk in a way with extra letters like "thissss" or "thattt". 

## Reflection
While something like machine learning for checking and blocking toxic comments would be helpful, it is also important to note the bias and possible mistakes that might occur in the code. It would also be important to realize that some malicious users will keep finding ways to get their toxic comments past comment-checkers and moderated comments. We could see how SH1T passed the threshold but for example a user typing "I am assss tired as a lazyyy cat" would have their comment marked as toxic instead. When writing code for something like this, we always have to watch out for these occurances. 


