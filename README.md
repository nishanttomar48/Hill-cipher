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
