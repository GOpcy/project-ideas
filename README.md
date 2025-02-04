# Ideas for projects
- [[#1. Advanced Golang Project Ideas|1. Advanced Golang Project Ideas]]
  - [[#1. Advanced Golang Project Ideas#Concurrency & Channels|Concurrency & Channels]]
  - [[#1. Advanced Golang Project Ideas#System Tools|System Tools]]
  - [[#1. Advanced Golang Project Ideas#Networking & WebSockets|Networking & WebSockets]]
  - [[#1. Advanced Golang Project Ideas#Security & Cryptography|Security & Cryptography]]
  - [[#1. Advanced Golang Project Ideas#Compilers & Low-Level Programming|Compilers & Low-Level Programming]]
  - [[#1. Advanced Golang Project Ideas#Game Development|Game Development]]
  - [[#1. Advanced Golang Project Ideas#Which One Should You Start?|Which One Should You Start?]]

- [[#2. Other Project Ideas|2. Other Project Ideas]]
  - [[#2. Other Project Ideas#Visualization & Interactive Tools|Visualization & Interactive Tools]]
  - [[#2. Other Project Ideas#Desktop Applications|Desktop Applications]]
  - [[#2. Other Project Ideas#Game Development|Game Development]]
  - [[#2. Other Project Ideas#Low-Level & Systems Programming|Low-Level & Systems Programming]]
  - [[#2. Other Project Ideas#Which One Should You Start?|Which One Should You Start?]]

## 1. Advanced Golang Project Ideas

### **Concurrency & Channels**
#### 1. Parallel Web Scraper
- Extend your existing scraper to handle multiple pages concurrently.
- Use **goroutines + channels** to process multiple URLs at the same time.
- Implement a worker pool pattern.

#### 2. Distributed URL Shortener
- Upgrade your **URL shortener** project into a **distributed service** with multiple instances communicating.
- Learn about **gRPC, concurrency, and load balancing**.
- Store short URLs in a **distributed key-value store** like **etcd**.

#### 3. Load Balancer
- Build a simple **HTTP load balancer** that distributes requests to multiple backend servers.
- Implement **round-robin or least connections algorithms** using Go’s concurrency model.

#### 4. Concurrent File Downloader
- Split large files into chunks and download them concurrently.
- Use **goroutines, worker pools, and channels**.
- Implement retry logic and download resumption.

---

### **System Tools**
#### 5. System Resource Monitor (like `htop`)
- Track **CPU, RAM, disk, network usage** in real-time.
- Use **Go's `runtime` package** to get system stats.
- Build a **CLI interface** using a library like **`tview` or `termui`**.

#### 6. Key-Value Database (Mini Redis)
- Implement an in-memory **key-value store** that supports **GET, SET, DELETE** commands.
- Use **Go’s `sync.Map` for concurrency**.
- Add a **TCP or HTTP interface** for clients.
- Implement **persistence** (write logs to disk).

### 7. Static Code Analyzer for Go (Like `golangci-lint`)
- Write a CLI tool that scans Go code and detects **inefficient code patterns**.
- Use **Go's `go/parser` package** to analyze AST (Abstract Syntax Tree).

---

### **Networking & WebSockets**
#### 8. Terminal-Based Chat App (WebSockets & CLI UI)
- Implement a **WebSocket server** in Go.
- Clients will connect via a **CLI interface** (like Slack for terminals).
- Learn **channels** for handling multiple connections.

#### 9. P2P File Sharing System
- Build a simple **peer-to-peer file sharing** system.
- Use **WebSockets, TCP, or gRPC** to communicate.
- Learn how to use **Goroutines & Mutexes** to handle concurrent transfers.

---

### **Security & Cryptography**
#### 10. Password Manager (CLI + Encryption)
- Store passwords in an **encrypted** local database.
- Use **AES encryption** (`crypto/aes`).
- Implement a CLI interface for adding/retrieving passwords.

#### 11. VPN or Proxy Server
- Build a **simple VPN** using **Go’s net package**.
- Use **encryption** to create a secure tunnel.
- Learn **how TCP/UDP networking works**.

#### 12. Secure Chat App (End-to-End Encryption)
- Encrypt messages with **AES or RSA** before sending via WebSockets.
- Implement secure **key exchange** (Diffie-Hellman).
- Learn **TLS and secure communications** in Go.

---

### **Compilers & Low-Level Programming**
#### 13. Tiny Golang Virtual Machine (Like a mini-JVM)
- Implement a stack-based **bytecode interpreter**.
- Write an assembler to compile simple programs into bytecode.
- Learn about **parsing, memory management, and execution models**.

#### 14. Embedded Web Server (Without Using `net/http`)
- Build an HTTP server **from scratch** using raw TCP sockets.
- Implement **request parsing, routing, and response handling**.
- Learn about **how HTTP servers work internally**.

---

### **Game Development**
#### 15. Multiplayer Game (Goroutines + WebSockets)
- Make a simple **multiplayer turn-based game** (like Chess or Tic-Tac-Toe).
- Use **WebSockets for real-time communication**.
- Handle multiple players using **Goroutines & Channels**.

#### 16. Game AI Bot
- Train a bot to play **Tetris or Space Invaders**.
- Use **Reinforcement Learning** (Q-Learning).
- Implement decision-making using **Go routines for concurrent processing**.

---

### **Which One Should You Start?**
If you want to **learn concurrency**:
- **Parallel Web Scraper**  
- **Load Balancer**  
- **Concurrent File Downloader**  
- **WebSocket Chat App**  

If you want to **learn advanced Go concepts (interfaces, AST, reflection)**:
- **Static Code Analyzer**  
- **Mini Redis Clone**  
- **Key-Value Database**  

If you want to **build something useful**:
- **Password Manager**  
- **System Monitor**  
- **P2P File Sharing**



## 2. Other Project Ideas

### **Visualization & Interactive Tools**
#### 1. Algorithm Visualizer
- Create an interactive tool to visualize algorithms like sorting, pathfinding (A*, Dijkstra), and recursion.
- Use **HTML/CSS + JavaScript** for a web-based visualizer.

#### 2. Heardle Clone (with Spotify API)
- Create a music guessing game similar to Heardle.
- Use **Spotify’s Web API** to fetch song previews.
- Optionally: Allow users to log in with **OAuth** and track scores.

---

### **Desktop Applications**
#### 3. Music Player Web/Desktop
- A lightweight music player supporting playlists, audio visualization, and media controls.
- Use **Electron** or **Any other language for desktop** for a cross-platform UI.
- Implement features like **custom equalizer, streaming support, and lyrics integration**.

#### 4. Pomodoro Timer Desktop App
- A productivity timer app with customizable sessions and notifications.
- Use **Electron (JavaScript)** for a desktop version.
- Add **to-do lists, statistics, and break reminders**.

#### 5. Text Editor
- Build a simple text editor with **syntax highlighting, search, and markdown preview**.
- Use **Golang, C, Zig, any other language**.
- Implement plugins, autosave, and optionally cloud sync.

---

### **Game Development**
#### 6. 2D Space Invaders Game
- A classic arcade game with a retro feel.
- Use **Unity (C#), Godot (GDScript), or Pygame (Python)**.
- For more challanging, try not using an engine in **Golang, C, Zig, any other language**
- Add levels, power-ups, and high-score tracking.

#### 7. CLI Tetris
- A command-line version of Tetris.
- Implement in **Golang, C, Zig, any other language**.
- Use **ncurses (Linux) or a basic ASCII renderer**.

---

### **Low-Level & Systems Programming**
#### 8. Mini Operating System (C or Zig)
- Develop a small OS kernel that boots and runs basic tasks.
- Learn **bootloaders, memory management, and system calls**.
- Use **Assembly + C or Zig** with **QEMU for testing**.

#### 9. Small Compiler (C or Zig)
- Build a simple compiler for a custom language or a subset of an existing one.
- Learn **parsing, tokenization, and code generation**.
- Target **LLVM IR, WASM, or assembly**.

---

### **Which One Should You Start?**
If you want to **learn frontend & interactivity**:
- **Algorithm Visualizer**  
- **Heardle Clone**  
- **Pomodoro Timer**  

If you want to **learn systems programming**:
- **Mini Operating System**  
- **Small Compiler**  

If you want to **build a fun game**:
- **2D Space Invaders**  
- **CLI Tetris**  

If you want to **develop useful desktop apps**:
- **Desktop Music Player**  
- **Text Editor**  
