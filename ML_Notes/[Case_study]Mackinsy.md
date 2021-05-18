## Guides: 

* [An executive’s guide to AI](https://www.mckinsey.com/~/media/McKinsey/Business%20Functions/McKinsey%20Analytics/Our%20Insights/An%20executives%20guide%20to%20AI/An-executives-guide-to-AI.ashx)
* Building Machine Learning Powered Applications 
* Fundamentals of Machine Learning for Predictive Data Analytics Algorithms, Worked Examples, and Case Studies
* workera report: AI Career Pathways: Put Yourself on the Right Track



---




<img src="file:///Users/asjad/Documents/ML_Notes/images/ml_application_1.png?lastModify=1613717147" alt="ml_application_1" style="zoom:67%;" />

<img src="file:///Users/asjad/Documents/ML_Notes/images/ml_application_2.png?lastModify=1613717147" alt="ml_application_2" style="zoom:67%;" />

<img src="file:///Users/asjad/Documents/ML_Notes/images/ml_application_3.png?lastModify=1613717147" alt="ml_application_3" style="zoom:67%;" />

## Notes from: Fundamentals of Machine Learning for Predictive Data Analytics Algorithms, Worked Examples, and Case Studies



**Converting Business Problems into ML Solutions**

*It is not feasible for an analytics practitioner to learn everything about the businesses with which they work as they will probably move quickly between different areas of an organization, or even different industries. Analytics practitioners must, however, possess what is referred to as **situational fluency**. This means that they understand enough about a business so that they can converse with partners in the business in a way that these business partners understand. For example, in the insurance industry, insurance policy holders are usually referred to as members rather than customers. Although from an analytics perspective, there is really little difference, using the correct terminology makes it much easier for business partners to engage with the analytics project. Beyond knowing the correct terminology to use, an analytics practitioner who is situationally fluent will have sufficient knowledge of the quirks of a particular domain to be able to competently build analytics solutions for that domain.*



Consider the following business problem: in spite of having a fraud investigation team that investigates up to 30% of all claims made, a motor insurance company is still losing too much money due to fraudulent claims. The following predictive analytics solutions could be proposed to help address this business problem:



**[Claim prediction]** A model could be built to predict the likelihood that an insurance claim is fraudulent. This model could be used to assign every newly arising claim a fraud likelihood, and those that are most likely to be fraudulent could be flagged for investigation by the insurance company’s claims investigators. In this way the limited claims investigation time could be targeted at the claims that are most likely to be fraudulent, thereby increasing the number of fraudulent claims detected and reducing the amount of money lost to fraud.



**[Member prediction]** A model could be built to predict the propensity of a member1 to commit fraud in the near future. This model could be run every quarter to identify those members most likely to commit fraud, and the insurance company could take a risk mitigation action ranging from contacting the member with some kind of warning to canceling the member’s policies. By identifying members likely to make fraudulent claims before they make them, the company could save significant amounts of money.



**[Application prediction]** A model could be built to predict, at the point of application, the likelihood that a policy someone has applied for will ultimately result in a fraudulent claim. The company could run this model every time a new application is made and reject those applications that are predicted likely to result in a fraudulent claim. The company would therefore reduce the number of fraudulent claims and reduce the amount of money they would lose to these claims.



**[Payment prediction]** Many fraudulent insurance claims simply over-exaggerate the amount that should actually be paid out. In these cases the insurance company goes through an expensive investigation process but still must make a reduced payment in relation to a claim. A model could be built to predict the amount most likely to be paid out by an insurance company after having investigated a claim. This model could be run whenever new claims arise, and the policy holder could be offered the amount predicted by the model as settlement as an alternative to going through a claims investigation process. Using this model, the company could save on claims investigations and reduce the amount of money paid out on fraudulent claims.



**Question 1: Is the data required by the solution available, or could it be made available?**

****



The first question addresses data availability. Every analytics solution will have its own set of data requirements, and it is useful, as early as possible, to determine if the business has sufficient data available to meet these requirements. In some cases a lack of appropriate data will simply rule out proposed analytics solutions to a business problem.

	- **The key objects in the company’s data model and the data available regarding them.** 
	- **The connections that exist between key objects in the data model.** 
	- **The granularity of the data that the business has available.**
	- **The volume of data involved.**
	- **The time horizon for which data is available.**





**[Claim prediction]** *Data Requirements:* This solution would require that a large collection of historical claims marked as *fraudulent* and *non-fraudulent* exist. Similarly, the details of each claim, the related policy, and the related claimant would need to be available. *Capacity Requirements:* Given that the insurance company already has a claims investigation team, the main requirements would be that a mechanism could be put in place to inform claims investigators that some claims were prioritized above others. This would also require that information about claims become available in a suitably timely manner so that the claims investigation process would not be delayed by the model.

**[Member prediction]** *Data Requirements*: This solution would not only require that a large collection of claims labeled as either *fraudulent* or *non-fraudulent* exist with all relevant details, but also that all claims and policies can be connected to an identifiable member. It would also require that any changes to a policy are recorded and available historically. *Capacity Requirements:* This solution first assumes that it is possible to run a process every quarter that performs an analysis of the behavior of each customer. More challenging, there is the assumption that the company has the capacity to contact members based on this analysis and can design a way to discuss this issue with customers highlighted as likely to commit fraud without damaging the customer relationship so badly as to lose the customer. Finally, there are possibly legal restrictions associated with making this kind of contact.

**[Application prediction]** *Data Requirements:* Again, a historical collection of claims marked as *fraudulent* or *non-fraudulent* along with all relevant details would be required. It would also be necessary to be able to connect these claims back to the policies to which they belong and to the application details provided when the member first applied. It is likely that the data required for this solution would stretch back over many years as the time between making a policy application and making a claim could cover decades. *Capacity Requirements:* The challenge in this case would be to integrate the automated application assessment process into whatever application approval process currently exists within the company.

**[Payment prediction]** *Data Requirements:* This solution would require the full details of policies and claims as well as data on the original amount specified in a claim and the amount ultimately paid out. *Capacity Requirements:* Again, this solution assumes that the company has the potential to run this model in a timely fashion whenever new claims rise and also has the capacity to make offers to claimants. This assumes the existence of a customer contact center or something similar.



**Prediction Subject Details:** Descriptive details of any aspect of the prediction subject. **Demographics:** Demographic features of users or customers such as age, gender, occupation, and address.
 **Usage:** The *frequency* and *recency* with which customers or users have interacted with an organization. The *monetary value* of a customer’s interactions with a service. The *mix* of products or services offered by the organization that a customer or user has used.

**Changes in Usage:** Any changes in the frequency, recency, or monetary value of a customer’s or user’s interactions with an organization (for example, has a cable TV subscriber changed packages in recent months?).
 **Special Usage:** How often a user or customer used services that an organization considers special in some way in the recent past (for example, has a customer called a customer complaints department in the last month?).

**Lifecycle Phase:** The position of a customer or user in their lifecycle (for example, is a customer a new customer, a loyal customer or a lapsing customer?).
 **Network Links:** Links between an item and other related items (for example, links between different customers or different products, or social network links between customers).

The actual process for determining domain concepts is essentially one of **knowledge elicitation**—attempting to extract from domain experts the knowledge about the scenario we are trying to model. Often, this process will take place across multiple meetings, involving the analytics and domain experts, where the set of relevant domain concepts for the analytics solution are developed and refined.



At this point in the motor insurance fraud detection project, we have decided to proceed with the proposed **claim prediction** solution, in which a model will be built that can predict the likelihood that an insurance claim is fraudulent. This system will examine new claims as they arise and flag for further investigation those that look like they might be fraud risks. In this instance the prediction subject is an insurance claim, and so the ABT for this problem will contain details of historical claims described by a set of descriptive features that capture likely indicators of fraud, and a target feature indicating whether a claim was ultimately considered fraudulent. The domain concepts in this instance will be concepts from within the insurance domain that are likely to be important in determining

whether a claim is fraudulent. Figure 2.3[31] shows some domain concepts that are likely to be useful in this case. This set of domain concepts would have been determined through consultations between the analytics practitioner and domain experts within the business.



**Question: what are some of the useful features that can be designed and implemented to solve this problem** 

Once domain concepts have been agreed on, the next task is to design and implement concrete features based on these concepts. A feature is any measure derived from a domain concept that can be directly included in an ABT for use by a machine learning algorithm. Implementing features is often a process of approximation through which we attempt to express as much of each domain concept as possible from the data sources that are available to us. Often it will take multiple features to express a domain concept. Also, we may have to use some **proxy features** to capture something that is closely related to a domain concept when direct measurement is not possible. In some extreme cases we may have to abandon a domain concept completely if the data required to express it isn’t available. Consequently, understanding and exploring the data sources related to each domain concept that are available within an organization is a fundamental component of feature design. Although all the factors relating to data that were considered during the

feasibility assessment of the analytics solution2 are still relevant, three key data considerations are particularly important when we are designing features.



---

**Question 2: What is the quality of the dataset** - We engage in EDA 



The basis of data exploration is statistics. 

1. Have *gotten to know* the features within the ABT, especially their central tendencies, variations, and **distributions**.

2. Have identified any **data quality issues** within the ABT, in particular **missing values**, **irregular cardinality**, and **outliers**.

3. Havecorrectedanydataqualityissuesdueto**invaliddata**.

4. Have recorded any data quality issues due to **valid data** in a **data quality plan** along

   with potential handling strategies.

5. Beconfidentthatenoughgoodqualitydataexiststocontinuewithaproject.



---

**Question3: What is the right modeling algorithm** 



The model with right with right expressivity - that balances bias and variance nicely. 



No free lunch theorem: 





Cheatsheet for selecting a model



Examples: 





---

**Quesiton 4: The right evaluation approach**



* *The choice of the correct performance measure for a particular problem depends on a combination of the nature of the prediction problem (e.g., continuous versus categorical), the characteristics of the dataset (e.g., balanced versus imbalanced), and the needs of the application (e.g., medical diagnosis versus marketing response prediction).*

* Cross validation approaches are generally preferred unless datasets are very large, in which case the likelihood of the **lucky split** becomes very low, and hold-out approaches can be used. 

* As with everything else, there is an application-specific component to the selection of an experimental design

