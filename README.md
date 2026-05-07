<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="version">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="license">
  <img src="https://img.shields.io/badge/no-dependencies-brightgreen" alt="zero dependencies">
</p>

<h1 align="center">🔍 DragCodePick</h1>
<p align="center"><strong>File Encoding & String Extraction Toolkit</strong> / <strong>文件编码转换与字符串提取工具</strong></p>

<p align="center">A pure front-end, client-side toolkit for file encoding conversion, string pattern extraction, and CTF flag detection — all in a single HTML file.</p>

---

[简体中文](#简体中文) | [English](#english)

---

## English

### ✨ Features

- **File Encoding Conversion** — Encode/decode files in Base64, Base32, or Hex (Base16) with one-click copy and text file export
- **String Pattern Extraction** — Extract IPs, phone numbers, ID cards, email addresses, URLs, and other data from files
- **Credential Discovery** — Detect passwords, API keys, tokens, private keys, JWTs, AWS keys, connection strings, and Bearer tokens
- **Crypto String Detection** — Identify AES, DES, RSA, hash (MD5/SHA), HMAC, ECB mode patterns, and hex-encoded keys
- **CTF Flag Detection** — Auto-detect CTF flag formats and sensitive keywords (password, secret, token, etc.)
- **Drag & Drop** — Simple drag-and-drop file upload with instant processing
- **Chinese/English UI** — Bilingual interface with language toggle

### 🚀 Quick Start

Open `DragCodePick.html` directly in any modern browser. No build tools, no dependencies, no server required.

### 🛠️ Usage

1. **Drag & drop** a file onto the drop zone, or click to select one
2. Switch between the three tabs:
   - **Encoding** — Choose Base64/Base32/Hex to encode/decode the file content
   - **Extract** — Select pattern types (Identity/Credential/Crypto) to extract matching strings
   - **CTF** — Automatically scan for flag formats and security keywords
3. **Copy** results to clipboard or **Export** as `.txt` files

### 🏗️ Architecture

A single-file vanilla HTML/CSS/JS application with zero external dependencies (other than Google Fonts).

| Component      | Description                                                                              |
| -------------- | ---------------------------------------------------------------------------------------- |
| **CSS**  | Dark theme with glassmorphism effects, custom scrollbars, responsive layout              |
| **HTML** | Three tab-sections: Encoding, Extract (3 sub-tabs), CTF                                  |
| **JS**   | FileReader, Uint8Array processing, custom Base32/Base16 encoders, regex-based extraction |

### 📋 Supported Patterns

| Category             | Types                                                                                           |
| -------------------- | ----------------------------------------------------------------------------------------------- |
| **Identity**   | IP addresses, phone numbers, Chinese ID cards, email, URLs                                      |
| **Credential** | Passwords, API keys, tokens, RSA private keys, JWT, AWS keys, connection strings, Bearer tokens |
| **Crypto**     | AES, DES, RSA, MD5/SHA hashes, HMAC, ECB mode, hex keys                                         |

### ⚠️ Privacy

All file processing is **client-side only** — no data is ever sent to any server. Files are read via the browser's `FileReader` API and processed entirely in memory.

---

## 简体中文

### ✨ 功能特性

- **文件编码转换** — 支持 Base64 / Base32 / Hex (Base16) 编码解码，一键复制或导出为文本文件
- **字符串提取** — 从文件中提取 IP 地址、手机号、身份证号、邮箱、URL 等数据
- **凭证发现** — 检测密码、API 密钥、Token、私钥、JWT、AWS 密钥、连接字符串、Bearer Token
- **加密字符串检测** — 识别 AES、DES、RSA、哈希（MD5/SHA）、HMAC、ECB 模式及 Hex 编码密钥
- **CTF Flag 检测** — 自动搜索 CTF Flag 格式及安全敏感关键词（password、secret、token 等）
- **拖拽上传** — 简洁的拖拽文件操作，即时处理
- **中英文界面** — 双语界面，一键切换

### 🚀 快速开始

直接用浏览器打开 `DragCodePick.html`。无需构建工具，无需依赖，无需服务器。

### 🛠️ 使用方法

1. **拖拽文件**到拖拽区域，或点击选择文件
2. 切换三个功能标签页：
   - **编码转换** — 选择 Base64/Base32/Hex 进行编码/解码
   - **信息提取** — 勾选提取类型（身份信息/凭证/加密），提取匹配的字符串
   - **CTF 检测** — 自动扫描 CTF Flag 格式和安全关键词
3. **复制**结果到剪贴板或**导出**为 `.txt` 文件

### 🏗️ 架构

单文件纯原生 HTML/CSS/JS 应用，无外部依赖（仅引用 Google Fonts）。

| 组成部分       | 说明                                                                            |
| -------------- | ------------------------------------------------------------------------------- |
| **CSS**  | 深色主题，玻璃拟态效果，自定义滚动条，响应式布局                                |
| **HTML** | 三个功能区域：编码转换、信息提取（3 个子标签）、CTF 检测                        |
| **JS**   | FileReader + Uint8Array 读取原始字节、自定义 Base32/Base16 编码器、正则匹配提取 |

### 📋 支持的模式

| 类别               | 类型                                                                     |
| ------------------ | ------------------------------------------------------------------------ |
| **身份信息** | IP 地址、手机号码、身份证号、电子邮箱、URL                               |
| **凭证**     | 密码、API 密钥、Token、RSA 私钥、JWT、AWS 密钥、连接字符串、Bearer Token |
| **加密**     | AES、DES、RSA、MD5/SHA 哈希、HMAC、ECB 模式、Hex 密钥                    |

### ⚠️ 隐私说明

所有文件处理**完全在客户端进行**——不会将任何数据发送到服务器。通过浏览器的 `FileReader` API 读取文件，全部在内存中处理。

---

## 📄 License

MIT
