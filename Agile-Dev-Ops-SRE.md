# How are Agile, DevOps, DevSecOps, GitOps, SRE related?

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
Respond to market                  Deliver change               Preserve availability
  conditions                         quickly                    (resistant to change)
</pre>

>### Framework

<pre>
 ----------------                    -------------                    ------------
| Change (agile) | ---[backlog]---> | Build (dev) | ---[release]---> | Run (ops)  |  ; Where [] is the transition.
 ----------------                    -------------                    ------------

                                     \<----------------SRE-----------------------/   ; Ops led - mature Products with very little change to codebase
                                                                                               - focus is on NFRs:
                                                                                                     Reliability (security, performance, integrity)
                                                                                                     Availability (resilience, redundancy, recovery)
                                                                                                     Scalability (adaptive capacity)
                                       \-------------DevOps--------------->/         ; Dev led - in newer Products, change to codebase is constant
                                        \----------DevSecOps------------->/          ; Security led - this is really DevComplianceOps
                                                                      \--GitOps--/   ; Infrastructure configuration - ephemeral, scalable, immutable,
                                                                                                                      repeatable
</pre>

### **Principles**
_**SRE:**_ systems engineering and software engineering are of equal value.  
_**Creating Customer Value:**_ is the ultimate measure of success. If you can't track the value created then you don't know whether you made a difference.  
_**Dev and Ops effort changes depending on where a Product is in its lifecycle:**_ newer products are Dev heavy by nature with little focus on Ops. For established Products with little ongoing change, the balance is reversed, a greater focus on Ops than Dev:

* New digital products/applications have a *high* frequency of change - there is more Development work, focus is on rapid change.
* Older digital products/applications have a *low* frequency of change - there is more Operations work to stabilise the environment, focus is on maintenance and uptime.


### Notes
SRE = Ops focused Development. Maybe we should call it OpsDev?  
DevSecOps = Security gets the focus but really this is DevComplianceOps and applies to any standard you need to comply with.
