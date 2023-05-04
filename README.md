# application-resource-manager


## Turbonomics Overview
 ARM tool to assure the performance of the application by making sure that they continually in real-time get all the resources they need to perform throught analytics and automation, and gradually lower the cost of infrastructure.

 - Better Performance
 - Lower cost
 - Increased Compliance

![Turbonomics](/assets/turbonomics.jpg?raw=true)


# Use Cases

## [Cloud Migration Plan](https://www.ibm.com/docs/en/tarm/8.8.6?topic=types-migrate-cloud-plan)

A Migrate to Cloud plan simulates migration of on-prem VMs to the cloud, or migration of VMs from one cloud provider to another. This plan focuses on optimizing performance and costs by choosing the most suitable cloud resources for your VMs and the volumes they use. To further optimize your costs, the plan can recommend moving workloads from on-demand to discounted pricing, and purchasing more discounts.

The plan results show :
- Projected costs
- Actions to execute your migration and optimize costs and performance
- Optimal cloud instances to use, combining efficient purchase of resources with assured application performance
- The cost benefit of moving workloads from on-demand to discounted pricing
- Discounts you should purchase

Turbonomic shows results for two migration scenarios :

- **Lift & Shift :** Lift & Shift migrates your VMs to cloud instances that match their current resource allocations.

- **Optimized :** As Turbonomic runs the plan, it looks for opportunities to optimize cost and performance. For example, it might discover overprovisioned VMs after analyzing the historical utilization of VM resources. If you were to migrate such VMs to instances that match their current allocations, then you would spend more than necessary. For an optimized migration, Turbonomic can recommend migrating to less expensive instances while still assuring performance, and then show the resulting savings. In addition, when you examine the actions for an optimized migration, you will see charts that plot the historical utilization data used in the analysis.



## [Business Unit](https://www.ibm.com/docs/en/tarm/8.8.6?topic=endpoints-businessunits-endpoint)

Business units may be one of three types, described below :

- BUDGET : A business unit that has a budget, and may contain children.

- DISCOUNT : A business unit that has a discount, and may contain children.

- DISCOVERED : A business unit that has been discovered by the Turbonomic instance. These business units should not be edited or deleted, except on the discovered target. 


Business Unit API for Cost purpose :

- Getting Cloud Service and Pricing Model Pairs for a Specified Business Unit :
    
    **/cloudservices**


- For Getting Price Adjustments Related to a Specified Business Unit : 
    
    **/priceadjustments**



## [Automation Policies](https://www.ibm.com/docs/en/tarm/8.8.0?topic=policies-automation)

Turbonomic uses Automation Policies to guide its analysis and resulting actions. These policies can specify :

- **Action Automation :** Whether to execute automatically or manually, or whether to just recommend the action.
- **Action Scripts :** Whether to have Turbonomic execute the action, or execute the action with Action Scripts.
- **Action Orchestration :** Whether to have Turbonomic execute the action, have Turbonomic direct an orchestrator to execute the action, or execute the action with Action Scripts.
- **Constraints and Other Settings :** Settings that affect the Turbonomic analysis of the state of your environment. These include operational, utilization, and scaling constraints.

