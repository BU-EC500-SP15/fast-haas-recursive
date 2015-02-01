# fast-haas-recursive
Recursive HaaS with fast provisioning

** Outline

1. Discuss Vision - Discuss Properties (eg. Security needs, Functionality, Performance, scalability,etc.)
  Vision:
  To build a HaaS layer over Haas that uses the functionality of base HaaS to deploy its resources.
  To implement a solution that can
  1. Deploy customer OS images on physical nodes as fast as possible
  2. Reclaim, nodes from customers to free pool as fast as possible
    a. Reclaiming involves two steps, removing the customer OS from the nodes and
    b. Replacing it with a standard os/bios-like image without rebooting the nodes.
  As the final outcome, we would like to have a solution by which a customer can
    a. Seek physical servers from HaaS
    b. Install their own copy of HaaS on HaaS
    c. Provide HaaS service to her customers

2. Scope
  In Scope:
    Command Line Utilites
    Construct RESTful APIs
	Recursive API calls to HaaS (hypervisor)
	Create Documentation
  Out of Scope:
    GUI
    Scalability/upper bounds of the HaaS implementation
    Security (recursive HaaS is equally secure as HaaS, and equally vulnerable)

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
  A. Users
    a. Security-conscious user
    b. High-performance-conscious user
    c. HaaS reseller
    d. Jason/Ian/EC500 professors
    e. Classmates
    f. Users not in scope of the project: ?
  B. Scrum Roles - first rotation, rotate every odd numbered sprint
    a. Product Owner - Sahil
    b. Scrum Master - Mike
    c. Team Members - Laura, Quentin

 5. To-Do List
   - Install HaaS on bare metal
   - Explore socat utility
   - Explore kexec utility 