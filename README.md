# Embed-PowerBI-in-Python
**In this repo I will show you how to embed your Power BI report in Python Jupyter Notebook**
The process of Embedding Microsoft Power BI in Python Jupyter Notebook is simple and easy to use.

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

![alt text](https://drive.google.com/uc?id=1Sxz6WKLSCiTl8nxny82Eba0GwITVI0mm)
