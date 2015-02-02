# fast-haas-recursive
Recursive HaaS with fast provisioning

## Outline

1. Discuss Vision - Discuss Properties (eg. Security needs, Functionality, Performance, scalability,etc.)

  Vision:
  To build a HaaS layer over Haas that uses the functionality of base HaaS to deploy its resources.
  
  To implement a solution that can
  
  1. Deploy customer OS images on physical nodes as fast as possible
  2. Reclaim, nodes from customers to free pool as fast as possible
  
    1. Reclaiming involves two steps, removing the customer OS from the nodes and
    2. Replacing it with a standard os/bios-like image without rebooting the nodes.

  As the final outcome, we would like to have a solution by which a customer can
    1. Seek physical servers from HaaS
    2. Install their own copy of HaaS on HaaS
    3. Provide HaaS service to her customers
    
2. Scope

  - In Scope:
    * Command Line Utilites
    * Construct RESTful APIs
    * Recursive API calls to HaaS (hypervisor)
    * Create Documentation
	
  - Out of Scope:
    * GUI
    * Scalability/upper bounds of the HaaS implementation
    * Security (recursive HaaS is equally secure as HaaS, and equally vulnerable)
    
3. Things to explore

  Recursive HaaS:
    Are there similar solutions out there?
    Has anyone else already accomplished something similar to this?
  
  Fast Provisioning:
  
    Has anyone done something similar to this? Examples, how was it accomplished?
    
    Was it efficient (fast enough)?  What is fast enough?
    
    What are different ways of pushing an image to several nodes?
    
    Which solutions suit our scenario? Why?
    
    What are the available solutions/tools to switch a system to new OS without rebooting?
    
    What are possible ways of avoiding to reboot a node to change its boot OS image?
    
4. Users/Personas/Roles of Project

  1. Users
    1. Security-conscious user
    2. High-performance-conscious user
    3. HaaS reseller
    4. Jason/Ian/EC500 professors
    5. Classmates
    6. Users not in scope of the project: ?
  2. Scrum Roles - first rotation, rotate every odd numbered sprint
    1. Product Owner - Sahil
    2. Scrum Master - Mike
    3. Team Members - Laura, Quentin
5. To-Do List
  * Install HaaS on bare metal
  * Explore socat utility
  * Explore kexec utility 
