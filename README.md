
# Welcome to Enth

<img src="http://enth.com/Images/Enth%20Logo.png" alt="Enth"/>
style="width:1366px; height: 496px;"/>

Enth is **n-dimensional awareness of data**.   Enth crawls networks, including private networks looking for data, structured, open, elastic, relational, text,.. Enth doesn’t ‘download’ this data, instead Enth **scans the data** as part of a machine learning process, in which Enth creates an **awareness of data**.  Enth uses this awareness of data to orchestrate the acquisition and transformation of data into **Spark**.  In other words, Enth tells Spark where to find specific data and what to do with it.

Enth-Spark-AI provides access to Enth.  This notebook contains information on installing Enth-Spark-AI into Apache Zeppelin, as well as provide some basic "How-To's" so you can quickly get going.  For more detailed information, please visit [Enth](http://www.enth.com).

### Installing Enth-Spark-AI ###

First, we need access Zeppelin's Interpreter Settings using setting icon on upper right corner of the notebook.

![Enth Settings](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Settings.png)

Then, under Interpreter Settings, select **Interpreter** menu. 

Scroll down until you find the Spark Interpreter, then select **Edit**.

![Enth Interpreter Settings](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Interpreter.png)

Once the edit mode is activated, scroll down until you find the **Dependencies Section**.  Within the Dependencies Section you will **Artifacts**.

![Enth Artifact Settings](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Artifact.png)

As of this writing the current Snapshot is **com.geppetto.pintaillabs:enth-spark-AI:0.70-spark1.6-SNAPSHOT**, add this as the artifact, then select **Save**.  You will be asked if you are sure and if you want to restart the Spark Interpreter.  Select **OK**.

### Adding the Snapshot Repository (optional) ###

If you are using a SNAPSHOT version of Enth-Spark-AI, you will need to add the **Snapshot Repository**.  Scroll to the top of the Interpreter page and select **Repository**.

![Enth Zeppelin Repository](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Repository.png)

Next to you current Repositories you should see a **+**.  Select the **+** to add a repository.  The **ID** is "snapshots".  The **URL** is "https://oss.sonatype.org/content/repositories/snapshots/" and next to **Snapshot** select TRUE (because it is)!  Select **Add**.

![Enth Zeppelin Repository](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/NewRepository.png)

You will need to restart your Zeppelin instance to complete the download and installation.

You can also naviage to https://oss.sonatype.org/content/repositories/snapshots/com/geppetto/pintaillabs/enth-spark-AI to find the most current Snapshot version.

### Test the Enth-Spark-AI installation! ###

In a new notebook, add a new paragraph and type the following, then run the paragraph.  You should see the following.  The highlighting portion represents the JSON plan created by Enth to satisfy your search request.

![Enth Zeppelin Repository](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Enth%20Success.png)

To see some actual results...try the following.  

![Enth Zeppelin Repository](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Results.png)

### Troubleshooting ###

1)  The first step in troubleshooting is to check the log!  Check [zeppelin home]/logs.  Look for 'Enth'.

2)  If Zeppelin replies with "error:  obect geppetto is not a memeber of package com", as shown below, this is most likely an installation problem. 

Check [zeppelin home]/local-repo/com/geppetto/pintaillabs/enth-spark-AI/[version].  The folder should exist and contains several files.  Try restarting, if that still fails, try to reinstall.

![Enth Zeppelin Repository](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Error.png)

3)  If you see "memory error"  in the logs or as a response to running your paragraph.  Check the memory available for your machine and check the amount allocated for Zeppelin.  Check the documentation for increasing memory for your version of Zeppelin. Look for 'zeppelin-env.sh'.

![Enth Zeppelin Repository](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Memory%20Error.png)
