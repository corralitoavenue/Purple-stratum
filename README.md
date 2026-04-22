# BitcoinPurple Stratum (CKPool)

This repository contains the Stratum mining server for BitcoinPurple, based on CKPool.

---

## ⚙️ Build Instructions

To compile the stratum server from source:

```bash
./autogen.sh
./configure
make
```

---

## 🚀 Running the Stratum

Before starting the pool, you must create a configuration file.

### 1. Create Configuration File

Create a `.conf` file (for example `ckpool.conf`) and configure:

- RPC connection to your BitcoinPurple node  
- Ports  
- Wallet address  
- Pool settings  

---

### 2. Start the Stratum Server

From the `src` directory:

```bash
./ckpool -c /path/to/your/ckpool.conf
```

Example:

```bash
./ckpool -c ../ckpool.conf
```

---

## 🔧 Features

### 🔹 Variable Difficulty (VarDiff)

Variable difficulty (VarDiff) is supported and can be enabled via the configuration file.

This allows the pool to automatically adjust miner difficulty based on hashrate, improving efficiency and reducing server load.

---

## 📄 Notes

- Make sure your BitcoinPurple node is fully synced before starting the pool.  
- Ensure RPC credentials in the configuration file are correct.  
- The pool requires a valid wallet address to operate.  

---

## 📜 License

See the LICENSE file for details.
