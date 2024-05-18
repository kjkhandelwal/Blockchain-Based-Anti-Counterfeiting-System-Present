# Blockchain-Based-Anti-Counterfeiting-System-Present

This project is a Blockchain-based Anti-counterfeit System designed to enhance supply chain transparency and combat the proliferation of fake products. By leveraging the immutable and secure nature of blockchain technology, our system ensures that product information is recorded transparently and tamper-proof throughout the supply chain. We use smart contracts written in Solidity on the Ethereum blockchain to automate and verify product authentication processes. Additionally, the system integrates QR codes to link physical products with their digital records, allowing consumers and stakeholders to easily verify product authenticity. This innovative solution aims to reduce counterfeit incidents, protect brand integrity, and increase consumer trust in the marketplace.

SETUP PROCESS:-
1. Clone the project
2. Extract the `src.zip` and verify that all the files are in the src folder only and not in src/src.

3. Go to the project folder, open terminal there and run following command to install required node_modules:-
```
npm install
```
4. Compile contract source files. (Compilation and deployment can be done using truffle migrate):-
```
truffle compile
```
5. Open Ganache, (to setup local blockchain)
    - crerate new workspace
    - add truffle-config.js  in truffle project 
    - change port to 7545 in server settings (same as port in truffle-config.js)
6. In chrome, open metamask 
   - add new test network using  
        - NETWORK ID (i.e. 5777 ,from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:7545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - import account using private key of any account from local blockchain available in Ganache.
7. In terminal, run following commands:-
- Run migrations to deploy contracts.
```
truffle migrate
```

- To start a server and it will open a homepage (index.html) file in the default browser.
```
npm run dev 
``` 
8. Login to metamask ,and connect the added account to local blockchain manually (i.e.localhost:3000)
9. Interact with website
