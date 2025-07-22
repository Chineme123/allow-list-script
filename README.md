# 🛡️ Allow List Cleaner

A simple Python script to **sanitize an allow list of IP addresses** by removing any IPs found on a given deny list.

This is useful in network security or system administration contexts where access control needs to be updated automatically, especially after banning or blacklisting certain IPs.

---

## 📌 What It Does

- Accepts the path to a file containing **allowed IP addresses** (one per line).
- Accepts a list of **denied IP addresses** (e.g., from a blocklist or ban report).
- Reads the allow list file.
- Removes any IP address from the allow list if it exists in the deny list.
- Overwrites the original file with the updated allow list (safe set).

---

## 📦 Installation

No dependencies are required outside the Python standard library.

Requires **Python 3.6+**.

---

## 🚀 Usage

```bash
python update_allow_list.py
```

## 📂 File Format

**allowlist.txt**
```
192.168.0.10
172.16.0.1
10.0.0.5
```

**denylist**
```
[10.0.0.5, 192.168.0.10]
```

After running the script, the `allowlist.txt` will be updated to:
```
172.16.0.1
```

---

## ✅ Use Cases

- Firewall automation
- Network access control
- IP ban enforcement
- Dynamic security rulesets

---

## 🧑‍💻 Author

**Chineme**  
Software Engineer | Cybersecurity Enthusiast  
[GitHub](https://github.com/chineme123)
