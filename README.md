# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/fdd0d66e-dd11-443e-9f46-9f5be481b7f9)

2.	Install java1.8 in folder /usr/local

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/cab30b09-b8d2-4a97-a0d6-ada83090b5f7)

3.	Install Hadoop

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/f9ccc9f9-edc3-486e-a5c2-60a8e977a884)

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/4f93c6e4-24ee-4cf7-8d5a-b2bde32a1db0)
 
5.	Set hadoop environment variables: Include the following lines /etc/profile file

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/84eb271b-8d1d-4cb3-a000-c509915e97be)

6.	Run the.bashrc & profile files from the $ prompt for updating the changes

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/78e76b27-5596-41dd-8e3e-1da4d1924860)

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/9d93c6f6-595d-42e9-a737-bd1a7ca947ae)

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/5ddbf2f0-6dfb-4b99-8cf7-5d4e9c28981a)

$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/bb55f39a-7421-445a-abe9-6dba66d032e7)

b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/6597475a-d5e2-45b4-bf19-d23c8f7182d5)

Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/ece80bcb-cc47-4fbb-8aa7-cdd170a52c52)

c)	mapred-site.xml
 
 ![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/5ae7a3e2-a6da-4c58-8793-970ba05406be)

Include the following lines in mapred-site.xml file
 
![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/f4d1409d-1ac4-43eb-b9d7-d5fce2bb5660)

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/bdbb87f6-5379-4df5-a9f9-6ac2aa02503f)

e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/c195eabf-4511-4348-a316-a00b77d0c049)

8.	Format the Hadoop File system implemented on top of the local file system using

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/789104d4-0c3b-4b25-9b60-df94606d2d36)

9.	Start Hadoop using

Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/4e2fe7b4-d2ef-46ab-b013-2773dd6f2183)

11.	Create a directory ‘/input’ in HDFS

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/5d592814-bc24-4186-9364-f0ae2225cf11)

12.	Copy the input files into the distributed file system

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/2a85102d-a4c8-4e34-ad13-000c08e96d41)

13.	Run some of the examples provided

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/80aecacc-8761-4978-9ca8-a1184547f488)

14.	Examine the output files

Copy the output files from the distributed file system to the local file system and examine them:

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/09101cbb-5b41-46e9-b112-3ca213ccbc71)
 
or
View the output files on the distributed file system

![image](https://github.com/kannan0071/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119641638/e135462e-265e-4f77-9f6e-1750ae9d9573)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
