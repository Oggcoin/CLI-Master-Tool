````md
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
````

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
package-lock.json        Locked dependency versions
OGG-CLI.bat              Windows launcher
ogg                      Linux/macOS launcher
keystore.example.json    Example wallet file
README.md                Guide
```

Do **not** upload or share:

```text
keystore.json
private key
seed phrase
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

### 2. Create wallet file

Copy:

```text
keystore.example.json
```

Rename the copy to:

```text
keystore.json
```

Open `keystore.json` and paste private key:

```json
{
  "privateKey": "PASTE_YOUR_PRIVATE_KEY_HERE"
}
```

On first launch, OGG CLI encrypts the key and asks OGG to create password.

After that, password is required every time CLI opens.

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

## 🐧 Linux / macOS Usage

Make launcher executable:

```bash
chmod +x ogg
```

Run:

```bash
./ogg
```

Or run command directly:

```bash
./ogg balance
./ogg stake 1000
```

If dependencies are missing, launcher installs them automatically.

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
seed phrase
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

Or just launch:

```text
OGG-CLI.bat
```

or:

```bash
./ogg
```

Launcher installs dependencies if missing.

---

### Wrong password

If password is wrong, CLI cannot unlock wallet.

Only delete encrypted `keystore.json` if OGG still has private key safely backed up.

Then create new `keystore.json` from `keystore.example.json`.

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

```
```
