# Basic Commands in Redis

## Strings

```sql

SET key value # For setting message

GET key # For getting message

```

```sql

APPEND key value

```

### Lists

- `LPUSH key value [another value ...]`: Add elements to the left of the list.
- `RPUSH key value [another value ...]`: Add elements to the right of the list.
- `LRANGE key start stop`: Retrieve elements from a specific range in the list.
- `LLEN key`: Get the length of the list.
- `LREM key count value`: Remove specific elements from the list.

### Hashes

- `HSET key field value`: Set a field-value pair in the hash.
- `HMGET key field [another field ...]`: Get multiple fields from the hash.
- `HINCRBY key field increment`: Increment a numeric field's value by a specific amount.
- `HDEL key field [another field ...]`: Delete fields from the hash.
- `HKEYS key`: Get all field names in the hash.

### Sets

- `SADD key member [another member ...]`: Add members to the set.
- `SMEMBERS key`: Get all members in the set.
- `SREM key member [another member ...]`: Remove members from the set.
- `SINTER key key2 [...keys]`: Find members present in all given sets.
- `SDIFF key key2 [...keys]`: Find members present in the first set but not in others.

### Sorted Sets

- `ZADD key score member [another member score ...]`: Add members to the sorted set with their scores.
- `ZRANGE key min max [WITHSCORES]`: Get members within a score range, optionally including scores.
- `ZREVRANGE key min max [WITHSCORES]`: Get members in reverse order within a score range.
- `ZINCRBY key increment member`: Increment a member's score by a specific value.
- `ZREM key member [another member ...]`: Remove members from the sorted set.

### Additional Commands

- `KEYS pattern`: Find keys matching a specific pattern.
- `DEL key`: Delete a key.
- `EXISTS key`: Check if a key exists.
- `EXPIRE key seconds`: Set an expiration time for a key.
- `TTL key`: Get the remaining time until a key expires.
- `PING`: Check if the server is alive.



