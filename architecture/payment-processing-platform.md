# Motility Reimbursement Cycle Management System

## Introduction

You will design a small subset of a larger system (defined in **Functional Requirements**, below). The _larger_ system is a high-volume, data-intensive revenue management system. 

### Scenario 

_Domain terms are in bold_.

Clients (**service providers**) pay a fee to Motility. In exchange, service providers allow their **members** (customers) to access Motility's locations. Motility locations host a widget exchange, where highly desireable widgets are traded, risk free, between members. Every time a member visits a Motility location, Motility pays the assocaited service provider a small reward (**reimbursement**), funded.

You will design the reimbursement component. 

You are responsible for designing a scalable, fault-tolerant system that facilitates interactions over HTTP and any other mode of interaction you believe is justifiable based upon your experience as an Engineer. In addition, your solution should detail the surface layer that system consumers will interact with. You are not responsible for designing the client. 

The intent of this challenge is to determine how you think about clarity in design, your aptitude for selecting the tooling best suited for addressing the below-outlined requirements, and communication. 

## Functional Requirements

These _Functional Requirements_ may not be complete; there may be gaps. Where there are gaps, please feel empowered to make assumptions about system behavior - as long as those assumptions are clearly communicated.

**1.** The system will allow for a consumer to register themselves as a **service provider**.  
&nbsp; &nbsp; **1.1.** The system will allow each service provider to register for a **reimbursement** cycle cadence.    
&nbsp; &nbsp; &nbsp; &nbsp; **1.1.1.** The system will enable a service provider to register for a reimbursement cadence as one of: daily, weekly, monthly, or yearly.  
&nbsp; &nbsp; **1.2.** The system will enable each service provider to submit a list of `n` number of recognized service provider **members**.  
&nbsp; &nbsp; &nbsp; &nbsp; **1.2.1.** The system will enable service providers to _update_ the recognized members associated with the service provider.  
&nbsp; &nbsp; &nbsp; &nbsp; **1.2.2.** The system will enable service providers to _remove_ members from the the recognized members associated with the service provider.    
&nbsp; &nbsp; &nbsp; &nbsp; **1.2.3.** The system will enable the service provider to _update_ or _remove_ the recognized members associated with the service provider at any point in time.   
&nbsp; &nbsp; **1.3.** The system will enable each service provider to submit a record of reimbursable **activity**.  
&nbsp; &nbsp; &nbsp; &nbsp; **1.3.1** The system will only recognize activity associated with recognized members associated with the service provider submitting the activity.    
&nbsp; &nbsp; &nbsp; &nbsp; **1.3.2** The system will enable a service provider to submit a record of activity for `n` number of **members**.    
&nbsp; &nbsp; &nbsp; &nbsp; **1.3.3** The system will allow a service provider to update the activity record for any member.    
&nbsp; &nbsp; &nbsp; &nbsp; **1.3.4** The system will allow a service provider to update the activity record for any member at any point in time.    
**2.** The system will **reimburse** service providers for the activity submitted on behalf of recognized members associated with the service provider.    
&nbsp; &nbsp; **2.1.** The system will reimburse service providers for the submitted member activity on the pre-registered reimbursement cadence.    
&nbsp; &nbsp; **2.2.** The system will only reimburse service providers for activity associated with recognized members.    
&nbsp; &nbsp; **2.3.** The system will reimburse service providers for a contractually agreed-upon percentage of the total value of the activity. 
**3.** The system will allow service providers to query the status of a given reimbursement cycle.

## Deliverables

Prepare an architectural diagram of your system. The system should be cloud-hosted and your design demonstrate your knowledge of fundamental cloud-hosted principles. 

Please spend no longer than two hours designing your system. This time should be spent conceptualizing the system, considering the various guidances below, and diagramming your solution. Incomplete solutions are acceptable; however, diagrammed components of the system should demonstrate rigor and completeness of thought. 

### Important Note Regarding Solution Scope

It is more important to isolate and design a well-behaved component of the system than it is to diagram the whole system defined by the **Functional Requirements** section above. We understand that this problem could evolve into a complex system with a tremendous number of considerations to demostrate. Focus on showing us your best, regardless of scope isolation choices. Your assessment will be evaluated on quality and depth, not breadth of scope.

### Guiding Question(s)

- What considerations did you make when designing your solution?
- What potential risks does your design try to mitigate?
- How did you ensure your design was easily understood by someone unfamiliar with the solution?
- Why did you select any one of the cloud-based services you selected?
- How simple would it be to add functionality to your design? Would the added functionality introduce unwanted complexity? Would a person adding functionality easily infer how the system should be extended?
- What happens when the system experiences unexpected volume?

### Principles To Consider

### Criteria For Success

Each of the below criteria should be explicitly and thoughtfully addressed.

- [ ] The system is descriptive of its intent.
- [ ] The system adheres to convention.
- [ ] The system handles functional fault.
- [ ] The system handles infrastructural failure.
- [ ] The system handles increased load.
- [ ] The system handles decreased load.
- [ ] The system makes clear decisions to optimize for efficiency.

### Criteria For Failure

Areas of weakness in a solution include:

- [ ] The inability to describe the motivation or reasoning behind a particular system component.
- [ ] Incompleteness in thought.


## Interview Format

You will be given 15 minutes to present your design _and_ facilitate questions while presenting. 15 minutes will then be dedicated to facilitating feedback on your design.
