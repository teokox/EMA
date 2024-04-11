# EMA
Encryption by Masking

<strong>EMA stands for “Encryption by Masking“.</strong>

For more information, visit https://www.creoart.com.

For more information on encryption and data masking, see the following links:

https://en.wikipedia.org/wiki/Cryptography</br>
https://en.wikipedia.org/wiki/Data_masking</br>
https://en.wikipedia.org/wiki/Caesar_cipher</br>
https://en.wikipedia.org/wiki/Substitution_cipher</br>
https://www.google.it/search?q=Cryptography</br>
https://www.google.com/search?q=data+masking</br>
https://en.wikipedia.org/wiki/Encryption</br>

<strong>Basically, EMA is a project designed to create a symmetric encryption method, consisting of two fundamental conceptual techniques named Ema_0 and Ema_1. The Ema_0 technique replaces the data value to be encrypted with the key value, Ema_1 instead shuffles them. These encryption and decryption techniques were developed mainly for theoretical, experimental, educational, and research purposes.</strong>

The project aims to develop a Java software called EMA.

The EMA method utilizes a master key comprising of two sub-keys. Ema_0 uses the first half and Ema_1 the second half.

The contents of the keys and of the data to be encrypted or decrypted belong to the set of 256 ASCII characters, with decimal value signed from -128 to 127 and unsigned from 0 to 255.

Read more about bytes and ASCII:

https://en.wikipedia.org/wiki/Advanced_Encryption_Standard</br>
https://en.wikipedia.org/wiki/Byte</br>
https://en.wikipedia.org/wiki/ASCII</br>

The terms ‘mask’ and ‘unmask’ now refer to encryption and decryption, respectively. The same applies to their related terms ‘masking/encryption’ and ‘unmasking/decryption’. The terms ‘cipher’ and ‘decipher’ have the same meaning.

Each technique utilises a unique sub-key to independently mask and unmask the data source. These techniques involve data substitution (Ema_0) and data shuffling (Ema_1), where the data source is replaced by key data and/or shuffled based on key values. It is important to note that Ema_0 and Ema_1 can be used in combination to create a highly secure encryption.

The following pages explain the basic concepts of EMA encryption:

ASCII code table</br>
The Masking/Encryption Concept</br>
-- The Replacement Technique</br>
-- The Shuffling Technique</br>
The Unmasking/Decryption Concept</br>
-- The Substitution Technique</br>
-- The Reordering Technique</br>

These techniques are based on simple data masking using key values, indexes, and data source values in the form of byte arrays. The data source elements and indexes are compared with the key elements and indexes. Simple operations such as XOR, sum, comparison, and array read/write are used to mask and unmask the data.

EMA pros:

- conceptual and use simplicity</br>
- very fast encryption/decryption</br>
- unbreakable encryption</br>
- very long keys do not affect computer performance</br>

EMA cons:

- of course, this encryption is only of the symmetric type
- Java program only (currently in development)
- EMA uses the Ema_0 and Ema_1 techniques simultaneously with two different keys of the same length.

These techniques are very simple and fast. At the level of the byte blocks, Ema_n basically replaces all the original data with the data of the first key and then mixes it with the data of the second key.

Unlike other symmetric encryption techniques, EMA can use very large keys without performance degradation.

EMA uses the following two masking/unmasking techniques:

<strong>Ema_0 replaces</strong> the input data according to the key values</br>
-- Masking (encryption) with Ema_0: direct substitution called replacement</br>
-- Unmasking (decryption) with Ema_0: reverse substitution called substitution</br>

<strong>Ema_1 shuffle</strong> the input data according to the key indexes and values</br>
-- Masking (encryption) with Ema_1: direct shuffling called shuffling</br>
-- Unmasking (decryption) with Ema_1: reverse shuffling called reordering</br>

The EMA encryption and decryption method utilises uncomplicated and recognizable techniques along with a minimal amount of code. In contrast to other algorithms, which depend on intricate calculations to factor large numbers and perform other complex algorithms.

We will see in detail what substitution and shuffling mean and how they are used in this method.

Decrypting or unmasking a masked file using these techniques essentially means guessing two keys, each of which can be up to several megabytes long.
