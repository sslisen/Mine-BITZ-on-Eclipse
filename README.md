# ePOW

# ⚡ Eclipse Bitz Setup Guide on Ubuntu

---

## 🚀 Setup Steps

1. Install Rust
```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh```

ℹ️ Follow the prompts. Once installed, run:
```source $HOME/.cargo/env```

2. Install Solana CLI
```curl --proto '=https' --tlsv1.2 -sSfL https://solana-install.solana.workers.dev | bash```

3. Create a Wallet (Keypair)
```solana-keygen new```
set Passphrase for better security or just skip (click enter)

This will create a new keypair at the default path:
```~/.config/solana/id.json```

👉 To generate a keypair at a custom path:
```solana-keygen new -o /path/to/keypair.json```

⚠️ Save your public key & mnemonic — it will be shown after creation.

4. Install Bitz CLI
```cargo install bitz```

5. Change RPC
```solana config set --url https://mainnetbeta-rpc.eclipse.xyz/```

6. Open Screen
```screen -s eclipse```

7. Start eMining
```bitz collect```

🔹 Other Commands
 	•	Claim your Bitz: ```bitz claim```
  •	Check your balance: ```bitz account```
  •	View all commands: ```bitz -h```

  Import to backpack:
  type ```solana config get```
  copy path of Keypair path
  type ```cat <Keypair path>```
  import copy array of number and import them on backpack in private key
