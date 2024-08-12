# Lab 02 - Copilot for Data Science and Data Engineering (preview)

![Data Engineering](/images/dataengineering.svg)
![Data Science](/images/datascience.svg)
![Copilot](/images/copilot.svg)

## Introduction
> Copilot for Data Engineering and Data Science is an AI-enhanced toolset tailored to support data professionals in their workflow. It provides intelligent code completion, automates routine tasks, and supplies industry-standard code templates to facilitate building robust data pipelines and crafting complex analytical models. Utilizing advanced machine learning algorithms, Copilot offers contextual code suggestions that adapt to the specific task at hand, helping you code more effectively and with greater ease. From data preparation to insight generation, Microsoft Fabric Copilot acts as an interactive aide, lightening the load on engineers and scientists and expediting the journey from raw data to meaningful conclusions.[^1]

## Lab
This lab will create a Notebook in the Data Engineering experience and use Copilot to write code and interact with the data.

1. Go to the **Data Engineering** persona:

![Data Engineering persona](/labs/lab02/images/dataengineeringpersona.png)

2. Create a new Notebook by clicking the **Notebook** button:

![New Notebook](/labs/lab02/images/newnotebook.png)

Optionally change the name of the notebook to something meaningful using the gear icon in the top left-hand corner.

3. Attach the Lakehouse
- Attach the Lakehouse created in Setup by clicking on the **Lakehouses** > **Add Lakehouse** button.  Add the existing Lakehouse created in Setup.

4. Click the **Copilot** button and then the **Get Started** button on the right-hand side.

![Copilot Button](/labs/lab02/images/copilotbutton.png)

5. This will add some code to the notebook and display sample prompts in the Copilot pane on the right-hand side:

![Copilot Pane](/labs/lab02/images/copilotpane.png)

6. Run the cell Copilot has added which contains the following code:

```Python
#Run this cell to install the required packages for Copilot
%pip install https://aka.ms/chat_magics-0.0.0-py3-none-any.whl
%load_ext chat_magics
```

Use <kbd>Ctrl</kbd>+<kbd>Enter</kbd> to run an individual cell or <kbd>Shift</kbd>+<kbd>Enter</kbd> to run the cell and proceed to the next cell.  Alternately click the `Play` icon next to the cell to run it.  It can sometimes take a few minutes for this code to run.

When the code has completed it should display a screen like this with useful information on the chat magics it has enabled:

![Chat Magics](/labs/lab02/images/chatmagics.png)

> [!TIP]
> Chat magics are useful for interacting with Copilot in notebook cells.  You can still interact with Copilot using the Copilot pane and copy any suggestions into the notebook.

7. Review the output document from the cell which enabled the chat magics starting `Chat_magic commands`.
8. Try `%%chat` magic
- ask questions about your notebook state or let the chat-magics 
help you understand or author it  

- Enter the following in a code cell:
```
%%chat
Tell me about this lakehouse
```

9. Try `%%code` magic
- generates code to work with or visualise your data

- Enter the following in a code cell:
```
%%code
Get the data from ukpublicholidays into a dataframe
```

10. Try `%describe` magic
- describes a loaded dataframe

- Enter the following in a code cell:
```
%describe
df_ukpublicholidays
```

11. Try the `%%add_comments` magic
- add comments to the code in the cell

- Enter the following in a code cell:

```
%%add_comments
display(df_ukpublicholidays)
```

12. Try the `%%fix_errors` magic
- fix errors in a cell
13. Try the `%%translate` magic
- translate code from one language to another
- use the ? to get help on any chat magic

- Enter the following in a code cell:
- Correct the lakehouse name to your lakehouse name

```
%%translate?
df = spark.sql("SELECT * FROM lh_copilotlab.ukpublicholidays LIMIT 1000")
display(df)
```

- Enter the following in a code cell:
```
%%translate -lscala -fpython
df = spark.sql("SELECT * FROM lh_copilotlab.ukpublicholidays LIMIT 1000")
display(df)
```
This should output some Scala.  Add the `%%spark` magic to the cell and run it to test the new code.

![Spark Magic](/labs/lab02/images/sparkmagic.png)


## Recap
This lab used Copilot in the Data Engineering workflow to add powerful chat magics to work with data and code.

## Discussion
- Which version of gpt is Copilot using here?
- What's the difference between interacting using chat magics versus the Copilot pane?
- Was Copilot useful in this lab?
- What other prompts did you try?

## Next Steps
[Lab 03 - Copilot for Data Warehouse](/labs/lab03/lab03.md)

## Links
- https://learn.microsoft.com/en-us/fabric/get-started/copilot-notebooks-overview
- https://learn.microsoft.com/en-us/fabric/data-engineering/author-execute-notebook
- https://learn.microsoft.com/en-us/fabric/get-started/copilot-notebooks-chat-magics

[^1]: https://learn.microsoft.com/en-us/fabric/get-started/copilot-fabric-overview