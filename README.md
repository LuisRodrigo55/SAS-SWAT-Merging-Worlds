# SAS-SWAT-Merging-Worlds
SAS Scripting Wrapper for Analytics Transfer (SWAT) package enable to execute code in SAS Viya and the Cloud Analytic Services (CAS) using native Python and R syntax.

Cloud technologies are constantly improving their capabilities, allowing to execute and analize data like we never seen before, for this reason the capability of integration between well know developing languages such as R and Python have become a strong desire for all Data engenieer and Data Scientist. The SAS Scripting Wrapper for Analytics Transfer (SWAT) package helps to satisfy this desire, functioning as a powerful client library that allows Python and R users to interface directly with the SAS Cloud Analytic Services (CAS) engine.

This integration works not only as a connector; it is a enhancer for data analysis, combining the ease of open-source syntax with the heavy-lifting capabilities of SAS Viya.

# What is SWAT?

SWAT is an API that enables a client-server workflow, allowing you to write native Python or R code on the client side to orchestrate analytics on a remote SAS Viya server, this is basically a translator, in escense it will take the  Python or R objects (like pandas DataFrames) and instructions and converts them into CAS actions, executes them on the distributed server, and returns the results back to your local environment. (This means we will we able to use the code we already know but using the capabilities of the SAS Server)

# Benefits of SAS SWAT
This integration opens the door to a complete new capabilities that can provide of great results for use 

1. No more limits

As mention before with SAS SWAT we will be able to work with the native Python and R, but the code will be execute with the SAS Server resources, this matters since both of them operate in-memory, ex. If we try to a 20GB dataset on a laptop with 16GB of RAM, the kernel will crash and we wont be able to process all the data and we will require of additional steps to complete the task.

If we use SWAT: The limit of memory that we canb access for the processing of the data is limited to the CAS server's memory, which is distributed across multiple nodes and will allows us to manipulate billions of rows not only from our dataset, but we will be able to also join this information to the same information we already have import to the SAS enviroment.

2. No need to learn new language or use complex sintax
   
Most of the Data scientists out there are familiar either with Python or R, with SAS SWAT they can continue working using this same languages without the need to become a SAS Programmer, this closese the gap and allow to more users to use this tool in the more convinient wat for them.

3. Production Pipeline Stability

If in your organization you decide to keep CAS as your central compute engine, SWAT allows you for the scripting of complex workflows, with this you can automate the data ingestion, transformation, and scoring pipelines entirely via script, avoiding the need for manual GUI interactions.

# Requirements
You must note that SWAT is new technology and it wont woork with SAS 9.4, it uses SAS Viya

Server Dependency: It requires access to a running SAS Viya / CAS server.
Version Compatibility: You generally need a client SWAT version that matches or is compatible with the server's CAS version.
Authentication: Requires valid credentials username/password, SAML, or other methods depending on your SAS deployment (LDAP, Kerberos, or Azure AD depending on setup).
