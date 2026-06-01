# 🪨 OGG CLI Master Tool

## One Tool. Everything OGG Need.

No website.  
No app.  
No middleman.  
No trust needed.

**OGG CLI Master Tool** is a command-line tool for interacting directly with the OGG Network.

OGG type command.  
Contract execute.  
Copper move.

```bash
ogg <command>
```

🪨 No UI.
🪨 No server.
🪨 No third party.
🪨 Just OGG, terminal, and blockchain.

---

## 📦 Latest Download

Download the latest version here:

https://github.com/Oggcoin/CLI-Master-Tool/releases/latest

---

## 🗿 What Is OGG CLI?

OGG CLI is the main terminal interface for the OGG Network.

It lets OGG interact with staking and Tribe Pool smart contracts directly from the command line.

No browser required.
No website to trust.
No wallet popup needed.

Everything happens through terminal.
Everything goes directly to chain.
Everything can be checked on Blockscout.

One tool. Two worlds.

---

## 🧱 What Is Inside?

The release package includes:

```text
index.js                 Main CLI logic
package.json             Dependency list
OGG-CLI.bat              Windows launcher
OGG-CLI.sh               Linux launcher
OGG-CLI.command          macOS launcher
README.md                Guide
```

Do **not** upload or share:

```text
keystore.json
private key
password
```

🪨 Private key is private. Tribe never ask.

---

## ⚙️ Setup

### 1. Download latest release

Go to:

https://github.com/Oggcoin/CLI-Master-Tool/releases/latest

Download and extract the package.

---

### 2. Launch CLI

**Windows** — double-click or run:

```text
OGG-CLI.bat
```

**Linux** — run:

```bash
chmod +x OGG-CLI.sh
./OGG-CLI.sh
```

**macOS** — double-click or run:

```bash
chmod +x OGG-CLI.command
./OGG-CLI.command
```

Launcher installs dependencies automatically on first run.

---

### 3. First launch — wallet setup

On first launch, CLI detects no wallet and runs setup wizard automatically:

```text
No wallet found. Let's get you set up.

1. Generate a new Oggcoin wallet
2. Import an existing wallet (paste private key)

Choose (1 or 2):
```

**Option 1 — Generate new wallet:**  
CLI creates a fresh wallet and shows address + private key on screen.  
Write down private key before pressing Enter — after this screen it is encrypted and hidden forever.

**Option 2 — Import existing wallet:**  
Paste your private key (input is hidden).  
CLI connects to Oggchain and shows address + balance to confirm it is the right wallet.

After either option — CLI asks to set a password (min 4 chars, confirmed twice).  
Private key is encrypted with **AES-256-GCM + PBKDF2** and saved to `keystore.json`.

Every launch after that — just enter password. Session stays unlocked until `exit`.

---

### Do not share

```text
keystore.json
private key
password
```

🪨 Private key is private. Tribe never ask.

---

## 🪟 Windows Usage

Run:

```text
OGG-CLI.bat
```

Or run command directly:

```text
OGG-CLI.bat balance
OGG-CLI.bat stake 1000
```

If dependencies are missing, launcher installs them automatically.

---

## 🐧 Linux Usage

Make launcher executable:

```bash
chmod +x OGG-CLI.sh
```

Run:

```bash
./OGG-CLI.sh
```

Or run command directly:

```bash
./OGG-CLI.sh balance
./OGG-CLI.sh stake 1000
```

If dependencies are missing, launcher installs them automatically.

---

## 🍎 macOS Usage

Make launcher executable:

```bash
chmod +x OGG-CLI.command
```

Run:

```bash
./OGG-CLI.command
```

Or run command directly:

```bash
./OGG-CLI.command balance
./OGG-CLI.command stake 1000
```

If dependencies are missing, launcher installs them automatically.

---

## 👛 Wallet Commands

Check balance.
Send copper.
Receive copper.
See history.
Export key.

```bash
ogg wallet
ogg send <to> <amount>
ogg receive
ogg history
ogg exportkey
```

### Examples

```bash
ogg wallet
ogg send 0x1234...abcd 100
ogg receive
ogg history
ogg exportkey
```

**What each does:**

- `wallet` — shows your address + current OGG balance
- `send <to> <amount>` — send OGG to any address, shows confirmation summary before broadcasting
- `receive` — displays your address to share with sender
- `history` — scans last 500 blocks, shows last 20 transactions (sends, receives, stakes, unstakes, claims and more)
- `exportkey` — decrypts and shows your private key on screen (password required again)

🪨 Nothing sends without OGG confirm first.

---

## 🥩 Staking Commands

Lock copper.
Earn copper.
Collect copper.
Leave when ready.

```bash
ogg balance
ogg stake <amount>
ogg rewards
ogg claim
ogg cooldown
ogg unstake <amount>
ogg withdraw
```

### Examples

```bash
ogg balance
ogg stake 1000
ogg rewards
ogg claim
ogg unstake 500
ogg withdraw
```

---

## 🏛️ Tribe Pool Commands

Speak for tribe.
Vote on ideas.
Release copper for builders.

```bash
ogg pool
ogg proposals
ogg proposal <id>
ogg propose
ogg vote <id> yes
ogg vote <id> no
ogg finalize <id>
ogg cleanup
```

### Examples

```bash
ogg pool
ogg proposals
ogg proposal 1
ogg vote 1 yes
ogg finalize 1
```

---

## 👁️ OGG Always See First

CLI never sends transaction without showing summary first.

Example:

```text
Amount to stake        1000.0000 OGG
From wallet            0x123...abc

Confirm? (yes/no):
```

OGG read.
OGG decide.
OGG confirm.

Then and only then — copper move.

🪨 Nothing happen without OGG say yes.

---

## 💸 What Costs Gas?

Reading chain is free.

Free/read commands:

```bash
ogg wallet
ogg receive
ogg history
ogg balance
ogg rewards
ogg cooldown
ogg pool
ogg proposals
ogg proposal <id>
```

Writing to chain costs small OGG gas fee.

Transaction commands:

```bash
ogg send <to> <amount>
ogg stake <amount>
ogg unstake <amount>
ogg withdraw
ogg claim
ogg propose
ogg vote <id> yes|no
ogg finalize <id>
ogg cleanup
```

🪨 Always keep small amount of OGG in wallet for gas.

---

## 🔍 Check Transactions On Blockscout

After every transaction, CLI shows transaction hash:

```text
TX: 0xabc...def
```

Paste hash into Blockscout to see exactly what happened.

Nothing hidden.
Nothing secret.
On chain forever.

---

## 🔐 Security Notes

OGG CLI stores wallet locally.

Never share:

```text
keystore.json
private key
password
```

If OGG lose private key, OGG lose access.
If OGG share private key, someone can move copper.

🪨 Keep key safe.

---

## 🧰 Troubleshooting

### CLI does not open

Open terminal inside CLI folder and run:

```bash
node index.js
```

This shows the real error instead of closing window.

---

### Dependencies missing

Run:

```bash
npm install
```

Or just launch the launcher for your platform — it installs dependencies automatically.

---

### Wrong password

If password is wrong, CLI cannot unlock wallet.

Only delete encrypted `keystore.json` if OGG still has private key safely backed up.

Then launch CLI again — setup wizard will run automatically.

---

## 🗿 OGG Way

One tool.
Everything OGG need.

No website.
No app.
No middleman.
No trust needed.

Just OGG, terminal, and blockchain.

🪨
