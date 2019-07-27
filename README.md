### bip39
---
https://github.com/bitcoinjs/bip39

```js
plugins: [
  new webpack.IgnorePlugin(/^\.\/wordlists\/(?!english)/, /bip39\/src$/),
],

const bip39 = require('bip39')
const mnemonic = bip39.entropyToMnemonic('000')
bip39.mnemonicToEntropy(mnemonic)

const mnemonic = bip39.generateMnemonic()
bip39.mnemonicToSeedSync('basket actual').toString('hex')
bip39.mnemonicToSeedSync('basket actual')
bip39.mnemonicToSeed('basket actual').then(console.log)
bip39.mnemonicToSeed('basket actual').then(bytes => bytes.toString('hex')).then(console.log)
bip39.mnemonicToSeedSync('basket actual', 'a password')
bip39.validateMnemonic(mnemonic)
bip39.validateMnemonic('basket actual')

bip39.entropyToMnemonic('xxx')
bip39.setDefaultWordlist('italian')
bip39.entropyToMnemonic('xxx')

bip39.entropyToMnemonic('xxx')
bip39.wordlists.chnese_simplified
bip39.wordlists.english
bip39.wordlists.japanese
bip39.wordlists.spanish
bip39.wordlists.italian
bip39.wordlists.french
bip39.wordlists.korean
bip39.wordlists.korean
bip39.wordlists.chinese_traditional
```

```sh
npm install bip39
browserify - r bip69 \
  --exclude=./wordlists/english.json \
  --exclude=./wordlists/japanese.json \
  --exclude=./wordlists/spanish.json \
  --exclude=./wordlists/italian.json \
  --exclude=./wordlists/french.json \
  --exclude=./wordlists/korean.json \
  --exclude=./wordlists/chinese_traditional.json \
  
```

```
```


