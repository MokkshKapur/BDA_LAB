# ✅ HDFS Command Summary

## 1. List directories
```bash
hdfs dfs -ls /
```

## 2. Create an empty file
```bash
hdfs dfs -touchz /testfile.txt
```

## 3. Create a directory
```bash
hdfs dfs -mkdir /dirO
```

## 4. Remove a file
```bash
hdfs dfs -rm /testfile.txt
```

## 5. Remove a directory

- For **empty** directory:
  ```bash
  hdfs dfs -rmdir /dirO
  ```

- For **non-empty** directory:
  ```bash
  hdfs dfs -rm -r /dirO
  ```

## 6. Read contents of a file
```bash
hdfs dfs -cat /dirA/file1.txt
```

## 7. Copy a file from one directory to another
```bash
hdfs dfs -cp /dirA/file2.txt /dirB
```

## 8. Move a file from one directory to another
```bash
hdfs dfs -mv /dirA/file3.txt /dirB
```

## 9. Copy a file from local system to HDFS
```bash
hdfs dfs -put localFile.txt /dirC/
```

## 10. Copy a file from HDFS to local system
```bash
hdfs dfs -get /hdfsFile.txt /home/cloudera
```

## 11. HDFS Admin Report
```bash
hdfs dfsadmin -report
```
*(Correct spelling! In the video it was wrong.)*
