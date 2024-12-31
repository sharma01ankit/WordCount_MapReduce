# WordCount_MapReduce
Title: Word Count Using MapReduce on Amazon Dataset
Objective:
The objective of this project is to process a large dataset (Amazon dataset) using Hadoop's MapReduce framework and find the count of occurrences for each word in the dataset. This process involves two main steps: mapping the dataset to word counts and reducing the results by aggregating counts for each word.
Approach:
1.	Mapper:
o	The mapper.py script reads the input dataset line by line.
o	It splits each line into words and emits each word with a count of 1.
2.	Reducer:
o	The reducer.py script aggregates the word counts. For each word, it sums up the occurrences of the word across all lines.
3.	Hadoop Streaming:
o	The program is executed using Hadoop's streaming API, allowing Python scripts to be used as MapReduce programs.
4.	Execution:
o	The job was submitted to Hadoop, processing the Amazon dataset stored in HDFS.
Tools Used:
•	Hadoop Streaming for running the Python MapReduce job.
•	HDFS for storing and processing the dataset.
•	Python for writing the Mapper and Reducer.
Steps to Run the Job:
1.	Prepare the Input: Upload the dataset to HDFS.
2.	Mapper and Reducer Scripts: Write Python scripts for the mapper and reducer.
3.	Run the MapReduce Job: Submit the job using Hadoop Streaming.
4.	Verify Output: Check the output in HDFS.
Verification of Output:
After executing the MapReduce job, the output can be verified by inspecting the word count results stored in the HDFS output directory.
