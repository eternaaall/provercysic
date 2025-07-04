# 💻 Cysic Prover Auto-Installer

This repository provides a one-command installation and management script for running Cysic Prover nodes on GPU servers.

Created by **@eternaaall** 🧠

---

## 🔧 Features

- One-line install  
- Interactive CLI menu  
- Session-based prover management via `screen`  
- Auto-restart on failure  
- Key cleanup logic built-in  
- Mode switching: Only Eth, Scroll or Both  

---

## 📦 Quick Start (1 Command Install)

```bash
bash <(curl -s https://raw.githubusercontent.com/eternaaall/provercys_byetrnl/main/install.sh)
```

You will be prompted to enter your EVM wallet and RPC URL (for Eth).

---

## 📋 Menu Features

When running, the script presents a menu:

1. **Attach** to running prover session  
2. **Update script and mode** (removes old install + keys)  
3. **Reset key** and stop all sessions  
4. **Launch new prover session**  
5. **Exit**  

---

## 🧹 Key & Session Cleanup

- Keys are stored under `/root/cysic-prover/data/`
- They are deleted automatically during updates and full resets
- Screen sessions are used to keep provers running in background

---

## ⚙️ Requirements

The script installs:
- `screen`
- `curl`
- `pciutils`
- `lshw`

It automatically skips installation if already present.

---

## 🛡 License

MIT — Free to use and modify.

---

> ⭐ Found it useful? Consider giving the repo a star!
