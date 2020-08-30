## Event Driven Applications

* Event Driven Programming - A classic example of event driven programming is the web browser. Every interaction with a webpage through it's interface is an event. Clicking buttons, pressing a key, etc. 
  * Event hanlders are callback functions to be called when an event is triggered
  * A loop listens for event triggers and calls the associated event handler for the given event

* Why is access control important? - Access control is important because of the principle of least privilege. Users should only be given access to information that is absolutely vital to their ability to complete a given task. 
* Describe an application that would need access control - An application that might need access control would be a financial appliation such as Quickbooks. For example, I had several responsibilities in my previous job that required limited access to our company's financial system in order to invoice accurately. However, the company did not grant me access to other sensitive information such as employee salaries, company profitability, and so forth.  
* What is a role used for? - A role is used to limit the amount of access that an employee has. For instance, a "user" role might have a certain type of access to an application, while an "admin" role might have more expansive access to the same application. 
* Why is role based access control more scalable than discretionary or mandatory access control? - It is easier to define access control based on a limited set of job roles and then place individuals in the appropriate role than to control access through mandatory control, which requires much more planning and higher cost, and discretionary control which increases the risk that data will be made accessible to users who should not have access to it. 

### Vocabulary

* Authorization - Policies that define what an individual or group may access. 
* Role Based Access Control - A method of controlling access based on prescribed roles
* Capabilities - The specific type of access that a given role has, such as "edit, comment, read". 