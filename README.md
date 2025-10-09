## 📌 Microscheduler – Lightweight Embedded Task Scheduler

Microscheduler is a lightweight, portable, open-source task scheduler designed for resource-constrained embedded systems.
It provides preemptive scheduling, round-robin execution, inter-task communication, synchronization, and timers — all without being tied to a specific microcontroller.

With its clean platform abstraction layer, Microscheduler can run on bare-metal MCUs (e.g., STM32, ESP32, nRF, AVR) or on a POSIX system (Linux/macOS) for development and simulation.

## ✨ Features

🕒 Pre-emptive, time-based, and round-robin scheduling

📦 Message queues for inter-task communication
🔒 Semaphores for synchronization and resource protection
⏲ Software timers (one-shot and periodic)
🧩 Custom memory allocator (dynamic allocation with simple APIs)
🌍 Portable design using a platform.c/.h layer
⚡ Runs on POSIX (Linux/macOS) and easily portable to any MCU

## 📂 Project Structure
```bash
microscheduler/
 ├── include/           # Public headers
 ├── src/               # Core implementation
 ├── ports/             # Platform ports (POSIX, Cortex-M template)
 ├── examples/          # Example applications (POSIX demo, MCU demo)
 ├── tests/             # Unit & integration tests (optional)
 ├── docs/              # Documentation and diagrams
 ├── CMakeLists.txt     # Cross-platform build
 ├── LICENSE
 ├── README.md
 └── CHANGELOG.md
 ```
## 🚀 Getting Started
Porting to an MCU

Implement platform.c/.h with:

Timer tick → ms_tick_isr()

Context switching (PendSV, or equivalent)

Task stack initialization

Link against src/ and include/ in your project.

## 🛠 Example Use Cases

Cooperative/preemptive multitasking on bare-metal MCUs

Lightweight RTOS alternative for small projects

Educational OS/RTOS design experiments

Cross-platform firmware component testing

## 📜 License

This project is released under the Apache 2.0.
