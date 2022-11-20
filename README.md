# SecureFileStorageUsingHybridCryptogaphy
Clone this Git Repository using "Visual Studio Code"
RUN app.py 
Enjoy the Website

Methodology-

In this project we've taken several cryptographic algorithms like 
ChaCha20Poly1305, AESGCM, Fernet and AESCCM to securely 
encrypt the uploaded file. 
Here the methodology is to firstly load the file on the server and divide 
the file into n parts then any of those select above cryptographic 
algorithms & these algorithms are often changed with every part in an 
exceedingly round robin manner. 
To achieve the above goal, the following methodology needs to be 
followed: 
1. Load the file on the server. 
2. Dividing the uploaded file into N parts. 
3. Encrypting all the parts of the file using any one of the selected 
algorithms, these algorithms are often changed with every part in an 
exceedingly round robin manner. 
4. The keys for cryptography algorithms are then secured using a 
different algorithm and the key for this algorithm is provided to the user 
as public key.
After the above 4 steps you will have a N-files which are in encrypted 
form which are stored on the server and a key which is downloaded as 
public key for decrypting the file and downloading it. 
To restore the file, follow the following steps: 
1. Load the key on the server. 
2. Decrypt the keys of the algorithms. 
3. Decrypt all the N parts of the file using the same algorithms which 
were used to encrypt them. 
4. Combine all the N parts to form the original file and provide it to the 
user for downloading. 
