There is a bucket which is getting filled up by specific amount of tokens at specific interval
e.g. 10 tokens per second.

When someone makes a request a token from bucket is removed.
When all tokens are removed and bucket is empty that means server is busy and no more
requests will be handled till next fill adds 10 more.

When empty return 429 too many attempts.

Buckets can be for :
- ip
- user
- API key
- Overall Server

Used for:
- used in network traffic shaping
- used in API rate limiting
- when data can be sent and at what speed
