# Cuckoo--Hashing
Cuckoo Hashing is an open addressing scheme for hash tables that guarantees O(1) worst-case lookup time. It uses two hash functions and two hash tables (or one table with two positions per item) to resolve collisions.

Each key can reside in one of two possible positions:

Position 1: hash1(key)

Position 2: hash2(key)

If a collision occurs, the existing key is displaced ("kicked out") and reinserted into its alternate position, potentially causing a chain of displacements until every key finds a spot or a rehash is triggered.

 Advantages
Worst-case O(1) lookup.

Simplicity of design compared to other advanced hash schemes.

 Usage
Ideal for situations where:

Predictable and fast lookup times are required.

The hash table operates in environments with bounded-sized sets.
