
**Question**

Download Handouts: [sysprofile.json](sdsds)

In this problem you will analyze a profile log taken from a mongoDB instance. To start, please download sysprofile.json from Download Handout link and import it with the following command:

```
mongoimport --drop -d m101 -c profile sysprofile.json
```

Now query the profile data, looking for all queries to the _students_ collection in the database _school2_, sorted in order of decreasing latency. What is the latency of the longest running operation to the collection, in milliseconds?

**Answer**

```
15820
```
