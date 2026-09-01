1: Rest	ful URIs uses actions and verbs instead of identifying resources instead an alternative would be to use PATCH /v1/orders/{id} with a payload
2: not read only since it changes server state, safe to repeat since put is idempotent meaning repeating produces the same thing
3: 422 or 400 for valid request that violates business rule, 500 means server/infrastructure error and 200 means that the purchase succeeded when it didn’t
4: /reservations while there is a safeguard for reserving twice cancelling twice isn’t there yet so that is most likely the current most dangerous one when a network is cut
5: Difficulty in most parts mainly because I was rushing though 
