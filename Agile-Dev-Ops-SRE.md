# How are Agile, DevOps, DevSecOps, GitOps, SRE related?

<pre>
 -------------                     -------------                   -------------  
| Business    |                   | Software    |                 | Platform    |  
| Change      | ----------------> | Engineering | --------------> | Engineering |  
 -------------                     -------------                   -------------  
</pre>

<pre>
  ----------                         ----------                     --------------
 | Creating |                       | Building |                   | Maintaining  |
 | Customer |    ---------------->  | Digital  |  ---------------> | Stable       |
 | Value    |                       | Products |                   | Environments |
  ----------                         ----------                     --------------
Respond to market                   Deliver change               Preserve availability
  conditions                          quickly                    (resistant to change)
</pre>

<pre>
 --------------                    -------------                    ------------
| Plan (agile) | ---[backlog]---> | Build (dev) | ---[release]---> | Run (ops)  |  ; Where [] is the transition.
 --------------                    -------------                    ------------

                                   \<----------------SRE-----------------------/   ; Ops led - mature Products with little change
                                                                                             - focus is on NFRs:
                                                                                                   Reliablity (security, performance, integrity)
                                                                                                   Availablity (resilience, redudancy, recovery)
                                                                                                   Scalability (adaprive capacity)
                                     \-------------DevOps--------------->/         ; Dev led - new Products, focus is on change
                                      \----------DevSecOps------------->/          ; Security led - security sells, this is really DevComplianceOps
                                                                    \--GitOps--/   ; Infrastructure configuration - ephermal, scaleable, immutable,
                                                                                                                    repeatable
</pre>
SRE = Ops focused Development. Maybe we should call it OpsDev? (*joke)  
DevSecOps = Security gets the focus but really this is DevComplianceOps and applies to any standard you need to comply with.

As a product matures the balance between Dev and Ops changes.Newer products are Dev heavy by nature with little focus on Operaions. For more established products with little change it is reversed - a greater focus on Ops than Dev.  
  *New digital products / applications - there is more Dev, focus on rapid change  
  *Older digital products / applications - there is more Ops, focus on maintenance and uptime  

##Principles

SRE - systems engineer and software engineering are of equal value.  
Customer Value - is the ultimate measure, if you can't track this then you don't know.
Cost layer.
