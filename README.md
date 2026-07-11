# SSLyze

This repository contains my practice, notes, and hands-on exercises while learning **SSLyze**, a Python-based SSL/TLS scanner used to analyze the security configuration of HTTPS servers.

## What is SSLyze?

SSLyze is an open-source tool that scans SSL/TLS configurations of web servers. It helps identify security issues by checking supported protocol versions, certificate validity, encryption settings, and known SSL/TLS vulnerabilities.

## Features

- Scan SSL/TLS configurations
- Inspect SSL certificates
- Check supported TLS versions
- Detect common SSL/TLS vulnerabilities
- Verify secure server configurations

---

# SSLyze Commands

## 1. Scan a Website

Performs a comprehensive SSL/TLS scan against the target server.

### Command

```bash
sslyze <Target-domain>
```

### Screenshot

<img width="998" height="656" alt="Screenshot 2026-07-11 125928" src="https://github.com/user-attachments/assets/6a0e7f6e-1fa6-4107-a752-40214140aea0" />


---

## 2. Certificate Information

Displays detailed information about the server's SSL/TLS certificate.

### Command

```bash
sslyze --certinfo <Target-domain>
```

### Screenshot

<img width="837" height="641" alt="Screenshot 2026-07-11 125945" src="https://github.com/user-attachments/assets/26349afc-1f9b-44b6-826b-a4266c942b14" />


---

## 3. Check TLS 1.3 Support

Checks whether the server supports the TLS 1.3 protocol.

### Command

```bash
sslyze --tlsv1_3 <Target-domain>
```

### Screenshot

<img width="1056" height="447" alt="Screenshot 2026-07-11 125958" src="https://github.com/user-attachments/assets/9c361461-9f49-4ddd-bdb7-6c04a100453b" />


---

## 4. Check for ROBOT Vulnerability

Tests whether the server is vulnerable to the ROBOT (Return Of Bleichenbacher's Oracle Threat) attack.

### Command

```bash
sslyze --robot <Target-domain>
```

### Screenshot

<img width="1047" height="457" alt="Screenshot 2026-07-11 130007" src="https://github.com/user-attachments/assets/09dbcd7a-54a3-4095-9838-8bb360fe4f2b" />


---

## 5. Check TLS Compression

Checks whether TLS compression is enabled, which could expose the server to CRIME attacks.

### Command

```bash
sslyze --compression <Target-domain>
```

### Screenshot

<img width="1053" height="448" alt="Screenshot 2026-07-11 130015" src="https://github.com/user-attachments/assets/3f248bd0-68b3-4708-8dc9-2328082f7ca3" />


---

## Disclaimer

This repository is created for **educational and ethical security learning purposes only**. Always obtain proper authorization before scanning or testing systems that you do not own or have explicit permission to assess.
