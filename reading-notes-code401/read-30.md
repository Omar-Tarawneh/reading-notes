# Read-30, Code 401, 5 May 2021

## Hash Tables

A hash table (often called a hash map) is a data structure that maps keys to values. Hash tables combine lookup, insert, and delete operations in an efficient way. The key is sent to a hash function that performs arithmetic operations on it. The result (called the hash value or hash) is an index of the key-value pair.

Hash tables have two parts:

- Object: An object with the table where the data is stored. The array holds all the key-value entries in the table. The size of the array should be set according to the amount of data expected.
- Hash function (or mapping function): This function determines the index of our key-value pair. It should be a one-way function and produce the a different hash for each key.

![hash-table](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Hash_table_3_1_1_0_1_0_0_SP.svg/1200px-Hash_table_3_1_1_0_1_0_0_SP.svg.png)

### Case of Use

Hash tables provide access to elements in constant time, so they are highly recommended for algorithms that prioritize search and data retrieval operations. Hashing is ideal for large amounts of data, as they take a constant amount of time to perform insertion, deletion, and search.

In terms of time complexity, the operation is 0(1). On average, a hash table lookup is more efficient than other table lookup data structures.

Examples:
Caches
Unique data representation
Lookup in an unsorted array
Lookup in sorted array using binary search

### Starter Code

```js
class HashEntry {
  constructor(key, data) {
    this.key = key;
    // data to be stored
    this.value = data;
    // reference to new entry
    this.next = null;
  }
}
```

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-30)
