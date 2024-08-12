# Prerequisites

![Microsoft Azure](/images/azure.svg)
![Microsoft Fabric](/images/fabric.svg)

These are the prerequisites for this lab:
- External Azure Subscription
  - **NB** Fabric does **not** currently work in Microsoft Non-prod / fdpo subscriptions
- Microsoft Fabric Capacity
  - see [this repo](https://github.com/DamOConnor/Fabric-IaC) if you do not already have a Fabric Capacity deployed
  - scaled to **F64**[^1]
- budget to spend **~£130** for half-day Fabric F64 consumption
- [Enable Copilot in Fabric](https://learn.microsoft.com/en-us/fabric/get-started/copilot-enable-fabric) if required

> [!IMPORTANT] 
> Check [Fabric region availability](https://learn.microsoft.com/en-us/fabric/admin/region-availability).  Enable the *Data sent to Azure OpenAI can be processed outside your capacity's geographic region...* if required:

- ![Geographic Processing](/prerequisites/images/geographicprocessing.png)

- ~~[Enable Git integration for Fabric workspaces](https://learn.microsoft.com/en-us/fabric/cicd/git-integration/git-get-started?tabs=azure-devops%2CAzure%2Ccommit-to-git): From Fabric Homepage > Settings > Admin portal~~

> [!TIP]
> Use [Microsoft Edge Profiles](https://www.microsoft.com/en-us/edge/learning-center/how-to-add-new-profiles?msockid=20f67ee92a346c49015f6f1a2e346a21&form=MA13I2) to manage external Azure subscriptions[^2]

## Copilot integration
![Copilot Integration](/images/copilotintegration.png)

## Discussion
- Which persona or workload is missing here and why?

## Next Steps
[Setup](/setup/setup.md)

## Links
- [Fabric IaC Repo](https://github.com/DamOConnor/Fabric-IaC)
- [Sign in and create multiple profiles in Microsoft Edge](https://support.microsoft.com/en-us/topic/sign-in-and-create-multiple-profiles-in-microsoft-edge-df94e622-2061-49ae-ad1d-6f0e43ce6435)



[^1]: [Copilot for Microsoft Fabric and Power BI: FAQ](https://learn.microsoft.com/en-us/fabric/get-started/copilot-faq-fabric)

[^2]:  Consider switching off Automated Profile Switching for that profile only.  
Settings > Profile preferences > Automatic profile switching > (disable all options)
