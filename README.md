Hill-Cipher
How often we need to send someone a message and make sure no one else reads it. To encounter this problem the messages sent across to others are encoded more often than not. The algorithms used are as complex as Nazi’s Enigma and as simple as Caesar Cipher. Hill Cipher, invented by Lester S Hill in 1029, is a polygraphic substitution cipher based on Linear Algebra and particular requires the user to have an elementary understanding of the matrices. In this project, we have developed an extended algorithm for Hill Cipher (both for encryption and decryption) and implement it on MATLAB 

MATLAB
Hill_Cipher.m : this file contains 'main' function
Encrypt.m: this is to write the algorithm of encrypting text using hill cipher
Decrypt.m: this is to write the algorithm of decrypting text using hill cipher

Methodology
Encrypt()
Input
A 3x3 matrix which works as a key matrix, key[3][3]
A plaintext string message
Output

An encoded string
Constrains

-32,000 ≤ key ≤ 32,000
message ∈ {A, B, C …, Y, Z}
Working

Convert plaintext to ASCII number then subtract 33.
Multiply key matrix with the plain text and mod92 operator
Add 33 to the resultant matrix to get the ASCII code of respective elements in the matrix
Decrypt()
Output
Decoded message same as the initial input message
Working
Finding inverse of key
Multiply the inverse of key matrix with the ASCII matrix
Use mod92 operator on the matrix and add 33 to get elements in ASCII form.
