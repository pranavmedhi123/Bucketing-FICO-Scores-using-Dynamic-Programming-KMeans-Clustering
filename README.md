# Bucketing-FICO-Scores-using-Dynamic-Programming-KMeans-Clustering

#### Summary

- We are given a loan dataset with 10k records, with details regarding customers' fico scores, among other details.
- Goal is to create a function that will dynamically assign fico scores to buckets in such a way that the buckets best summarize the data while also mapping the buckets(boundaries) to ratings where lower rating denotes better fico score.

#### Conclusion

- Dynamic programming approach to minimize MSE in buckets lead to a complexity of O(n^3.k)(n being number of fico_scores, k is the number of buckets).
- KMeans Clustering approach proved to be far more efficient and ran in O(n) complexity.
- One other method that could be adopted is a mix of Greedy+Dynamic Programming approach. But it leads to complexity of O(n^2* k) as we have to precompute the subarray calculations before hand in a memoization array which in itself costs O(n^2), while the greedy algorithm will then semi-accurately give out best boundaries in a single pass costing O(n)
  
