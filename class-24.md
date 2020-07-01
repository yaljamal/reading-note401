# HashTable

it is a data structure that utilize key value pairs  This means every Node or Bucket has both a key, and a value it have : 

1. Hash :it is a function to give us the index of array
2. Buckets  :  A bucket is what is contained in each index of the array of the `hashTable`
3. Collisions : A collision is what happens when more than one key gets hashed to the same location of the `hashTable` .

## Internal Methods

1. `Add(value)` =>
1.  send the key to the GetHash method.
2. Once you determine the index of where it should be placed, go to that index
3. Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
4. If something does exist, add the new key/value pair to the data structure within that bucket.
2. `Find(key)` =>takes in a key nd goes to the index location specified. Once at the index location is found in the array
3. `Contains(key)` => 

it  will accept a key and return a bool on if that key exists inside the `hashTable` .

4. `GetHash(key)` => will accept a key as a string and then return the index of the array where the key/value should be placed.
