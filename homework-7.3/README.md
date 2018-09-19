
**Question**

Which of the following statements are true about choosing and using a shard key? Check all that apply.

**Answer**

```
 - There must be an index on the collection that starts with the shard key.
 - MongoDB cannot enforce unique indexes on a sharded collection other than the shard key itself or indexes prefixed by the shard key.
 - Any single update that does not contain the shard key or _id field will result in an error.
```
