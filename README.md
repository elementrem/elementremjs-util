##elementremjs-util
A collection of utility functions for elementrem. It can be used in node.js or can be in the browser with browserify.

```
$ npm install

...
.....
  define
    ✓ should trim zeros
    ✓ shouldn't allow wrong size for exact size requirements
    ✓ it should accept rlp encoded intial data
    ✓ it should not accept invalid values in the constuctor
    ✓ alias should work 

  zeros function
    ✓ should produce lots of 0s

  sha3
    ✓ should produce a sha3

  sha3 without hexprefix
    ✓ should produce a sha3

  sha3-512
    ✓ should produce a sha3

  sha256
    ✓ should produce a sha256

  ripemd160
    ✓ should produce a ripemd160
    ✓ should produce a padded ripemd160

  rlphash
    ✓ should produce a sha3 of the rlp data

  unpad
    ✓ should unpad a string

  unpad a hex string
    ✓ should unpad a string

  pad
    ✓ should left pad a Buffer
    ✓ should left truncate a Buffer
    ✓ should left pad a Buffer - alias

  rpad
    ✓ should right pad a Buffer
    ✓ should right truncate a Buffer
    ✓ should right pad a Buffer - alias

  bufferToHex
    ✓ should convert a buffer to hex

  intToHex
    ✓ should convert a int to hex

  intToBuffer
    ✓ should convert a int to a buffer

  bufferToInt
    ✓ should convert a int to hex
    ✓ should convert empty input to 0

  fromSigned
    ✓ should convert an unsigned (negative) buffer to a singed number
    ✓ should convert an unsigned (positive) buffer to a singed number

  toUnsigned
    ✓ should convert a signed (negative) number to unsigned
    ✓ should convert a signed (positive) number to unsigned

  isValidPrivate
    ✓ should fail on short input
    ✓ should fail on too big input
    ✓ should fail on invalid curve (zero)
    ✓ should fail on invalid curve (== N)
    ✓ should fail on invalid curve (>= N)
    ✓ should work otherwise (< N)

  isValidPublic
    ✓ should fail on too short input
    ✓ should fail on too big input
    ✓ should fail on SEC1 key
    ✓ shouldn't fail on SEC1 key with sanitize enabled
    ✓ should fail with an invalid SEC1 public key
    ✓ should work with compressed keys with sanitize enabled
    ✓ should work with sanitize enabled
    ✓ should work otherwise

  importPublic
    ✓ should work with an Elementrem public key
    ✓ should work with uncompressed SEC1 keys
    ✓ should work with compressed SEC1 keys

  publicToAddress
    ✓ should produce an address given a public key
    ✓ should produce an address given a SEC1 public key
    ✓ shouldn't produce an address given an invalid SEC1 public key
    ✓ shouldn't produce an address given an invalid public key

  publicToAddress 0x
    ✓ should produce an address given a public key

  privateToPublic
    ✓ should produce a public key given a private key
    ✓ shouldn't produce a public key given an invalid private key

  privateToAddress
    ✓ should produce an address given a private key

  generateAddress
    ✓ should produce an address given a public key

  generateAddress with hex prefix
    ✓ should produce an address given a public key

  generateAddress with nonce 0 (special case)
    ✓ should produce an address given a public key

  hex prefix
    ✓ should add
    ✓ should return on non-string input

  isPrecompiled
    ✓ should return true
    ✓ should return false

  toBuffer
    ✓ should work
    ✓ should fail

  baToJSON
    ✓ should turn a array of buffers into a pure json object
    ✓ should turn a buffers into string

  ecsign
    ✓ should produce a signature

  ecrecover
    ✓ should recover a public key
    ✓ should fail on an invalid signature (v = 21)
    ✓ should fail on an invalid signature (v = 29)
    ✓ should fail on an invalid signature (swapped points)

  .toChecksumAddress()
    ✓ should work

  .isValidChecksumAddress()
    ✓ should return true
    ✓ should validate

  .isValidAddress()
    ✓ should return true
    ✓ should return false

  message sig
    ✓ should return hex strings that the RPC can use


  77 passing (59ms)
...
....
Firefox 48.0.0 (Ubuntu 0.0.0): Executed 77 of 77 SUCCESS (1.822 secs / 1.323 secs)
elementremjs-util@4.5.0 /home/chain/elementrem/test/elementremjs-util
```
