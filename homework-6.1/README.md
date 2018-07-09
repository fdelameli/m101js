
**Question**

Download Handouts: [companies_dataset.zip](https://github.com/fabiodelabruna/m101js/raw/master/homework-6.1/companies_dataset.zip)

Starting with the example we looked at for calculating the total number of relationships individuals have participated in (in the CrunchBase data set):

```
db.companies.aggregate( [
    { $match: { "relationships.person": { $ne: null } } },
    { $project: { relationships: 1, _id: 0 } },
    { $unwind: "$relationships" },
    { $group: {
        _id: "$relationships.person",
        count: { $sum: 1 }
    } },
    { $sort: { count: -1 } }
] )
```

Write an aggregation query that will determine the number of unique companies with which an individual has been associated. To test that you wrote your aggregation query correctly, from the choices below, select the number of unique companies that _Eric Di Benedetto (eric-di-benedetto)_ has been associated with. I've attached the CrunchBase data set for use in this problem.

Hint: Review the available [accumulators](https://docs.mongodb.org/manual/meta/aggregation-quick-reference/#accumulators) before beginning this exercise.

As a check on your work, the number of unique companies for _roger-ehrenberg_ is 16, for _josh-stein_ is 14, and the number for _tim-hanlon_ actually is 28.

**Answer**

```
15
```
