A Rap Beef (START HERE)
This is the first game in KC7cyber. It will teach you about identifying phishing campaigns, how to interpret security/audit logs to identify malicious activity and how to investigate a basic cybersecurity intrusion.

There are no requirements for that specific game. 

The scenario is that there are two hip-hop artists are in a musical feud, and you, as a Security Analyst for OWL Records, need to keep the company information safe and ensure your artists are not getting exposed during the ongoing feud.

When you start the game you are presented with the first question. On the left side there is the current question displayed with some story-relevant information and on the right side we have the environment, where you put in **Kusto Query Language (KQL)** queries and get their results, which will help answer the questions.

In this game there are two sections. The first section called "Enough beef for a burger" features 13 questions. The other section "Less beef, more phish" has 22 questions.

# Section "Enough beef for a burger":

## Question 1
Here the scenario is reiterated again. To pass this question just type `ready` in the answer field.

## Question 2:
Nothing much to do except for typing `barz` to continue.

## Question 3:
Now the story really begins. Through unethical means (bribing), you receive a hint that the IP address 18.66.52.227 was used by your competitor to probe OWL Records' systems in early April. Make a note of both the IP and early April for Question 5. After typing `thanks dawg` in the field you continue the story.

## Question 4:
This is the first question, where we use the **Kusto Query Language (KQL)**. For now, the queries we should use are being provided, but at later sections or games we have to write the queries ourselves. For now, you will be following the instructions. I marked and copied the query into the query field. I pressed the run button after that. To successfully answer the question, copy the first name you see in the results table (`Sean Crater`) into the answer field.

## Question 5:
In this question, you'll learn that you can have multiple queries in the KQL pane. You can run multiple queries in the KQL pane, if they are separated by a blank line. Click inside the query you want to run before pressing 'Run' to execute it. 

To answer the question, add the provided query to the pane, select it, and run it. You'll notice to the right of the UI element that says Done there is an element which displays how many records have been returned. Type that number (`19`) to the answer field. Note down for your report that the attacker used T1594 (Search Victim-Owned Websites) of the MITRE ATT&CK framework for their Reconnaissance.

## Question 6:
This question asks you about the information the person wanted to gather about the protagonist Dwake. For that you should look inside of the 19 results you were given. Before copying the email address as the answer, take a closer look at the last four lines for additional context. It looks like the person is trying to reset Dwakes password. 

Note down the timestamps of those four, especially the last one (`2024-04-10T13:02:47Z`), because you will potentially see some interesting activities later. Security questions pose a vulnerability in IAM systems because attackers can often find answers through **open-source intelligence (OSINT)**, social media, or data breaches. **Multi-factor authentication (MFA)** or authenticator apps are more secure alternatives. Note down that the attacker used T1589.002 (Gather Victim Identity Information: Email Addresses) in your report.

## Question 7:
The answer you are looking for is in the record with the timestamp 2024-04-10T10:52:38Z (`trash`).

## Question 8:
The answer you are looking for is in the record with the timestamp 2024-04-10T10:57:47Z (`dwake_audrey@owl-records.com`)

## Question 9:
This is why you should be careful what you post online or what is potentially visible via official documents. Attackers can easily search for answers of security questions online and therefore can impersonate you. If you must answer those questions, add a twist to your answers. Consider services that use alternatives like multi-factor authentication, email-based resets or authenticator apps for password resets. The right answer to the question is `1 and 3`.

## Question 10:
Dwake's mother's maiden name can be found in the second line of the verse (`Washington`).

## Question 11:
Dwake's childhood pet can be found in the first line of the second paragraph (`Fluffy`).

## Question 12:
This question introduces us to a query with the has_any method, which compares the left side with the list that in the provided within the brackets. Use that query and right click the url in the result and copy it to the answer field. Note down that the attacker has now a valid account (T1078 in Mitre ATT&CK) and can start acting on their objectives, as well as the timestamp for your report.

## Question 13:
This question shows what can happen if one takes over an email account. Be prepared for worse things to come, because attackers usually won't stop at defacement. Defacement is usually the last step in the killchain of an cyber attack. Type in `oh lawd` to complete the section. Congratulations!

# Section "Less beef, more phish"

## Question 1:
Just when you thought the incident is over a Ransomware post appears on one of the many forums of the dark web. In this case it's BreachForums, which is quite famous for distributing data breaches and contraband goods that are sold there.

I am wondering why the ransomware actors are still using Bitcoin as a payment method when there are alternatives that offer better anonymity. My best guess is that Bitcoin very accessible for victims. To solve the question just type `darkweb` in the answer field.

## Question 2:
Phishing (or some of its forms like vishing) are usually one of the easier ways to get into an organization. The answer of your homie is a safe bet, even if it is vague. Type in `lesdoit` to continue the story.

## Question 3:
You remember that your homie gave you an ip address. Now it is the time to use a reverse DNS lookup. A reverse DNS lookup maps an IP address to its associated domain. Security analysts use it to identify potentially malicious infrastructure, detect phishing sites, or uncover attacker-controlled servers. 

Typically, you want to do a reverse DNS lookup passively to not attract any attention from the potential attacker. For that webpages like `who.is` are the go to choice. For now you can just copy the provided query and run it. You should find the answer in the `domain` column. Note down the domain name for the next question.

## Question 4:
This time we are introduced to the take operator, which returns the specified amount of rows at random. From the provided columns (timestamp, sender, reply_to, recipient, subject, verdict and link) only sender, reply_to, recipient and link can contain domain names. 

If the attacker had bad operational security they would be sending it from their company email, but I assume that this attacker has good operational security. If the attacker has good operational security the columns sender, reply_to and recipient would only contain innocent domains. By process of elimination the most likely to contain the domain (`betterlyrics4u.com`) is the link column. I wonder why they would use their own domain as the link used in a phishing campaign.

## Question 5:
Copy the query and run it. You can count the rows manually or use the ui element that already counted the rows :)

## Question 6:
Just count the senders manually and copy the sender who has the most rows from the previous query into the answer field. No need to use more KQL than necessary.

## Question 7:
Copy the other email address in the answer field. No need to invest more brain power in here.

## Question 8:
This time we are introduced to the concept of variables in KQL. The keyword for that is `let <name> = <value>`. We are also introduced to use multiple datasets in a query. Copy that query and let it run. You'll see that the phish was targeted at the `Rapper`s in the organization. 

In the lessons learnt section of the report you will do after the incident you should suggest a phishing awareness targeted at their rappers, where they get not only generic training but also are getting a list of services that OWL Records offers internally. There is probably a Songwriter hired, so they do not need to have a ghostwriter. Maybe add some custom phishing simulations specific for this high-risk role.

## Question 9:
There is only one other role listed than Rapper. Use the query from Question 8 to get the answer.

## Question 10:
Copy the name of the `Lead Rapper`. Continue to the next question.

## Question 11:
Copy the IP address of the Lead Rapper there. Note the ip down to search for events after 2024-04-10T13:02:47Z from Question 6 of the previous section.

## Question 12:
You could copy the given query, but I decided to narrow down the results for now by adding `and recipient == "dwake_audrey@owl-records.com"` to it, because I want to see the capabilities of the editor. The query editor suggested making the part I added in a variable instead, which I accepted. I am glad that the editor has this suggestion function. That way you may learn a thing or two. My final query looks like this:

```kql
let target = "dwake_audrey@owl-records.com";
Email
| where link has "betterlyrics4u.com" and recipient == target
```

The right answer can be found in the column subject.

## Question 13:
From the previous query copy the column link. I wonder what was inside of the full email. Due to Data protection and privacy regulations we are probably prohibited to see it. Alternatively, the logging agent ignores the full email body by default.

## Question 14:
Copy the column verdict into the answer field. My guess is that the clean verdict was, because it is a legitimate site and it might have a good reputation.

## Question 15:
Just type `GhostWriter` in the answer field, which is the last word of the email. 

The phishing link could have been detected by Dwake if he would have hovered over the link and noticed that it led to a competitor. Another red flag would be that the email is very generic and that the mail came from an unknown sender. Sometimes you will get hit with sales pitches like that. Note don that the attacker used Phishing (T1566) as initial access as well.

## Question 16:
Just copy the timestamp in the result of the query you have been given. Before you move on to the next question my gut feeling as an detection engineer and analyst tells me that you should look if anyone else went to the url. 
Remove the `| where src_ip == "10.10.0.5"` from the query. Looks like someone else did also fall for the email at 2024-04-15T11:53:12Z and their ip is 10.10.0.21. Note that down for your report.

I used the following query to figure out to whom 10.10.0.21 belongs:
```kql
let employee_ip = "10.10.0.21";
Employees
| where ip_addr == employee_ip
```

Snoop Thompson also clicked on the phishing link. This indicates that the phishing campaign was effective against multiple employees, highlighting the need for an improved phishing awareness campaign and stronger email security controls (e.g., link scanning, DMARC enforcement)

## Question 17:
First things first: Why would you log in at a competitor with the credentials of the company you are employed at? This should have raised a lot of red flags. Even if it wasn't your competitor you should be very careful not to logon with your company credentials to unknown or unapproved websites. 

There is also a sign-up button unavailable, but this is a detail that could be missed easily. The page was clearly designed to capture credentials. To solve the question type in the contents of the button under Forget password.

## Question 18:
To answer that question run the provided query. Copy the timestamp in the answer field.
Before moving on, remember that in Question 16 we discovered Snoop Thompson also clicked on the link. Let's find out if he also gave away his credentials
Remove the `| where username == "dwaudrey"` from the query.

It appears that Snoop Thompson's credentials were also compromised, or another unauthorized action took place. Strangely, 11 successful authentication attempts were recorded from the suspicious IP address. This warrants immediate action! Reset the passwords for all affected users and note that down for your report.

When looking for all mails where the link contains betterlyrics4u.com it seems like everyone targeted clicked on the link and gave their credentials. Management will not be in a good mood after hearing this.

```kql
Email
| where link has "betterlyrics4u.com"
```

## Question 19:
As mentioned previously all attempts were successful. That is not good.

## Question 20:
Just run the query and count the rows. It seems like the attacker used some keywords used in classifying assets and files such as confidential, secret, sensitive to find proprietary data and company secrets. Then the attacker went through folders which indicate that they store sensitive data like internal_communications. Lastly the attacker downloaded all emails in the draft folder and zipped it into `DwakesDirtySecrets.zip`.

Let's also see what they did with other accounts. For that I have modified the query to
```kql
InboundNetworkEvents
| where timestamp between (datetime("2024-04-12T00:00:00") .. datetime("2024-05-01T00:00:00"))
| where not( url has "dwaudrey")
| where src_ip has "18.66.52.227"
```

It seems like the attacker used the same keywords and methodology, except for writing a draft email. I wonder why every rapper has a folder called employee complaints.

## Question 21:
Look in the last row of Question 20’s original query. You should find a zip file in the URL row. Copy that and you are done.

## Question 22:
You are now at the end of the game. Just type in less hack more love in the answer field.

Now you should write your report to management and suggest some improvements, f.e. regular phishing awareness campaigns tailored for high-risk groups. You might also want to design and implement some detections f.e. authentication from non-internal IP addresses or an alert when multiple people fall for the same phishing campaign. 

I am going to assume that all employees have static ip addresses there. There was likely no formal incident response plan in place, or it was incomplete. Develop and implement incident response playbooks for different attack scenarios, including phishing campaigns, credential compromise, and data exfiltration. 

Playbooks should outline detection methods, containment steps, escalation procedures, and post-incident analysis to improve resilience. While addressing these concerns, management should also restrict access to sensitive folders, such as inboxes containing confidential communications. 

Additionally, implementing a Data Loss Prevention (DLP) solution can help monitor and block unauthorized bulk email downloads, preventing potential data exfiltration. Include in your report the full timeline of the attack and your findings. By now, all affected employees have rotated their passwords.
