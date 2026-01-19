# Notes
- Presents algorithms for online learning in sponsored search auction settings.
- Algorithms don't know the item valuation.
- Agorithms achieve almost full information regret rates.
- Conclusions: WIN-EXP has less regret than EXP3
- Algorithms with regret rates against the best fixed bid in hindsight.
- Algorithms of equivalent performance to a fully observed environment (full information).
- Participants cannot pre-assess the value of the good.
- Participants learn by doing.
- The large number of auctions allows for a sort-of-training.
- The algorithms learns to bid optimally over time - minimizing its regret.
- The bidder must win the good in order to learn its value - pay higher price.
- Exploration and Exploitation interplay.
- Goal of the paper: algorithm which learns how to bid (optimally) in this partially observed environment with minimum regret.

**Contributions**:
1. Online learning setting for multiple auction scenarios.
2. WIN-EXP algorithm - based on EXP3


## Multi Armed Bandit problem - MAB
- You have multiple slot machines
- Each machine has a different, unknown pay-out probability
**Challenge**
- How to choose machines to play to maximize profit?
- **Exploration**: try different machines to gather information
- **Exploitation**: stay with the best performing machine, knowing machine, so far for guaranteed result.


## Online learning
- Data is presented sequentially from a continuous stream of data.


## Sponsored search auction
- The results or a search are a sponsored by 3rd parties.


# 5-page outline

## Page 1
- Problem introduction
- Learning to Bid Without Knowing your Value
- Learning-by-Doing Approach
- Classic MAB


## Page 2
- The Outcome-Based Feedback Framework


## Page 3
- WIN-EXP algorithm


## Page 4
- Algorithm extensions


## Page 5
- Experiments & Conclusion
