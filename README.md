Critical Thinking (2 points total) Modify this ReadMe file to answer the following questions directly in place.


i.Kaggle changes links/ file locations/login process/ file content
The problem for users is difficulty / fail to access the original data sets, when the system fetching the old link. 
Now, Kaggle has set up “Input Files” in Kaggle Kernels. Kaggle Kernels can directly load the data sets, also able to use R / Python to practice ML models. Kaggle Kernels has been created to solve this problem.  Users don’t need to download data sets in local space, directly accessing the data/meta data through Kaggle website. It has much more convenience for user without problem loading big data sets into their local hard drive.  
https://www.kaggle.com/dansbecker/finding-your-files-in-kaggle-kernels



ii.We run out of space on HD / local permissions issue - can't save files
Apache Hadoop is a collection of open-source software utilities that facilitate using a network of many computers to solve problems involving massive amounts of data and computation. t provides a software frame work for distributed storage and processing of big data using the MapReduce programming model. 
However, The model training process in big data machine learning is both computation- and memory-intensive. Many parallel machine learning algorithms consist of iterating a computation over a training dataset and updating the related model parameters until the model converges. In the Big Data era, both the volume of a dataset and the number of model parameters can be huge. To accelerate the performance of the iterative computation, it’s common to cache the training data and model parameters into memory. However, due to the limitations of memory, in many scenarios, it might not all fit. It’s a challenge to run machine learning training algorithms efficiently with memory constraints.
Apache Spark started in 2009 as a research project at UC Berkley’s AMPLab, a collaborate on involving students, researchers, and faculty, focused on data-intensive application domains. The goal of Spark was to create a new framework, optimized for fast iterative processing like machine learning, and interactive data analysis, while retaining the scalability, and fault tolerance of Hadoop MapReduce. 
Spark is an open source framework focused on interactive query, machine learning, and real-time workloads. It does not have its own storage system, but runs analytics on other storage systems like HDFS, or other popular stores like Amazon Redshift, Amazon S3, Couchbase, Cassandra, and others. Spark on Hadoop leverages YARN to share a common cluster and dataset as other Hadoop engines, ensuring consistent levels of service, and response.

https://en.wikipedia.org/wiki/Apache_Hadoop
https://medium.com/@Petuum/a-solution-to-the-memory-limit-challenge-in-big-data-machine-learning-49783a72088b
https://aws.amazon.com/big-data/what-is-spark/?trk=ps_a131L000005ivBSQAY&trkCampaign=pac_emr_webpage_big_data_what%27s_spark&sc_channel=ps&sc_campaign=pac_q2-04-2018_emr_paid_search&sc_outcome=Product_Adoption_Campaigns&sc_geo=NAMER&sc_country=mult&sc_publisher=Google&sc_medium=PAC-PaaS-P|PS-GO|Non-Brand|Desktop|PA|Analytics|EMR|US|EN|Text&s_kwcid=AL!4422!3!301096469481!p!!g!!big%20data&ef_id=W3OMpwAAAI7aSGvT:20181013202256:s




iii.Someone updated python packages and there is unintended effect (functions retired or act differently)
A side effect refers simply to the modification of some kind of state - for instance:
•Changing the value of a variable;
•Writing some data to disk;
•Enabling or disabling a button in the User Interface.
Contrary to what some people seem to be saying:
•A side effect does not have to be hidden or unexpected (it can be, but that has nothing to do with the definition as it applies to computer science);
•A side effect has nothing to do with idempotency. An idempotent function can have side effects, and a non-idempotent function may have no side effects (such as getting the current system date and time).

https://softwareengineering.stackexchange.com/questions/40297/what-is-a-side-effect


iv.Docker issues - lost internet within docker due to some ip binding to vm or local routing issues( I guess this falls under lost internet, but I am talking more if docker is the cause rather then ISP)
•Docker containers can connect to the outside world without further configuration, but the outside world cannot connect to Docker containers by default. A bridge network is created (with the name bridge) when you install Docker. Every outgoing connection appears to originate from the host’s IP space; Docker creates a custom iptables masquerading rule.
•“standard Masq-HOWTO describes how to enable the Linux IP Masquerade feature on a given Linux host. IP Masq is a form of Network Address Translation or NAT that allows internally networked computers that do not have one or more registered Internet IP addresses to have the ability to communicate to the Internet via your Linux boxes single Internet IP address.”
•http://www.tldp.org/HOWTO/html_single/Masquerading-Simple-HOWTO/
•someone posted a solution for binding to VM docker-machine on stackoverflow:
•Here are some details to help those confused about adding a NIC to the VM in VirtualBox. I have only used VirtualBox for this and cannot advise about other virtualization system configurations.
•Stop the VM by selecting it in the VM Manager and using the right-click menu or pressing 'command-F'.
•Click "Settings".
•Click "Network".
•Select one of the Adapters that is not currently enabled.
•Enable it.
•Select "Bridged Adapter" in the "Attached to" selection.
•Click OK.
•Start your VM and try it out.
https://stackoverflow.com/questions/33021581/how-to-bind-the-vm-docker-machine-creates-to-osx-ip-address





