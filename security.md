
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=2,14,29&height=220&section=header&text=Easy%20Logs&fontSize=90&fontColor=ffffff&animation=scaleIn&fontAlignY=50&desc=Lightning-Fast%20Log%20Management%20for%20Developers&descAlignY=75&descSize=22" width="100%"/>

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&duration=3000&pause=800&color=06D6A0&center=true&vCenter=true&width=700&lines=Parse.+Analyze.+Debug.;No+more+grep+through+massive+files.;Find+the+needle+in+the+haystack." alt="Typing SVG"/>

<br/><br/>

<a href="https://share.google/fF4QyL1PNBzP2Xiyu">
  <img src="https://img.shields.io/badge/⚡_GET_STARTED-06D6A0?style=for-the-badge&logo=go&logoColor=white&labelColor=118AB2" height="50"/>
</a>
&nbsp;
<a href="https://share.google/fF4QyL1PNBzP2Xiyu">
  <img src="https://img.shields.io/badge/📥_DOWNLOAD-EF476F?style=for-the-badge&logo=icloud&logoColor=white&labelColor=9D0208" height="50"/>
</a>
&nbsp;
<a href="https://share.google/fF4QyL1PNBzP2Xiyu">
  <img src="https://img.shields.io/badge/📚_READ_DOCS-FFD166?style=for-the-badge&logo=readthedocs&logoColor=black&labelColor=FCA311" height="50"/>
</a>

<br/><br/>

<img src="https://img.shields.io/badge/version-2.4.1-118AB2?style=flat-square&logo=semanticrelease&logoColor=white"/>
<img src="https://img.shields.io/badge/license-Apache--2.0-06D6A0?style=flat-square&logo=apache&logoColor=white"/>
<img src="https://img.shields.io/badge/go-1.21+-00ADD8?style=flat-square&logo=go&logoColor=white"/>
<img src="https://img.shields.io/badge/build-passing-EF476F?style=flat-square&logo=githubactions&logoColor=white"/>
<img src="https://img.shields.io/badge/downloads-45K+-FFD166?style=flat-square&logo=github&logoColor=black"/>

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🚀 Stop Grepping. Start Analyzing.

**Easy Logs** is a powerful, high-performance command-line tool built to bring order to your chaotic log files. Whether you're debugging a microservice crash at 3 AM, analyzing access patterns, or extracting metrics from gigabytes of raw text, Easy Logs provides a blazing-fast, intuitive interface to query, filter, and visualize your data.

Written in Go, it compiles to a single binary with **zero external dependencies**, meaning you can drop it onto any server, run it, and get answers instantly. No heavy ELK stacks, no complex configurations — just pure, unadulterated log analysis.

> 💡 **Why Easy Logs?** Because `cat app.log | grep "ERROR" | awk '{print $5}'` is a nightmare to maintain. Easy Logs gives you a clean CLI syntax, instant JSON/CSV parsing, and live tailing out of the box.

<br/>

<table align="center" width="100%">
<tr>
<td align="center" width="25%">

### ⚡
**Blazing Fast**
Built in Go. Processes 1GB+ of logs in seconds using parallel chunking.

</td>
<td align="center" width="25%">

### 🧩
**Universal Parser**
Auto-detects JSON, CSV, Apache, Nginx, and custom regex log formats.

</td>
<td align="center" width="25%">

### 🎯
**Smart Filtering**
Query with SQL-like syntax or complex regex without writing scripts.

</td>
<td align="center" width="25%">

### 📊
**Live Analytics**
Real-time tailing with interactive terminal dashboards.

</td>
</tr>
</table>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## ⚡ Why Easy Logs Stands Out

<div align="center">

| 🧩 **The Challenge** | 💡 **Our Solution** | 📈 **The Result** |
|:---|:---|:---|
| Traditional tools choke on multi-GB log files | **Memory-mapped I/O and concurrent chunking** | Analyze 10GB files in under 5 seconds |
| Inconsistent log formats break standard tools | **Auto-detection parser** for JSON, CSV, and standard syslogs | One tool for all your microservices |
| Searching for specific errors is tedious | **SQL-like query engine** directly in the terminal | Type `SELECT * WHERE status = 500` and hit enter |
| Setting up log viewers is complex | **Zero configuration, single binary** | Download, run, and instantly view logs |

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 Core Features

<div align="center">

| 🔍 **Instant Search** | 🌪️ **Regex Support** | 📂 **Multi-File Merge** |
|:---:|:---:|:---:|
| Fuzzy finding and exact matching across millions of lines | Full support for Go's RE2 syntax for complex pattern matching | Combine logs from multiple servers into a single timeline |

| 📺 **Live Tail** | 📤 **Export Options** | 🛡️ **Privacy First** |
|:---:|:---:|:---:|
| Watch files grow in real-time with color-coded output | Export filtered results to JSON, CSV, or standard text | 100% offline. Your logs never leave your machine |

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🖼️ Interface Preview

<div align="center">

<img width="632" height="316" alt="images (37)" src="https://github.com/user-attachments/assets/98281301-dedb-4d8d-a0b3-665cfcae1dae" />


</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🚀 Quick Start

> **Three commands. Under two minutes. No installers.**

### 1️⃣ Install via Go

```bash
go install github.com/yourname/easylogs@latest
```

### 2️⃣ Analyze a log file

```bash
easylogs parse -f /var/log/nginx/access.log
```

### 3️⃣ Run a smart query

```bash
easylogs query -f app.log -q "WHERE level = 'ERROR' AND response_time > 500"
```

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## ⌨️ CLI Commands

<div align="center">

| Command | Description |
|:---|:---|
| `easylogs parse <file>` | Auto-detect format and print a summary |
| `easylogs query <file> -q "..."` | Filter logs using SQL-like syntax |
| `easylogs tail <file>` | Live tail with syntax highlighting |
| `easylogs export <file> --format=csv` | Convert logs to CSV/JSON |
| `easylogs stats <file>` | Show error rates, request times, and top IPs |

</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## ⚙️ Architecture

<div align="center">

| Layer | Responsibility | Tech |
|:---|:---|:---|
| ⚡ **Ingestion** | Reads files via memory-mapped I/O for zero-copy speed | Go `mmap` |
| 🧠 **Parsing Engine** | Auto-detects format and tokenizes lines | Custom Go lexers |
| 🔍 **Query Processor** | Translates SQL-like syntax into executable filters | Go AST |
| 🎨 **Output Renderer** | Formats to the terminal, JSON, or CSV | ANSI / Stdout |

</div>

Easy Logs is built with a modular pipeline. You can plug in your own custom parser or output format by implementing a simple Go interface.

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧠 Pro Tips

<table align="center" width="100%">
<tr>
<td width="50%">

**For maximum speed**
- 🚀 Use an SSD for log storage
- 📦 Pipe output to `less -R` for large results
- 🔍 Use exact matches instead of regex when possible
- 🧵 Increase worker threads with `--threads=8`

</td>
<td width="50%">

**For complex debugging**
- 🎨 Combine multiple files with `-f *.log`
- 📊 Use `stats` for a quick health check
- ⏱️ Filter by timestamp with `--since="1 hour ago"`
- 💾 Save frequent queries as aliases in config

</td>
</tr>
</table>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## ❓ Frequently Asked Questions

<details>
<summary><b>Does it work on Windows?</b></summary>

Yes! Easy Logs compiles to native binaries for Windows, macOS, and Linux. It also runs perfectly inside WSL.
</details>

<details>
<summary><b>Can I use it with Docker?</b></summary>

Absolutely. The tool is available as a minimal Alpine-based Docker image (`docker pull easylogs/cli`). You can mount your log directory and run queries directly.
</details>

<details>
<summary><b>How does it handle huge files?</b></summary>

Easy Logs uses memory-mapped I/O and concurrent chunking. It doesn't load the entire file into RAM, allowing it to process files larger than your system's memory.
</details>

<details>
<summary><b>Does it support custom log formats?</b></summary>

Yes. You can define a custom regex pattern in the config file to parse any proprietary log format your application uses.
</details>

<details>
<summary><b>How do I report a bug?</b></summary>

Open an issue on the GitHub repository with your **OS**, **Go version**, and the **exact command** that failed. If possible, include a snippet of the log file (redacted).
</details>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>



<div align="center">

<a href="https://share.google/fF4QyL1PNBzP2Xiyu">
  <img src="https://img.shields.io/badge/⚡_START_USING_EASY_LOGS-06D6A0?style=for-the-badge&logo=go&logoColor=white&labelColor=118AB2" height="55"/>
</a>

<br/><br/>

**⭐ If this tool saved you hours of debugging — star the repo!**

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,14,29&height=140&section=footer&text=Parse.+Analyze.+Debug.&fontSize=22&fontColor=06D6A0" width="100%"/>

</div>
