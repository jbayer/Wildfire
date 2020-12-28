# Wildfire
![Wildfire Screenshot](screenshot.png)

### "Once it takes fire, the substance will burn fiercely until it is no more."
**- George RR Martin, A Feast for Crows***

Wildfire is a secure deletion tool in C#. Using [SP800-88](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-88r1.pdf) conformant methods, Wildfire destroys accessible files locally or over a network to resist an adversary's attempts to recover data.

Wildfire implements secure deletion using the [AES-256 GCM](https://en.wikipedia.org/wiki/Galois/Counter_Mode) algorithm. It encrypts data at the byte level using cryptographically random keys, then deletes the file. This procedure ensures data is urecoverable even if the file is stored on storage media or a filesystem that does not immediately overwrite data marked for deletion (a common characteristic of most file and storage systems). 

Wildfire and its source code are licensed under the [MIT License](https://en.wikipedia.org/wiki/MIT_License). 
