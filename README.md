# 💸 Web3 Payment Application on Internet Computer

A **secure**, **decentralized**, and **trustless** payment application powered by the **Internet Computer Protocol (ICP)**. Built using **Motoko** (for canister backend logic) and **JavaScript** (frontend), this dApp allows seamless blockchain-based transactions without centralized intermediaries.

---

## 🚀 Features

- 🔐 **Secure Transactions** — Peer-to-peer payments via cryptographically verified canister calls.
- 🌐 **Decentralized Backend** — Logic hosted on Internet Computer canisters written in Motoko.
- ⚡ **Fast and Low-Cost** — Powered by ICP’s scalability and efficiency.
- 📲 **JavaScript Frontend** — Modern and interactive UI/UX using vanilla JS or a frontend framework.
- 🔄 **State Persistence** — User balances and transactions securely stored on-chain.
- 🧠 **Smart Contracts** — Custom Motoko smart contracts to handle logic and validation.

---

## 🛠️ Tech Stack

| Layer | Tech |
|-------|------|
| **Blockchain** | Internet Computer Protocol (ICP) |
| **Backend** | Motoko |
| **Frontend** | JavaScript, HTML, CSS |
| **Agent Library** | `@dfinity/agent`, `@dfinity/auth-client` |
| **Dev Tools** | DFX CLI, Internet Identity |

---

## 🧑‍💻 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/)
- [DFX SDK](https://internetcomputer.org/docs/current/developer-docs/build/install-upgrade-remove)
- Internet Identity
 
# Setup and Installation
## Requirements 
● Windows 10 or higher (version 2004 or higher). Build 19041.xxx or
 higher.
● 64-bit machine (System type x64 based PC)

## Steps
### WSL
1. Find the WindowsPowerShellin your Start menu andrun it as the Administrator
```
 wsl --install
```
2.  Once that’s done, you’ll need torestartyour computer
3.  Upon restart you will be prompted to setup an ubuntuusernameand
 passwordand then you will have successfully installedWSL. (Keep a
 note of both of these pieces of information, you’ll need it later on).
4. To confirm that everything worked correctly, type the following
 command into PowerShell:
```
wsl --list --verbose
```
### VS Code
1. Download and install the latest version of VSCode
2. Install the Motokolanguage extension in VSCode (make sure it’s from theDfinity team )
3. Install the Remote WSLextension.

### Node
1. Search and open upUbuntufrom the Start menu.
2. Type the following command to install homebrew
   ```
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)
   ```
3. When prompted enter thepasswordfor the user
4. The installer will tell you how to add brew to the PATH
5. Also run the command under the line “Install Homebrew’s dependencies if you have sudo access”
   ```
   sudo apt-get install build-essential
   ```
6. Check that everything worked by typing the command
   ```
    brew -version
   ```
7. Install node using homebrew with the following command
   ```
    brew install node
   ```
8. Once it’s done check that it worked with
   ```
   node --version
   ```
### DFX
1.  Open up Ubuntu from the Start menu
2.  Copy the following command and paste it into your terminal and hit enter to install DFX
```
DFX_VERSION=0.9.3 sh -ci "$(curl -fsSL https://sdk.dfinity.org/install.sh)"
```
3. After DFX has installed it will tell you where it was installed. e.g.
4. e.g. in my case, it tells me that it has been installed in /home/angela/bin/dfx
5. Copy the installation path you got from the last step and replace
 <REPLACE WITH YOUR INSTALLATION PATH> from the command below
```
 export PATH=$PATH:<REPLACE WITH YOUR INSTALLATION PATH>
```
6.  Paste the formatted command from the previous step and hit enter
7.   Check that it has been added by running
```
echo "${PATH//:/$'\n'}"  
```
8. Check that dfx has been successfully installed with the following
 command
```
dfx --version
```
### Create the Default Hello DApp
1. Open upUbuntufrom the start menu and create a newfolder called
 ic-projects using the following command
```
mkdir ic-projects
```
2. Change directory into that folder using the command
   ```
   cd ic-projects
   ```
3.  Inside this ic-projects folder, we’re going to create our first Internet
 Computer DApp using the following command
```
dfx new hello
```
4. You can see this new project and folders by running the following command
   ```
    explorer.exe .
   ```
5. Open up VSCode and click on the green icon on the bottom left. It looks like
 this
6.  SelectNew WSL Window
7.  Inside the new window go to yourExtensionspaneland select theRemote
 WSLextension, click onInstall in WSL: Ubuntu
8. Now take a look through the files inside thesrcfolder.The main.mo is the
 Motoko file that we’ll be writing most of our code in.

# Run Completed Code
1. Make sure dfx is running
```
dfx start --clean
```
2. Deploy the project
```
dfx deploy
```
3. Start NPM
```
npm start
```



