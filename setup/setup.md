# Setup
Complete setup actions for the labs in this section.

1. [Create a Fabric workspace](#1-create-a-fabric-workspace)
2. [Create a Lakehouse](#2-create-a-lakehouse)
3. [Load Sample Data](#3-load-sample-data)
4. [Check the data has been imported correctly](#4-check-the-data-has-been-imported-correctly)
5. [Proceed to Lab 01](#5-proceed-to-lab-01)

## 1. Create a Fabric workspace
- Go to https://app.fabric.microsoft.com/ in your external subscription
  - if this is your first time using Fabric you may have to sign in using your external subscription admin email
  - if this is **not** your first time signing into Fabric you might see the Power BI icon instead
- Click on the **Microsoft Fabric** icon in the bottom left-hand corner, then click **Power BI**:

![Fabric Home](/images/fabrichome.png)

- Click on **Workspaces** and then **New workspace**:

![New workspace](/images/newworkspace.png)
- Give the workspace a unique name
- Ensure the workspace is connected to the F64 (or above) Fabric Capacity:
  - Click **Advanced**, then **Fabric capacity**:

![Fabric Capacity](/images/fabriccapacity.png)

- Select your capacity from the dropdown
- Click **Apply** to create the workspace

> [!NOTE]
> If the **Fabric capacity** is grayed out, your F64 capacity may be paused, or you may not have access to it.  Check your capacity status and refresh the browser window if required


## 2. Create a Lakehouse
- Go to the **Data Engineering** persona:

![Data Engineering persona](/setup/images/dataengineeringpersona.png)

- Create a new Lakehouse for the lab by clicking on the large **Lakehouse** button in the 'Recommended items to create' section:

![Lakehouse Button](/setup/images/lakehousebutton.png)

- Give it a unique name.  Do **not** enable the **Lakehouse schemas (Public Preview)** option at this point:

![Data Engineering persona](/setup/images/newlakehouse.png)

- Click **Create** to create the Lakehouse in the current workspace

## 3. Load sample data
- Click **Start with sample data** to add sample data to the Lakehouse

![Sample Data](/setup/images/sampledata.png)

This can take a few minutes to run.  When the data has finished loading it should look like this:

![Sample Data Loaded](/setup/images/sampledataloaded.png)

## 4. Check the data has been imported correctly
- Inspect the tables by clicking on them, eg `publicholidays`

## 5. Proceed to Lab 01

## Next Steps
[Lab 01 - Copilot for Data Factory](/labs/lab01/lab01.md)


## Links
- [Create a workspace](https://learn.microsoft.com/en-us/fabric/get-started/create-workspaces)