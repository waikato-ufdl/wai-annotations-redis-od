Inline stream processors for making predictions via a Redis backend:

* `redis-predict-ic`: broadcasts images via Redis and listens for predictions in JSON being broadcast (label/prediction pairs)
* `redis-predict-od`: broadcasts images via Redis and listens for predictions in OPEX format being broadcast
