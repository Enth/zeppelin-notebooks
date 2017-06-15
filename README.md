
# Welcome to Enth
Enth is **n-dimensional awareness of data**.   Enth crawls networks, including private networks looking for data, structured, open, elastic, relational, text,.. Enth doesn’t ‘download’ this data, instead Enth **scans the data** as part of a machine learning process, in which Enth creates an **awareness of data**.  Enth uses this awareness of data to orchestrate the acquisition and transformation of data into **Spark**.  In other words, Enth tells Spark where to find specific data and what to do with it.

Enth-Spark-AI provides access to Enth.  This notebook contains information on installing Enth-Spark-AI into Apache Zeppelin, as well as provide some basic "How-To's" so you can quickly get going.  For more detailed information, please visit [Enth](http://www.enth.com).

### Installing Enth-Spark-AI ###

First, we need access Zeppelin's Interpreter Settings using setting icon on upper right corner of the notebook.


![Enth Interpreter Settings](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Interpreter.png)

Then, under Interpreter Settings, select **Interpreter** menu. 

Scroll down until you find the Spark Interpreter, then select **Edit**.

![Enth Interpreter Settings](https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Interpreter.png)

Once the edit mode is activated, scroll down until you find the **Dependencies Section**.  Within the Dependencies Section you will **Artifacts**.

![Enth Artifact Settings] (https://raw.githubusercontent.com/Enth/zeppelin-notebooks/master/Enth-Spark-AI%20Installation/images/Artifact.png)

As of this writing the current Snapshot is **com.geppetto.pintaillabs:enth-spark-AI:0.70-spark1.6-SNAPSHOT**, add this as the artifact, then select **Save**.  You will be asked if you are sure and if you want to restart the Spark Interpreter.  Select **OK**.
