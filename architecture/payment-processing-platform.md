## Introduction

Design a data-intensive system capable of facilitating high-volumepayment processing transactions. You are responsible for designing a scalable, client-agnostic, fault-tolerant system that facilitates interactions over HTTP and any other mode of interaction you believe is justifiable based upon your experience as an Engineer. Your solution should detail the surface layer system consumers will interact with. You are not responsible for designing a client. 

The intent of this challenge is to determine how you think about clarity in design, your aptitude for selecting the tooling best suited for addressing the below-outlined requirements, and communication. 

## Deliverables

## Interview Format

You will be given 15 minutes to present your design _and_ facilitate questions while presenting. 15 additional mimnutes will be dedicate to facilitating feedback on your design.

### Guiding Question(s)

- What considerations did you make when designing your solution?
- What potential risks does your design try to mitigate?
- How did you ensure your design was easily understood by someone unfamiliar with the solution?
- Why did you select any one of the cloud-based services you selected?
- How simple would it be to add functionality to your design? Would the added functionality introduce unwanted complexit? Would a person adding functionality easily infer how the system should be extended?
- What happens when the system experiences unexpected volume?

## Functional Requirement(s)

1. The system will allow for a consumer to register themselves as a **service provider**.  
&nbsp; 1.1. The system will allow each service provider to register a **reimbursement** cadence.    
&nbsp; &nbsp; &nbsp; &nbsp; 1.1.1. The reimbursement cadence can be at the granularity of daily, weekly, monthly, or yearly.  
1.2. The systel will allow each service provider to 
- The system will enable those service providers to submit a record of activity for `n` number of **members**.
- 



## Criteria For Success

Each of the below criteria should be explicitly and thoughtfully addressed.

- [ ] The system is descriptive of its intent.
- [ ] The system adheres to convention.
- [ ] The system handles functional fault.
- [ ] The system handles infrastructural failure.
- [ ] The system handles increased load.
- [ ] The system handles decreased load.
- [ ] The system makes clear decisions to optimize for efficiency.

## Criteria For Failure

Areas of weakness in a solution are:

- [ ] The inability to describe the motivation or reasoning behind a particular system component.  
