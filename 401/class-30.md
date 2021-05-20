
# Hash Tables 

![](https://he-s3.s3.amazonaws.com/media/uploads/2cabd32.jpg)


## Hashing 

 the process of converting a given key into another value. A hash function is used to generate the new value according to a mathematical algorithm.
  A good hash function uses a one-way hashing algorithm, or in other words, the hash cannot be converted back into the original key.


  ## Hash Tables 
collection that is used to store in the form of  key-value items, where you can store the key into a data structure, and quickly retrieve the value 

This means every Node or Bucket has both a key, and a value.

`bucket` is what is contained in each index of the array of the hashtable.

Each “bucket” holds one key/value pair combination.
if there is there is no entry in a specific bucket, the buckets (each index of the array) all start null

The hash table starts each bucket empty and overwrites their value once a key generates a hashCode that corresponds with an index.

Note:  it’s important to store the entire key/value pair in the bucket, not just the value



`Hash`  encoding  the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.




it takes an incoming string and converts it to a value that could be used for either
- security 
- old unique values
- Dictionary
- Library


hash tables have the big o of O(1) 
Instead of adding elements to an array from beginning to end,which what you normally do when you want to search for a specific item and that and that takes
 O(n) because you go though each item in the array

but the  hash map uses a “hash function” to place each item at a precise index location, based off it’s key.

## Structure

- Hashing 
in hashing the same key should always produce the same hash code. 
hash codes are described as deterministic which indicates that their output is determined only by their input.

to store values: 
- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- store the key with the value by appending both to the end of a linked list

to read values:
- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- use the array index to access the short LinkedList - - - -
- representing a bucket
- search through the bucket looking for a node with a key/value pair that matches the key you were given


## Collisions 
- it occurs when more than one key hashes to the same index
whichever was added first is at the front of the list. 
- the worst possible hash is one that hashes every single key to the same exact index of an array

Collisions are solved by changing the initial state of the buckets. Instead of starting them all as null we can initialize a LinkedList in each one
then their key/value pairs can be stored as a node in a linked list.


## Internal Methods 

- Add() 
takes in a key, gets the Hash,see if the key exists and return the value. 

- Find() 
takes in a key, gets the Hash, goes to the index location specified and  return the value. 
- Contains() 
accept a key, and return a bool on if that key exists inside the hashtable. 

- GetHash() 
accept a key as a string, conduct the hash, and then return the index 