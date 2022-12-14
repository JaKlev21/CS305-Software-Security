# CS305-Software-Security
1.	Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

For our assignments, we were to be developers for Global Rain, helping the client Artemis Financial modernize their company by developing a secure web-based software application. Artemis Financial is a consulting company that helps its customers with financial plans like savings, retirement, investments, and insurance. To reach more customers or provide a more robust service, they needed a web-based application to keep up with the market's direction and stay competitive. 

2.	What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?

Despite my reluctance to write, I felt I was good at addressing and supporting each rubric question. Expanding on each of the topics in such a way helped clarify some of the areas of the readings that I may not have had a complete grasp of. I can read the words on the page, but retention and knowledge come from practical application. I prefer that practical application is in the form of coding the application. However, as I was chipping away at supporting my positions, I found that I was researching alternate sources that explained the subject differently, which helped my understanding and, eventually, the explanation. 

Everything is moving towards a mobile or cloud model. Very rarely are their new applications that are loaded and executed locally on anyone’s machine. This course set some important groundwork for that industry and model. The internet is a playground for others to poke and prod web applications to search for weaknesses and vulnerabilities. Often in some of the secondary static testing it was discovered that many applications vulnerabilities were introduced by the libraries and dependencies the developers chose to utilize to code the application in. In addition to this, there are vulnerabilities that the developer can induce through poor industry standards or practices. 

3.	What part of the vulnerability assessment was challenging or helpful to you?

The vulnerability assessment that I found most challenging was the researching and recording the individual dependency vulnerabilities identified. I found it more tedious than anything else. I worked to create a scraping script that would record each of the dependencies their vulnerability codes then reach out to the NVD database and get the description of each vulnerability. This allowed me to review each dependency description right next to the others and see that most had a common theme – specific versions had vulnerabilities. Knowing this it was clear that I needed to know what version was currently deployed. This made is rather simple to determine the apparent course of action would be that the required dependencies to be updated and that would patch the known vulnerabilities.

4.	How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

Understanding the methods and techniques that malicious actors have used to gain access or deny the service of a web application are great ways to help understand the layers of security. Including access controls to the data that is sent and received, such as input validation, cryptography and error handling are some of the methods that can increase layers of security. Additionally, staying current on the libraries that developers use for particular applications and what the known vulnerabilities are, are some of the methods to asses vulnerabilities and determine mitigation techniques. 

5.	How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

Once the final application was written, and the pre-refactored static test matched the post-refactored static test, it was clear that the refactored code did not introduce any new vulnerabilities. Once the application is run, it is important to look at the application through the browser and see all the data that is being passed through it. Ensuring that extra payloads cannot be passed through or regex strings could be sent to prevent the application or the hardware running it would behave differently than it was intended.

6.	What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

Resources that I have come to appreciate throughout this course was the dependency check repository that provides a link to the (sometimes many) sources that have information for each vulnerability. Looking through each of them offered some insight as to some of the communications that go on between developers who identified the vulnerability and those working to close the loop, so to speak. 

7.	Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

I have a raspberry pi computer in my garage that I took some out of the box (knew nothing about it) Apache server and developed an HTML file to read my garage door open/close status and to actuate the door opener. Taking the knowledge from this course, I have a better understanding of what that Apache server was and how it did what it did. I would rewrite that whole system to create an HTTPS server with some more access controls. Like not having a PHP script to run code straight off the raspberry pi, which could be a problem if it were run too many times or manipulated to run a different code. 
With that said, I would rather have a portfolio of working applications that I created to show interested employers. Such as the final secure “Garage Pi,” as it has come to be known.
