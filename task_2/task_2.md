### Task
Implement duplex pipe in C using some OOP principles (see example 1).
Maximize the performance of echo test (from parent to child and back) on huge files (> 4 Gb). The main metric is time spent on data transmission.
"Play" with buffer sizes and limits on pipe size.

### Notes:
1. Create big file if needed:
\# 4 Gb file:
time dd if=/dev/urandom of=file.txt bs=1048576 count=4096

2. If you want to check the data integrity, compare the checksums of input and received file:
md5sum <file_name>
