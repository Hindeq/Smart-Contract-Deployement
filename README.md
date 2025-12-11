# Smart Contract Deployment with Flutter

## Description
This project is a Flutter-based decentralized application (DApp) that interacts with an Ethereum smart contract deployed on Ganache. It allows users to read and update a name stored in the smart contract.

The project uses:
- Flutter for the frontend
- Web3dart for interacting with the Ethereum blockchain
- Truffle for compiling, testing, and migrating smart contracts
- Ganache as a local Ethereum blockchain

---

## Features
- Connect to Ethereum smart contract (HelloWorld.sol)
- Display the current name stored in the contract
- Update the name using a text input
- Works on Web and Windows

---

## Project Structure
smart_contract/
├─ lib/
│ ├─ contract_linking.dart # Handles the smart contract connection

│ ├─ helloUI.dart # User interface for interacting with the contract

│ └─ main.dart # Main entry point

├─ src/artifacts/HelloWorld.json # Contract ABI and deployed address

├─ pubspec.yaml # Flutter dependencies

└─ README.md


---

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Hindeq/Smart-Contract-Deployement.git
cd Smart-Contract-Deployement
```
2. Install Flutter dependecies
   flutter pub get
3. Make sure Ganache is running and the smart contract is migrated using Truffle:
     truffle migrate

## Notes

- Update the _privateKey in contract_linking.dart with your Ganache account private key.

- Update the RPC URLs in contract_linking.dart if needed:

- For Web: http://127.0.0.1:7545

- For Android/Emulator: http://10.0.2.2:7545

## Dependencies

provider: state management

web3dart: Ethereum blockchain interaction

http: HTTP client

web_socket_channel: WebSocket client

flutter: SDK

## License
Academic Project
