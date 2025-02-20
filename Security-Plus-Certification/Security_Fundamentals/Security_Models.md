The CIA triad is a fundamental model in information security.  It consists of three core components.  Confidentiality is guarding information (data) from unauthorized access.  Integrity is guaranteeing data exactness and preventing unauthorized modification.  Availability is guaranteeing that the data and systems are accessible when necessary.

Authentication, Authorization, and Accounting (AAA) is a framework used to gain access to a computer’s resources, enforce policies, monitor usage, provide key information needed for billing services and any other processes that are key for network management and security.  This framework is mainly used for network and software applications being accessible to specified users.
Authentication is when the user is identified to have access to the internal resources of the network.  Authentication credentials are stored in the network database.  A user will have their own authentication credentials.  If the credentials match what is saved in the database, the user will have access to the internal resources of the network.
Authorization is a method of enforcing policies.  If the user wants to access certain things about the network; they must have authorization to do so.  
Accounting is the monitoring of a user while they are accessing the network.  What is monitored is the login time, the data sent, the data received, and the logout time.  

Security models are recommendations on how security should be implemented within an organization.  Security models are structures that specify which people should have access to data and the operation of the operating system.  Security models give mathematical mappings of theoretical goals.  The three “classic” models, that also serve as the foundation for several other models, are Bell-LaPadula model, Biba model, and Clark-Wilson model.  There are two other models worth mentioning.  The Brewer and Nash model and Harrison Ruzzo Ullman model.

The Bell-LaPadula model is multilevel.  The model creates a set of access rules and security levels that indicate how users may access objects at various security levels.  This model is usually used by the military or government institutions.  Some banks and hospitals also use the model because they too have very important data to protec.  The model consists of three rules.   
The Simple Confidentiality Rule: the user may only read files at the same level of security or lower.  It is also called the no read-up rule.
Star Confidentiality Rule: the user may only write files at the same level or the upper-level security.  It is also called the no write-down rule.
Strong Star Confidentiality Rule: the user may only read and write files on the same level of security.  There is no access to files above or lower than the user’s security level.  It is also called the No read write-up or down rule.  It is the most secure rule.

The Biba model was created to improve upon the Bell-LaPadula model.  The Biba model conveys a set of access control rules specified more maintaining data integrity.  Data and subjects are organized or categorized according to how reliable they are.  The model consists of three rules.
No Write-Up (Integrity Axiom): no one is allowed to add to or change data that has a lower integrity level.
No Read Down (Simple Security Property): a user cannot read a file with a higher integrity level.  
In this model a user only has access to what they are authorized to have access to.

The Clark-Wilson model was created to protect data integrity from threat actors and their malicious intentions.  The model conveys that the system should maintain consistency between internal and external data.  That only authorized users should be allowed access to data and the ability to make alteration to the data.  No unauthorized user should be allowed access whatsoever.  This model specifies how data should behave to maintain their validity when they change from one system state to another.  The model outlines certification, enforcement procedures and the capabilities of the principles used inside the system.

The Brewer and Nash model was created to establish a set of rules to reduce conflicts of interest.  The model’s goal is to prevent a user from having access to sensitive data that could lead to dire consequences due to personal conflicts of interest.  The model supports data segregation and dynamic access controls.  Dynamic access controls are determined based upon the user’s previous interaction with the sensitive data.

The Harrison Ruzzo Ullman model (HRU) was created to address concerns over information flow.  This model adopts discretionary access control utilizing an access matrix to understand allowable actions that users can perform on files.







