## This is a simple singularity test

# How to build

to rebuild from scratch run:

`./rebuild.sh`

## check running instance

`singularity instance list`

## How to check that redis is working

Connect to Redis ( insert password: `ThisIsNotAStrongPassword!` )

`redis-cli --askpass`

write a key
```
127.0.0.1:6379> set foo bar
OK

127.0.0.1:6379> keys *
1) "foo"

127.0.0.1:6379> exit
```
