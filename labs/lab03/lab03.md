# Lab 03 - Copilot for Data Warehouse (preview)

![Data Warehouse](/images/datawarehouse.svg)
![Copilot](/images/copilot.svg)

## Introduction
> Microsoft Copilot for Synapse Data Warehouse is an AI assistant designed to streamline your data warehousing tasks. Copilot integrates seamlessly with your Fabric warehouse, providing intelligent insights to help you along each step of the way in your T-SQL explorations.[^1]

> [!NOTE]
> Run this lab in MSIT.  Copilot for Data Warehouse does not appear to be enabled in External Azure subscriptions just yet.

## Lab
This lab will use Copilot to interact with the Data Warehouse persona to explain, write and fix T-SQL.

1. Go to the **Data Warehouse** persona:

![Data Warehouse persona](/labs/lab03/images/datawarehousepersona.png)

2. This will display the list of artefacts available in the Data Warehouse persona:

![Data Warehouse artefacts](/labs/lab03/images/datawarehouseartefacts.png)

3. Click **Warehouse** to create a new Data Warehouse.  Give it a unique name.

4. Click **Sample data** to load sample data into the warehouse:

![Sample Data](/labs/lab03/images/sampledata.png)

This can take a few minutes to run.  When the sample data is loaded it will look like this:

![Loaded Sample Data](/labs/lab03/images/loadedsampledata.png)

5. Click the **Copilot** button.

![Copilot button](/labs/lab03/images/copilotbutton.png)

Now use Copilot to interact with the sample data.  Enter the following prompts:

6. Start writing T-SQL
- Enter the following prompt:
```
What can I do in the Fabric Query editor?
```
7. Create a table
- Enter the following prompt:
```
Create a table to hold weather data (date, zip, temperature, and rainfall).
```
8. Ask a question
- Enter the following prompt:
```
Suggest questions that I can ask about this warehouse.
```

9. Tidy up - delete the data warehouse if you created it in MSIT.

## Discussion
- Was Copilot useful in this lab?
- What other prompts did you try?

## Next Steps
~~[Lab 04 - Copilot for Real-Time Intelligence](/labs/lab04/lab04.md)~~

## Links
- https://learn.microsoft.com/en-us/fabric/data-warehouse/copilot
- https://learn.microsoft.com/en-us/fabric/data-warehouse/copilot-quick-action

[^1]: https://learn.microsoft.com/en-us/fabric/data-warehouse/copilot