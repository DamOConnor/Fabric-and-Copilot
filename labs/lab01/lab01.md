# Lab 01 - Copilot for Data Factory 

![Data Factory](/images/datafactory.svg)
![Copilot](/images/copilot.svg)

## Introduction
> Copilot for Data Factory is an AI-enhanced toolset that supports both citizen and professional data wranglers in streamlining their workflow. It provides intelligent code generation to transform data with ease and generates code explanations to help you better understand complex tasks.[^1]

## Lab
This lab will create a Dataflow Gen2 pipeline and use Copilot to add activities to the pipeline.

1. Click on the **Power BI** icon in the bottom left-hand corner.
2. Select **Data Factory**:

![Data Factory Persona](/labs/lab01/images/datafactorypersona.png)

3. You will be presented with the artefacts that can be created in the Data Factory persona including Dataflow Gen2 and Data Pipelines.
4. Select **Dataflow Gen2**:

![New Dataflow Gen2](/labs/lab01/images/newdataflowgen2.png)

5. This will take you into the main Dataflow Gen 2 design canvas.  Click the **Copilot** button:

![Dataflow Gen 2 Design Canvas](/labs/lab01/images/dfg2mainscreen.png)

6. Then click **Get Data**, select the recently created Lakehouse from the 'OneLake data hub' section, then select only the `publicholidays` table:

![Get Data](/labs/lab01/images/getdata.png)

- Ignore all the system queries
- Then click **Create**

7. Enter the following prompts:

```
Filter to only select data from United Kingdom
```

```
Filter from year 2000 onwards
```

- Inspect the code created by clicking the gear icon in the **Applied steps** section:

![Get Data](/labs/lab01/images/appliedsteps.png)


> [!IMPORTANT]
> If you receive the following error, enable the *Data Sent to Azure OpenAI can be processed outside your capacity's geographic region, compiance boundary or national cloud instance* option  in the Admin portal:  
> "You can't use Copilot in this workspace because its capacity is located ouside your tenant's region"


8. Enter the following prompt:

```
Save the data to a table called ukpublicholidays
```

- This step should fail.  Data destination cannot currently be added.

9. Manually add a data destination which is the current Lakehouse and a table called `ukpublicholidays`.

10. Click **Publish**.

11. Review the [Limitations of Copilot for Data Factory](https://learn.microsoft.com/en-us/fabric/get-started/copilot-fabric-data-factory#limitations-of-copilot-for-data-factory) article.

## Discussion
- Was Copilot useful in this lab?
- What other prompts did you try?
- What are the limitations of Copilot for Data Factory?

## Next Steps
[Lab 02 - Copilot for Data Science and Data Engineering](/labs/lab02/lab02.md)

## Links
- https://learn.microsoft.com/en-us/fabric/get-started/copilot-fabric-data-factory

[^1]: https://learn.microsoft.com/en-us/fabric/get-started/copilot-fabric-data-factory