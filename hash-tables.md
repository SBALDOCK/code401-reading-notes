## Hash Tables

- Hash - Result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
- Buckets - What is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
- Collisions - What happens when more than one key gets hashed to the same location of the hashtable.

- Hashtables are a data structure that utilize key/value pairs. This means every **node** or **bucket** has both a key and a value.

- The goal is the ability to store the key into this data structure and quickly retrieve the value. This is done through a **hash**. The ability to encode the key that will eventually map to a specific location in the data structure that we can look directly to retrieve the value

- If you **hash** a key and determine the exact location of the value, a lookup can use O(1) time complexity, which is ideal when quick lookups are required.

### How does it work?

- A hash code turns a key into an integer. They must be deterministic, meaning their output is determined only by their input. Hash codes could never have randomness to them. The same key should always produce the same hash code.
- A hashtable is traditionally created from an array.

### Hastable Video Notes

- Data structure used to store information
- Key and Value
- Key - Could be something like a name
- Value - Could be my phone number
- A way to implement an associative array
- Array structure
- Write a hash function - Looks at a certain key, evaluates the key, and spits out an index of where in the array to store the information
- Hash(key) -> index
  - Hash(Steve) -> 3
  - Every time you enter the same key, it'll spit out the same value (3)
- What happens if a hash value is the same as an existing hash value?
  - This is a collision
  - Create a linked list off of each index so that the same hash value is chained to the existing hash value
- Enter the key inside the hash function, which will spit out an index of the location.
- There should not be very many links off of any single index
