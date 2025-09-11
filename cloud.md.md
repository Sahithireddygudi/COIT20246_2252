**Cloud Services**

We investigated the costs of hosting Truelec's servers using Microsoft
Azure and Amazon AWS. The official cloud pricing calculators were used,
and the exported estimates are provided in our repository for
verification:

-   AzureEstimate.xlsx

-   AWSEstimate.csv

VM Specifications (per server)

-   Region: Australia East (Azure) / Asia Pacific (Sydney) AWS

-   Operating System: Windows Server 2022

-   vCPUs: 4

-   RAM: 16 GB

-   Storage: 256 GB SSD

Cost Comparison

  -----------------------------------------------------------------------------------
  Provider    VM Specs    Monthly     12-Month     5-Year Total  Estimate File
              (Sydney     Cost        Cost                       
              Region)                                            
  ----------- ----------- ----------- ------------ ------------- --------------------
  Azure       4 vCPUs, 16 \$392.79    \$4,713.50   \$23,567.52   AzureEstimate.xlsx
              GB RAM, 256                                        
              GB Premium                                         
              SSD                                                

  AWS         4 vCPUs, 16 \$327.01    \$3,924.12   \$19,620.60   AWSEstimate.csv
              GB RAM, 256                                        
              GB gp2 SSD                                         
              (EBS)                                              
  -----------------------------------------------------------------------------------

Note: Values are in USD. Each cost is for one VM. Truelec requires 6
servers, so totals would be 6× these values.

Analysis

-   Azure Advantages: Tighter integration with Microsoft ecosystem (AD,
    Office 365, licensing). Easier for existing Windows workloads.

-   AWS Advantages: Slightly lower costs, flexible services, broader
    global network.

-   Disadvantages of Cloud: Recurring operational costs, vendor lock-in,
    dependency on internet availability.

Recommendation

While AWS offers lower costs (\~17% cheaper), we recommend Microsoft
Azure for Truelec. The integration with Microsoft services, licensing
compatibility, and simplified administration outweigh the modest cost
difference.
