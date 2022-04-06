## Redis CLI remove multiple keys using pattern
Replace [pattern] with key pattern you want to use<br>
eg: redis-cli eval "return redis.call('del', unpack(redis.call('keys', ARGV[1])))" 0 "fqc*"

```sh
redis-cli eval "return redis.call('del', unpack(redis.call('keys', ARGV[1])))" 0 [pattern]
```
