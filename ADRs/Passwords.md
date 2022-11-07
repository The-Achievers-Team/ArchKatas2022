Decision: We will use salted hashes for storing ours user passwords, instead of simple hashes. (A salt is added to the hashing process to force their uniqueness, increase their complexity without increasing user requirements, and to mitigate password attacks like hash tables)

Pros:

1. Security: The unique hash produced by adding the salt can protect us against different attack vectors, such as hash table attacks, while slowing down dictionary and brute-force offline attacks.


Cons:

1. Extra processing time: Salted hashing typically requires more computational resources and time to do the matching check, as compared to 


Justification: The security benefit provided by salted hashes is much too important.