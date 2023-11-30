# Huffman-Encoding

This code is based on the concept of Huffman Encoding and Decoding.
It can compress and decompress a text file.

Huffman encoding and decoding is a widely-used method in data compression.

Huffman Encoding:

Frequency Analysis: Count the frequency of each character in the data.
Build Huffman Tree: Create a binary tree where each character is a leaf node. Combine the least frequent characters in a tree structure, with the least frequent characters farthest from the root.
Assign Codes: Each edge in the tree represents a '0' or '1'. Assign a unique binary code to each character, based on the path from the root to the character.
Encode Data: Replace each character in the original data with its binary code from the tree.

Huffman Decoding:

Use Huffman Tree: Utilize the same tree created during encoding.
Decode Data: Read the encoded binary data bit by bit, traverse the tree from the root to the leaves. Each leaf node corresponds to a character in the original data.

To compress a file put command as ./hello compress aa.txt aazip.huf
To decompress a file put command as ./hello compress aazip.huf aa.txt
