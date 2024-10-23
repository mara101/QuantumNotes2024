==Cybersecurity must be integrated throughout the entire lifecycle of a system==. This includes from the initial design phase through implementation, operation, and eventual decommissioning(Decommissioning refers to the intentional removal or retirement of software applications, hardware, or entire technology systems from an organization's IT environment. This process is not simply about turning off a server or uninstalling software; rather, it involves a systematic approach to ensure a smooth transition while minimizing disruptions and risks.). Proper security considerations at each stage can help mitigate risks and vulnerabilities.
#### Key Phases in the System Lifecycle:

1. **Requirements Analysis**
    
    - Identify the security needs of the system based on its functionality and environment.
    - Perform a [[RISK ESTIMATION| risk assessment]] to evaluate potential threats and vulnerabilities.
2. **Technical Options**
    
    - Evaluate different technologies and approaches for meeting the identified security requirements.
    - Consider available security products, such as firewalls, intrusion detection systems, encryption tools, etc.
3. **Design**
    
    - Integrate security into the system design.
    - Develop **security services** like authentication, authorization, and data protection.
4. **Development and Implementation**
    
    - Implement the security controls as part of the system's architecture.
    - Ensure security testing is performed to validate that the controls work as intended.
5. **Setup and Configuration**
    
    - Once the system is live, configure it securely by setting up policies and procedures.
    - Implement **security management practices** to monitor and maintain the system’s security.
6. **Security Testing**
    
    - Conduct regular **security audits** and tests to detect potential vulnerabilities or breaches.
    - Adjust security measures as necessary to respond to new threats.
7. **Operations and Management**
    
    - Actively manage the system’s security during its operation, adjusting security policies as new threats emerge.
    - Continuous monitoring and incident response plans are key during this phase.
8. **Decommissioning**
    
    - Ensure secure decommissioning of the system by removing or destroying sensitive data and revoking access controls.

#### Window of Exposure
The window of exposure is the amount of time that goes from the first time deployment of a zeroday vulnerability (or the discovery by researchers) to the installation of the patch in a system. Usually this type of visualization is represented by a graph that plot the time and the level of risk during the cycle.   
![[Screenshot_20240930_084810.png]]To minimize the window of exposure (*WOE*) researchers follows the rule of *responsible disclosure*. It consists in working with the vendors for 120 days(it may vary based on the gravity of the zeroday and the complexities derived from the creation of a patch) where in this time of period the vendor is strongly recommended to release a patch, because at the end of this period the vulnerability will be released to the public. 
This type of method prevents that others non ethical people discovers the vulnerability before the patch and takes advantage of the vulnerability.

#### What is security at the end?

If we've learned anything from the past couple of years, it’s that computer security flaws
are inevitable. Systems break, vulnerabilities are reported in the press, and still many
people put their faith in the next product, or the next upgrade, or the next patch. “This
time it’s secure,” they say. So far, it hasn’t been.
Security is a process, not a product. Products provide some protection, but the only way
to effectively do business in an insecure world is to put processes in place that recognize
the inherent insecurity in the products. The trick is to reduce your risk of exposure
regardless of the products or patches.
Bruce Schneir.



#### Flashcards
What is security?(try to reference Bruce Schneir)::[[SECURITY IN THE LIFETIME OF A SYSTEM AND WINDOW OF EXPOSURE]]
What is WOE and responsible disclosure?[[SECURITY IN THE LIFETIME OF A SYSTEM AND WINDOW OF EXPOSURE]]

