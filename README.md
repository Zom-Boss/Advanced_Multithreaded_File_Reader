# Advanced_Multithreaded_File_Reader
<br>
The "file_monitor.hpp" is used for reading a file and also notifying whenever the data inside a file is changed in real time . It also tells which thread chunks changed during a modification.
<br>
The "directory_monitor.cpp" is used for monitoring the directory. It instantiates a new instance of "FileChangeMonitor" class for each text file already present in the present directory. It also keeps monitoring the directory and whenever a new text file is introduced in the directory, another new instance of the class would be created.
<br>
The "multiple_thread.cpp" and "single_thread.cpp" in the code are here for speed comparisons between the two ways of file reading.
<br>
In the "multiple_thread.cpp" , only the calculation of hash and monitoring activities are removed form the "file_monitor.hpp" as we are just comparing the speed of reading
<br>

