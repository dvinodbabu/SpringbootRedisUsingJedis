# **Redis Cache**

### **What**?

* Remote Dictionary Server is a OpenSource - BSD licensed software
* In memory datastructure store
* Supports datastructures like strings,hashes,lists,sets, sorted sets etc.. - Data Structure server
* Has in built replication
* High Availability with redis-sentinel and automated partioning using redis-cluster
* supports lua scripting
* Written in ANSI C
* supports pipelining

<img src="https://www.cloudmanagementinsider.com/wp-content/uploads/2019/08/Did-you-know_-Redis-Fact-1.png" width="400">


---
### **Why**?
* Can be used as database,cache, and a message broker
* Exceptionally fast − About 110000 SETs per second, about 81000 GETs per second.
* Supports rich data types
* Operations are atomic − All Redis operations are atomic, which ensures that if two clients concurrently access, Redis server will receive the updated value.
* Multi-utility tool

---

### **How**?
* Key value store
* key-value store is the ability to store some data, called a value, inside a key.
* The value can be retrieved later only if we know the specific key it was stored in.
* There is no direct way to search for a key by value
* it is like a very large hash/dictionary, but it is persistent, i.e. when your application ends, the data doesn't go away. 

---
### **Configuration**
```
CONFIG GET * 
CONFIG SET loglevel "notice" 
```

### **Example** 

* String
    
```
SET key value
GET key
```
* Hashes

```
HMSET key field1 value1 field2 value2 ....
HMGETALL key
```

* Lists

```
LPUSH key value1 value2 value3 ....
RPUSH key value1 value2 value3 ....
LRANGE key start stop
```
* Sets

```
SADD key member1 member2 member3
SMEMBERS key
```

### **Links**
[API](https://redis.io/commands#hash)

[Tutorial](https://www.tutorialspoint.com/redis/redis_hashes.htm)

[Jedis](https://redislabs.com/lp/redis-java/)

[Jedis - Example](https://www.baeldung.com/jedis-java-redis-client-library)

