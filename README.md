# AWS - Big Data (Data Analytics) Specialty Exam Study Guide

Last year, I passed the [Google Cloud Professional Data Engineer](https://cloud.google.com/certification/data-engineer) certification exam and posted a [collection of study materials](https://github.com/Leverege/gcp-data-engineer-exam/blob/master/Data%20Engineering%20Notes.pdf) that I used to prepare for the exam. This year, I took the AWS equivalent exam, [AWS Big Data Specialty](https://aws.amazon.com/certification/certified-big-data-specialty/), which covers AWS Big Data services (e.g. Kinesis, Redshift, EMR) and design choices to run big data solutions on AWS. In April, the exam is gettig a new name, AWS Certified Data Analytics Specialty, but the materials covered seem to still test the life cycle of collection, ingestion, storage, processing, and visualization of data. I hope this study guide is helpful in passing the exam on your first try! 

## Exam Format
The AWS Certified Big Data Specialty exam consists of approximately 65 multiple choice questions (the exact number of questions may vary). You have 170 minutes to complete the exam at a certified test location. The [official exam guide](https://d1.awsstatic.com/training-and-certification/docs-bigdata-spec/AWS%20Certified%20Big%20Data%20-%20Specialty_Exam%20Guide_v1.4_FINAL.pdf) details the distribution of the exam questions per domain (i.e. collection, storage, processing, analysis, visualization, and data security), but in practice, I found it easier to approach the exam by focusing on the relevant AWS products, namely EMR, Redshift, DynamoDB, and Kinesis. 

I found the [official sample exam questions](https://d1.awsstatic.com/training-and-certification/docs-bigdata-spec/BD-S%20Sample%20Questions%20for%20Web.pdf) to be slightly more difficult than the actual exam. For the most part, the actual exam had four choices with a combination of two products/approaches that allowed you to quickly rule out two of the answers. For example, a question might ask about a scenario involving a NoSQL database with Kinesis data streams and the choices would be some combination of DynamoDB, Kinesis, and RDS. You can rule out the answer with RDS and narrow it down to the answers involving DynamoDB from there. 

## Study Plan
Since this is an AWS Big Data exam, it's imperative to know the key AWS Big Data and Machine Learning products and understand the recommended architectural patterns. While having hands on experience with AWS toolset is best, the test assesses your high-level understanding of the data life cycle, security, and integration between the products more so than hands-on details. In other words, the exam does not expect to you to memorize the instance types and all the debug messages from Redshift, but will ask you to design a DynamoDB table based on design constraints. 

There were several questions on security best practices including encryption and IAM as well as recovery mechanisms both within regions and globally. Take some time to read through the FAQ section for each of these products as encryption options and back up mechanisms differed slightly from product to product. For general AWS Big Data knowldge, [AWS whitepapers](https://aws.amazon.com/whitepapers/) and reInvent videos referenced from A Cloud Guru or Linux Academy proved to be the most useful. 

Overall, there was a heavy emphasis on design, troubleshooting, and optimization of big data scenarios involving EMR, Redshift, and DynamoDB in that order. A common type of problem was asking how to design a solution given certain limitations or to re-design an existing solutiion to optimize for cost, complexity, or time to market (e.g. using a managed service like Kinesis Firehose vs. using Kafka). 

Finally, there were a few questions asking for which Hadoop product to use in a certain situations (e.g. Presto vs. Hive vs. Sqoop) and a couple of easy questions about what type of visualizations to use on QuickSight (e.g. line chart vs. bar chart). 

I hope that the [exam study guide](https://github.com/Yitaek/aws-big-data-exam/blob/master/AWS%20Big%20Data%20Specialty%20Study%20Guide.pdf) helps you pass the test. If you notice any inaccuracies or want to contribute, feel free to leave a issue! 

## Resources
Practice Questions:
- https://www.aws.training/Details/Curriculum?id=21332
- https://www.whizlabs.com/aws-certified-big-data-specialty
- https://www.study4exam.com/amazon/aws-certified-big-data-specialty-questions-pdf

Other Exam Overviews/Debriefs:
- https://medium.com/@simonleewm/my-path-to-aws-big-data-speciality-certification-4baff3a8150
- https://towardsdatascience.com/how-did-i-get-certified-with-aws-big-data-specialty-e26f20114d3c
- https://ashwin.cloud/blog/aws-certified-big-data-specialty/

Courses:
- https://acloud.guru/learn/aws-certified-big-data-specialty
- https://linuxacademy.com/course/aws-certified-big-data-specialty-course
