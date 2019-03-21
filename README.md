# contracts
1. Card Repository - Defines the ownership of cards to players

## Requirements
1. Environment for building EOS contracts
2. EOS.CDT 1.4.1


## Compile contracts
```bash
mkdir -p build
cd build
cmake ../

make
```


## Hash
1. Get hash of running contract:
   ```bash
   cleos --url https://node1.asteroidrush.io:8210 get code cardrepo
   ```
2. Get hash of compiled contract:
   ```bash
   sha256sum build/cardrepo.wasm
   ```


## Documentation
1. Install doxygen
2. Run from root folder:
```
doxygen
```
3. Open [doc/html/index.html](./doc/html/index.html)