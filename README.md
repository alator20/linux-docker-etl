# linux-docker-etl



1. In the file, there are 2 folders (input and output) and 1 python script. There are 2 csv files (t1 and t2) in the input folder.
2. Docker image included that will:
    -Use the python script to read the data from input folder.
    -Write the result data into output folder.
3. The python script is in the container.
4. The input and output folder is in the host, in another word, outside the container. What you need to do is to mount the 2 folders from host to the container.
5. make container running first, and then run python script. This means when you use docker run to start up the container, the python script will not run. The python script only runs when you give container an order with command docker exec.


Visual:


![Docker_lab_Process](https://user-images.githubusercontent.com/14003325/235817356-99b25489-b910-4514-911c-7e25d2fb5e7e.jpg)
