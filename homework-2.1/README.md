**Question**

Which of the choices below is the title of a movie from the year 2013 that is rated PG-13 and won no awards? Please query the **video.movieDetails** collection to find the answer.

NOTE: There is a dump of the video database included in the handouts for the "Creating Documents" lesson. Use that data set to answer this question.

**Answer**

```
> db.movieDetails.find({"year": 2013, "rated": "PG-13", "awards.wins": 0}).pretty();
{
	"_id" : ObjectId("5692a3e124de1e0ce2dfda22"),
	"title" : "A Decade of Decadence, Pt. 2: Legacy of Dreams",
	"year" : 2013,
	"rated" : "PG-13",
	"released" : ISODate("2013-09-13T04:00:00Z"),
	"runtime" : 65,
	"countries" : [
		"USA"
	],
	"genres" : [
		"Documentary"
	],
	"director" : "Drew Glick",
	"writers" : [
		"Drew Glick"
	],
	"actors" : [
		"Gordon Auld",
		"Howie Boulware Jr.",
		"Tod Boulware",
		"Chen Drachman"
	],
	"plot" : "A behind the scenes look at the making of A Tiger in the Dark: The Decadence Saga.",
	"poster" : null,
	"imdb" : {
		"id" : "tt2199902",
		"rating" : 8,
		"votes" : 50
	},
	"awards" : {
		"wins" : 0,
		"nominations" : 0,
		"text" : ""
	},
	"type" : "movie"
}

```
