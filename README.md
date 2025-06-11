# Advanced_Multithreaded_File_Reader
## 📌 Project Goals

The primary goals of this project are:

- ✅ **Efficient Multi-threaded File Reading**:  
  To develop a multi-threaded file reader capable of handling large files by dividing the data into chunks and processing them in parallel.

- 💡 **Optimized I/O with Buffered Reading**:  
  To implement a buffered reading mechanism that minimizes I/O overhead and improves performance.

- 🔄 **Real-time File Modification Detection**:  
  To design a robust detection mechanism that monitors real-time file modifications without interrupting or corrupting the ongoing reading process.

- ⚙️ **Performance Benchmarking**:  
  To evaluate and compare the performance of the multi-threaded approach against a traditional single-threaded file reading approach.

## 📁 File Descriptions

- **`file_monitor.hpp`**  
  This header file is responsible for reading a file and detecting real-time changes in its content. It identifies and notifies which specific thread-handled chunks of the file have been modified.

- **`directory_monitor.cpp`**  
  This source file monitors the current directory for text files. It creates a new instance of the `FileChangeMonitor` class for each `.txt` file present. Additionally, it continuously observes the directory, and whenever a new text file is added, a corresponding new monitor instance is created automatically.

- **`multiple_thread.cpp`**  
  This file demonstrates multi-threaded file reading. It is used for performance benchmarking and comparison. In this version, hash calculation and real-time monitoring functionalities (originally from `file_monitor.hpp`) are removed to strictly focus on read speed.

- **`single_thread.cpp`**  
  This file implements the single-threaded approach for reading files. It is used to compare performance against the multi-threaded method.


