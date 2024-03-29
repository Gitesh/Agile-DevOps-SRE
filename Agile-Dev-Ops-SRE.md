# How are Agile, DevOps, DevSecOps, GitOps, ChatOps, AIOps, FinOps, SRE related?

>### Practice
<pre>
 -------------                     -------------                   -------------  
| Business    |                   | Software    |                 | Platform    |  
| Change      | ----------------> | Engineering | --------------> | Engineering |  
 -------------                     -------------                   -------------  
</pre>


>### Objective 
<pre>
  ----------                         ----------                    --------------
 | Creating |                       | Building |                  | Maintaining  |
 | Customer |    ---------------->  | Digital  |  --------------> | Stable       |
 | Value    |                       | Products |                  | Environments |
  ----------                         ----------                    --------------
Respond to market                  Deliver change               Preserve reliability
  conditions                          quickly                   (resistant to change)
</pre>


>### Capability

<pre>
 ----------------                    -------------                    ------------
| Change (agile) | ---[backlog]---> | Build (dev) | ---[release]---> | Run (ops)  |   ; Where [] is the transition.
 ----------------                    -------------                    ------------

                                      <----------------SRE------------------------|   ; Ops led - mature Products with very little change to codebase
                                                                                                - focus is on NFRs:
                                                                                                     Reliability (security, performance, integrity)
                                                                                                     Availability (resilience, redundancy, recovery, repairability)
                                                                                                     Scalability (adaptive capacity)
                                      -----------------DevOps-------------------->    ; Dev led - in newer Products, change to codebase is constant
                                      ----------------DevSecOps------------------>    ; Security led - this is really DevComplianceOps
                                                                     |---GitOps---|   ; Version controlled infrastructure configuration - ephemeral, scalable,                                                                                                                                                   immutable, repeatable
                                                                     |----AIOps---|   ; Prevantative maintenance enabled by predictive failure and anomaly detection
              |-----------------------FinOps--------------------------------------|   ; forecasting, budgeting and tracking spend across the SDLC
                                                    |----ChatOps----|                 ; use of auditable collaboration tools to progress workflow requests
</pre>

### **Principles**
\
_**SRE:**_ platform engineering and software engineering are of equal value. Together they create a self balancing system that helps product teams to get features to market quickly, but not at the expense of reliability and integrity (see NFRs).  
\
_**Creating Customer Value is the ultimate measure of success:**_ If you can't track the value created then you don't know whether you made a difference:  
* Business agility is an outcome of engineering disciples embracing speed.  

* Smaller, reversible change supports stability AND agility. 

* Feedback + agility enables innovation.

\
_**Dev and Ops effort changes depending on where a Product is in its lifecycle:**_ newer products are Dev heavy by nature with little focus on Ops. For established Products with little ongoing change, the balance is reversed, a greater focus on Ops than Dev:

* New digital products/applications have a *high* frequency of change - there is more Development work, focus is on rapid change.

* Older digital products/applications have a *low* frequency of change - there is more Operations work to stabilise the environment, focus is on maintenance and uptime.

\
_**Non-functional requirements:**_ Operational reliability gives confidence in stability. Stability builds trust, trust attracts customers. A product owner is feature focused so will not ask for NFRs. Ops should define non-negotiable NFRs. 

* Quality - The quality of incoming work from previous stages affects the later stages. As DevOps is a feedback loop, quality eventually affects everything. Improving quality automatically improves productivity.  

* Reliability - measures whether a system is functioning correctly. This will require prioritisation of Ops work over features (SRE). Improving the quality of incoming code from 'Build' gives 'Run' reliability. This applies equally from 'Change' to 'Build'.

* Availability - individual components of a system may be available within the period measured (SLA), but it does not mean the system is functioning correctly.
* Repairability - reduces downtime. Complex systems are difficult to repair. Making SPoFs easy to repair improves availabilty. Use preventative maintenance.
* Scalability - automated, flexible and demand based resource use (CPU, Network, Storage).  


  
### **Notes**
SRE = Ops focused Development. You could call it OpsDev.

DevSecOps = Security gets the focus but really this is DevComplianceOps and applies to any standard you need to comply with.  

Capability = people (skills, tacit knowledge), process (methodologies, automated for codified knowledge), and technologies (optional vs standardised).  

Agile = is a framework - flexible, non prescriptive (ambiguous, no specific steps or process), room for creativity and customisation).  

Development = is a methodology (prescriptive, consistent, systematic way of doing something).

ChatOps = is a preventative control. It ensures changes are reviewed and approved by knowledgable person prior to progressing the workflow.

Tech Debt = addressing technical debt is a form of preventatitive maintenance.

Monitoring = is a reactive control if detection is post event occurrance; a preventative control if historical data is used to identfiy trends.

AIOps = data science and machine learning used to automate operational processes
