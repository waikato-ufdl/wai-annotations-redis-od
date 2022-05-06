# wai-annotations-redis-predictions
wai.annotations plugin for making predictions via models communication through Redis backend.

The manual is available here:

https://ufdl.cms.waikato.ac.nz/wai-annotations-manual/

## Plugins
### REDIS-PREDICT-OD
Adds object detection overlays to images passing through.

#### Domain(s):
- **Image Object-Detection Domain**

#### Options:
```
usage: redis-predict-od [--channel-in CHANNEL_IN] [--channel-out CHANNEL_OUT] [--key-label KEY_LABEL] [--key-score KEY_SCORE] [-d REDIS_DB] [-h REDIS_HOST] [-p REDIS_PORT] [-t TIMEOUT] [-v]

optional arguments:
  --channel-in CHANNEL_IN
                        the Redis channel on which to receive predictions.
  --channel-out CHANNEL_OUT
                        the Redis channel to send the images out
  --key-label KEY_LABEL
                        the meta-data key in the annotations to use for storing the label.
  --key-score KEY_SCORE
                        the meta-data key in the annotations to use for storing the prediction score.
  -d REDIS_DB, --redis-db REDIS_DB
                        the database to use
  -h REDIS_HOST, --redis-host REDIS_HOST
                        the Redis server to connect to
  -p REDIS_PORT, --redis-port REDIS_PORT
                        the port the Redis server is running on
  -t TIMEOUT, --timeout TIMEOUT
                        the timeout in seconds to wait for a prediction to arrive
  -v, --verbose         whether to output debugging information.
```
