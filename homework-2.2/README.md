**Question**

Using the video.movieDetails collection, which of the queries below would produce output documents that resemble the following. Check all that apply.

NOTE: We are not asking you to consider specifically which documents would be output from the queries below, but rather what fields the output documents would contain.
```
{ "title" : "P.S. I Love You" }
{ "title" : "Love Actually" }
{ "title" : "Shakespeare in Love" }
```

**Answer**

```
> db.movieDetails.find({}, {title: 1, _id: 0});
> db.movieDetails.find({year: 1964}, {title: 1, _id: 0});
```
