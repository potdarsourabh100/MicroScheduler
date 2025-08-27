📌 Microscheduler – Lightweight Embedded Task Scheduler

Microscheduler is a lightweight, portable, open-source task scheduler designed for resource-constrained embedded systems.
It provides preemptive scheduling, round-robin execution, inter-task communication, synchronization, and timers — all without being tied to a specific microcontroller.

With its clean platform abstraction layer, Microscheduler can run on bare-metal MCUs (e.g., STM32, ESP32, nRF, AVR) or on a POSIX system (Linux/macOS) for development and simulation.

✨ Features

🕒 Pre-emptive, time-based, and round-robin scheduling

📦 Message queues for inter-task communication

🔒 Semaphores for synchronization and resource protection

⏲ Software timers (one-shot and periodic)

🧩 Custom memory allocator (dynamic allocation with simple APIs)

🌍 Portable design using a platform.c/.h layer

⚡ Runs on POSIX (Linux/macOS) and easily portable to any MCU

📂 Project Structure
