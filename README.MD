# AES 128/192/256 bit (CBC/GCM)

Simple Compact AES Encrypt/Decrypt from built-in crypto module

aesEncrypt(keyLength, method, data, key)
aesDecrypt(keyLength, method, data, key)

## Example

```
var cipherText = aesEncrypt('256','cbc','Hello World', 'my secret key');
console.log(cipherText);
// output:
// {
//  iv: '9tWJEc6h9onW7pz0KkiO+g==',
//  encryptedData: 'N9GG5fnKsXA1USC8pHbQGg=='
// }

var decipherText = aesDecrypt('256', 'cbc', cipherText, 'my secret key');
console.log(decipherText);
// output:
// Hello World
```
