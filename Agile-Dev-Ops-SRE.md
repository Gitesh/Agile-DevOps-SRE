# How are Agile, DevOps, DevSecOps, GitOps, SRE related?



  -------------                     -------------                   -------------
 | Business    |                   | Software    |                 | Platform    |
 | Change      | ----------------> | Engineering | --------------> | Engineering |
  -------------                     -------------                   -------------

  ----------                        ----------                      --------------
 | Creating |                      | Building |                    | Maintaining  |
 | Customer |    ----------------> | Digital  |   ---------------> | Stable       |
 | Value    |                      | Products |                    | Environments |
  ----------                        ----------                      --------------
Responds to market            Delivers change quickly          Preserves availability(resist change?)
conditions

 --------------                    -------------                    ------------
| Plan (agile) | ---[backlog]---> | Build (dev) | ---[release]---> | Run (ops)  |  ; Where [ ] is the transition.
 --------------                    -------------                    ------------

                                   \<----------------SRE-----------------------/   ; Ops led - mature Products with little change
                                                                                    - focus is on NFRs:
                                                                                                   Reliablity (security, performance, integrity)
                                                                                                   Availablity (resilience, redudancy, recovery)
                                                                                                   Scalability (responsive capacity)
                                   \-------------DevOps--------------->/         ; Dev led - new Products, focus is on change
                                      \----------DevSecOps------------->/          ; Security led - security sells, this is really DevComplianceOps
                                                                    \--GitOps--/   ; Infrastructure configuration - ephermal, scaleable, immutable


SRE=Ops focused Development. How about we call it OpsDev? (*joke)
DevSecOps = Security gets the focus but really this is DevComplianceOps and applies to any standard you need to comply with.

New applications - there is more Dev
Old applications - there is more Ops

As a product matures the balance between Dev and Ops changes a digital product matures.
Newer products are Dev heavy by nature with little focus on Operaions. For more established products with little change it is reversed - a greater focus on Ops than Dev.

------------

**Principles
-------------

SRE - systems engineer and software engineering are of equal value.
Customer Value - is the ultimate measure, if you can't track this then you don't know.
Cost layer.
