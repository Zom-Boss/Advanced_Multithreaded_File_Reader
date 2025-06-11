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


<br>
The "file_monitor.hpp" is used for reading a file and also notifying whenever the data inside a file is changed in real time . It also tells which thread chunks changed during a modification.
<br>
The "directory_monitor.cpp" is used for monitoring the directory. It instantiates a new instance of "FileChangeMonitor" class for each text file already present in the present directory. It also keeps monitoring the directory and whenever a new text file is introduced in the directory, another new instance of the class would be created.
<br>
The "multiple_thread.cpp" and "single_thread.cpp" in the code are here for speed comparisons between the two ways of file reading.
<br>
In the "multiple_thread.cpp" , only the calculation of hash and monitoring activities are removed form the "file_monitor.hpp" as we are just comparing the speed of reading
<br>

