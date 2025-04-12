# ePOW

** Eclipse Bitz Setup Guide on Ubuntu 💚**


## 🚀 Setup Steps

1. Install Rust
```bash 
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
2. Follow the prompts. Once installed, run:
```bash
source $HOME/.cargo/env
```
3. Install Solana CLI
```bash 
curl --proto '=https' --tlsv1.2 -sSfL https://solana-install.solana.workers.dev | bash
```
4. Create a Wallet (Keypair)
```bash
solana-keygen new
```
Set Passphrase for better security or just skip (click enter)
<br><br>
This will create a new keypair at the default path:
```bash
~/.config/solana/id.json
```
<br><br>
To generate a keypair at a custom path:
```bash
solana-keygen new -o /path/to/keypair.json
```
⚠️ Save your public key & mnemonic — it will be shown after creation.
<br><br>
5. Install Bitz CLI
```bash
cargo install bitz
```
6. Change RPC
```bash
solana config set --url https://mainnetbeta-rpc.eclipse.xyz/
```
7. Open Screen
```bash
screen -s eclipse
```
8. Start eMining
```bitz collect```
You need 0.005 $ETH on Eclipse to start mining, send it to your public key
<br><br>
🔹 Other Commands

  •	Claim your Bitz:
```bash
bitz claim
```
  
  •	Check your balance:
```bash
bitz account
```
  
  •	View all commands:
```bash
bitz -h
```
<br><br>
Import to backpack:
```bash
solana config get
```
<br><br>  
copy path of Keypair path
<br><br>  
  type
```bash
cat <Keypair path>
```
<br><br>
Import copy array of number and import them on backpack in private key
