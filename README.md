# Embed-PowerBI-in-Python
**In this repo I will show you how to embed your Power BI report in Python Jupyter Notebook**
The process of Embedding Microsoft Power BI in Python Jupyter Notebook is simple and easy to use.

## Requirement:
Basic knowledge of Microsoft Power BI, Power BI Service(Web), how to Publish from Power BI Desktop to web.

## Step 1: Pip install the Microsoft Power BI Client. This can be done either through cmd or directly on your Notebook.

```
!pip install powerbiclient
```

## Step 2: Import all necessary libraries

```
#import all necessary library
from powerbiclient import Report
```

## Step 3: Get Group ID & Report ID:
**NOTE:** The Group ID and Report ID can be gotten from your Power BI Service workspace URL

- Go to [PowerBI Service](https://www.powerbi.com).
- Login with all necessary credentials.
- Go to your WorkSpace where you have the Report published.
- Copy out the Group ID and Report ID.

The Image below will explain better on how to go about it.

![alt text](https://github.com/kiddojazz/Embed-PowerBI-in-Python/blob/master/Images/Embed-Python-to-PowerBI-Gif.gif)

## Step 4: Authentification of your device.
This section is where you will need to sign in to your Azure Cross Platform authentification.

- Run the code below then click on the link that appears below `https://microsoft.com/devicelogin`.
- After that is completed, you will need to copy the `code` provided.
- Login in to the appropraite account needed and follow each steps.

```
# Authenticate the device to embed
from powerbiclient.authentication import DeviceCodeLoginAuthentication
 
# Initiate device authentication
device_auth = DeviceCodeLoginAuthentication()
```

![alt text](https://github.com/kiddojazz/Embed-PowerBI-in-Python/blob/master/Images/Azure-Python-Embed.gif)

## Step 5: Generate your Power BI report
This is the last step in which you generate your Power BI report.

```
# Generate the report
report = Report(group_id=group_id, report_id=report_id, auth=device_auth)
report
```

#  Watch [YouTube](https://www.example.com) 


