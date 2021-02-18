## This is the blog of Types of Machines in the CIS4330-Microservices class
### After reading the “Types of Machines” in the provided pdf, the following is my brief summary:

**What the advantages of Virtual Machines are?**
- They can make computing more efficient. Sharing a large physical machine’s power among many smaller virtual machines helps reduce stranded capacity by permitting the creation of virtual machines that are the right size for their requirements.
- They are fast to create and destroy. There is very little lead time between when one is requested and when the virtual machine is usable. Some systems can spin up a new virtual machine in less than a minute. Some systems create hundreds of ephemeral machines across many physical machines, run a parallel compute job, and then destroy the machines when the job is complete.
- They are controlled through software, so virtualization systems are programmable. An API can be used to create, start, stop, modify, and destroy them. Software can be written to orchestrate these functions on a large scale. This is not possible with physical machines, which have to be racked, cabled, and configured via manual labor.
- A virtual machine can detect CPU contention. 

**What the advantages of containers are?**
- They are very lightweight because they do not require an entire OS. Only the specific system files needed by the software are copied into the container. Each container has its own copy of the packages, shared libraries, and other supporting files that it requires. 
- They are usually the underlying technology in PaaS. They consume the exact amount of resources they need at the time, so they are much more efficient means of providing such shared services.
- Being self-contained, they eliminate dependencies and conflicts. 

**When you might select physical machines over virtual machines?**
- As for the performance factor, if organizations work with a large amount of data which needs to be constantly processed, and organizations running services and operations which require highly productive computing hardware for their implementation, Physical servers are far more powerful and efficient than VMs, due to the fact that VMs are prone to performance issues as a result of an overflow of virtual servers in a physical machine. 

### After researching more on the internet, the following is how cloud would aid microservices:

According to the article microsevices from ibm (https://www.ibm.com/cloud/learn/microservices), “individual containers don’t have the overhead of their own operating system, they are smaller and lighter weight than traditional virtual machines and can spin up and down more quickly, making them a perfect match for the smaller and lighter weight services found within microservices architectures”. Docker is a potential candidate. Docker is a set of platform as a service (PaaS) products that use OS-level virtualization to deliver software in packages called containers.  In addition, according to the introduction from amazon web service (https://aws.amazon.com/docker/) “running Docker on AWS provides developers and admins a highly reliable, low-cost way to build, ship, and run distributed applications at any scale.”

Microservices are not necessarily exclusively relevant to cloud computing; however, they frequently go together when microservices is being a popular architectural style for new applications, and the cloud is being a popular hosting destination for new applications.

With microservices, each individual component can adopt the stack best suited to its specific job. Stack proliferation can lead to serious complexity and overhead when we manage it by ourselves; however, consuming the supporting stack as cloud services can dramatically minimize management challenges.
