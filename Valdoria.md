- [Section 1: "KQL 101"](#section-1-kql-101)
  - [Question 1:](#question-1)
  - [Question 2:](#question-2)
  - [Question 3:](#question-3)
  - [Question 4:](#question-4)
  - [Question 5:](#question-5)
  - [Question 6:](#question-6)
  - [Question 7:](#question-7)
  - [Question 8:](#question-8)
  - [Question 9:](#question-9)
  - [Question 10:](#question-10)
  - [Question 11:](#question-11)
  - [Question 12:](#question-12)
  - [Section summary](#section-summary)
- [Section 2: "Welcome to Valdoria"](#section-2-welcome-to-valdoria)
  - [Question 1:](#question-1-1)
  - [Question 2:](#question-2-1)
  - [Question 3:](#question-3-1)
  - [Question 4:](#question-4-1)
  - [Question 5:](#question-5-1)
  - [Question 6:](#question-6-1)
  - [Question 7:](#question-7-1)
  - [Question 8:](#question-8-1)
  - [Section summary](#section-summary-1)
- [Section 3: Plenty of Phish](#section-3-plenty-of-phish)
  - [Question 1:](#question-1-2)
  - [Question 2:](#question-2-2)
  - [Question 3:](#question-3-2)
  - [Question 4:](#question-4-2)
  - [Question 5:](#question-5-2)
  - [Question 6:](#question-6-2)
  - [Question 7:](#question-7-2)
  - [Question 8:](#question-8-2)
  - [Question 9](#question-9-1)
  - [Question 10](#question-10-1)
  - [Question 11](#question-11-1)
  - [Question 12:](#question-12-1)
  - [Question 13:](#question-13)
  - [Question 14:](#question-14)
  - [Question 15:](#question-15)
  - [Question 16:](#question-16)
  - [Question 17:](#question-17)
  - [Question 18:](#question-18)
  - [Question 19:](#question-19)
  - [Question 20:](#question-20)
  - [Question 21:](#question-21)
  - [Question 22:](#question-22)
  - [Question 23:](#question-23)
  - [Question 24:](#question-24)
  - [Question 25:](#question-25)
  - [Question 26:](#question-26)
  - [Section summary](#section-summary-2)
- [Section 4: A scandal](#section-4-a-scandal)
  - [Question 1:](#question-1-3)
  - [Question 2:](#question-2-3)
  - [Question 3:](#question-3-3)
  - [Question 4:](#question-4-3)
  - [Question 5:](#question-5-3)
  - [Question 6:](#question-6-3)
  - [Question 7](#question-7-3)
  - [Question 8:](#question-8-3)
  - [Question 9](#question-9-2)
  - [Question 10](#question-10-2)
  - [Question 11](#question-11-2)
  - [Question 12](#question-12-2)
  - [Question 13](#question-13-1)
  - [Question 14](#question-14-1)
  - [Question 15](#question-15-1)
  - [Question 16](#question-16-1)
  - [Question 17](#question-17-1)
  - [Question 18](#question-18-1)
  - [Question 19](#question-19-1)
  - [Question 20](#question-20-1)
  - [Question 21](#question-21-1)
  - [Question 22](#question-22-1)
  - [Question 23](#question-23-1)
  - [Question 24](#question-24-1)
  - [Question 25](#question-25-1)
  - [Question 26](#question-26-1)
  - [Question 27](#question-27)
  - [Question 28](#question-28)
  - [Question 29](#question-29)
  - [Question 30](#question-30)
  - [Question 31](#question-31)
  - [Question 32](#question-32)
  - [Question 33](#question-33)
  - [Question 34](#question-34)
  - [Section summary](#section-summary-3)
- [Bonus](#bonus)
  - [Section 4, Question 9](#section-4-question-9)
  - [Section 4 Question 12](#section-4-question-12)
- [Final remarks](#final-remarks)
  - [Phishing awareness is critical](#phishing-awareness-is-critical)
  - [Detection without response is ineffective](#detection-without-response-is-ineffective)
  - [Access control weaknesses](#access-control-weaknesses)
  - [Credential theft and password hygiene](#credential-theft-and-password-hygiene)
  - [Lack of network egress monitoring](#lack-of-network-egress-monitoring)
  - [Persistence \& Post-Exploitation Activity](#persistence--post-exploitation-activity)
- [Next steps](#next-steps)
  - [Incident Response \& Remediation](#incident-response--remediation)
  - [Security Awareness Training](#security-awareness-training)
  - [Implement MFA \& Password Policies](#implement-mfa--password-policies)
  - [Improve Logging \& Monitoring](#improve-logging--monitoring)
  - [Harden infrastructure](#harden-infrastructure)


**A Scandal in Valdoria**

This is the second game in KC7cyber. It will teach you about basic **Kusto Query Language (KQL)** Syntax, including the commands "where", "take" and "distinct". You will learn to effectively filter data and apply time-based filters. You will correlate events in order to create a full timeline of the attacks. Additionally, you will learn and to interpret Powershell scripts and the corresponding malicious commands run by attackers.

There are no requirements for the game.
The scenario is that an election is upcoming in Valdoria. The Valdorian Times published an unauthorized article accusing the leading candidate of corruption. You will help investigate the attack that occurred.

The game has four sections. First is "KQL 101" and features 12 questions around KQL. The second section is called "Welcome to Valdoria" and has eight questions. The third section "Plenty of phish" features 26 questions, while the last section "A scandal" has 34 questions.

# Section 1: "KQL 101"
Before we can start investigating attacks, we need to know how to ask the right questions. This starts with mastering Kusto Query Language (KQL). This section lays the groundwork. You'll get familiar with core KQL operators like `take`, `where`, `count`, and `distinct`. If you've worked with other query languages before (like SQL or SPL), KQL will feel intuitive. Even if you haven't, don't worry, because we'll build it up as we go.

This section is intentionally basic, but don't skip it. Knowing how to pivot quickly across tables, isolate key fields, and narrow timeframes is foundational in threat hunting. You'll also start to think like an analyst by asking "What am I trying to prove or disprove with this query?".

## Question 1:
Here the scenario is reiterated again and features a video. I would suggest that you read the accompanying training guide, which is linked under the video. To pass this question just type `ready` in the answer field.

## Question 2:
Here you will learn about the **Azure Data Explorer (ADX)**, which is on the right pane. By now you should have read the training guide. If you haven't you *should* do it now, because it will help you answer all the questions in this section.

In this question you will learn on how to use the **take** operator. This operator returns up to the specified number of rows, but the order of rows is not guaranteed. Copy the provided query and run it. Your task is to run the query for each table. Below is a template you can use:

```kql
Table
| take 10
```
Familiarize yourself with the columns and the data. In the real world you will sometimes see fields that are not populated or missing completely. Then you do need to find alternative ways to prove or disprove your hypothesis.
When you are done with that type `done`.

## Question 3:
Here we are introduced that one can just copy and paste the queries that are given to us. The current task is to figure out how many employees are working at the Valdorian Times. For that you should use the `count` operator. Run the provided query and type in the answer.
 
## Question 4:
Here they introduce the **where** operator, which you will use frequently, because you will almost never want the full dump of a table. The template of a where operator looks like this:

```kql
Table
| where <field> <operator> <value>
```

This time the task is to figure out the editorial director's name.
Just copy the query under the question and run it. Copy the value you see in the `name` column to the answer field.

## Question 5:
This time the question asks about the amount of emails that `Nene Leaks`received. For that they introduce the `count` operator, which counts the rows returned by the query.

If you still have the query from the previous question you can get her email address from the column `email_addr`. Then paste the email address in the query below:

```kql
Email
| where recipient == "Nene's Email Address Here"
| count
```

## Question 6:
Here the `distinct` operator is introduced. In order to figure out how many distinct senders sent emails from the domain `weprinturstuff.com` replace `<Domain Name>` with the domain and `<field>` with sender in the provided query.

Copy the result of the query into the answer field.

## Question 7:
This time we are asked to calculate the number of distinct sited `Lois Lane` visited.

In order to fill the placeholders in the given query, we need to figure out Lois Lane's IP address. For that we'll use the query:

```kql
Employees
| where name=="Lois Lane"
```
Note down the column `ip_addr`, because we'll use in in further steps.

Next, we should look for all outbound network events from Lois:
```kql
OutboundNetworkEvents
| where src_ip == "10.10.0.22"
```
From the returned rows only the column `url` seems to have websites in it. Let's use that for the distinct operator. Additionally we should count the distinct results.

The final query should now look like this:
```kql
OutboundNetworkEvents
| where src_ip == "10.10.0.22"
| distinct url
| count
```
Now run that query and enter the result into the answer field.

## Question 8:
This time we should figure out how many distinct domains in the `PassiveDns` records contain the word "hire".

First we should look at the table PassiveDns again to remember its columns.

```kql
PassiveDns
| take 10
```
Luckily the column `domain` contains the domain name. The column `ip` contains the ip the domain resolves to. If the column `ip` is empty or missing we must figure it out otherwise, f.e. with the lookup service `who.is`.

Now that we know that the `domain` field holds the domain, we can finish the query that was provided by the question.

```
PassiveDns
| where domain contains "hire"
| distinct domain
| count
```
Run that query and put the result in the answer field.

## Question 9:
This time we are asked to provide one of the ips the domain `jobhire.org` resolves to.
If you remember from last question that the ip a domain resolves to is stored in the column `ip` You can just replace `<field>` with it. Other than that just replace the domain with `jobhire.org`. Run the query and copy one of the ips returned into the answer field.

## Question 10:
This time we should figure out how many distinct websites employees with the first name "Mary" visited.

This question also introduces us to variables, which are defined with the let keyword. `let <name> = <value>;` is a template on how you use variables. In this question we also learn that the value of a variable can also be the result of a query.

This time you have to add the unique count to the query that is given to us.
If you forgot how the table OutboundNetworkEvents looks like you can always do 
```kql
OutboundNetworkEvents
| take 10
```

Figure out where the websites could be stored. Once you have figured that out run the query and put the result in the answer field.

## Question 11:
This time you have to replace `<list_variable_name>` with a name you want to give it and `<Employee Name>` with `Mary`to solve the question.

## Question 12:
Congratulations! You have passed **KQL 101** and have learnt. Type in `ready` to progress to the next section. 

## Section summary
You learned the fundamentals of KQL:

-    How to look at sample data with `take`,
-    Narrow results with `where`,
-    Count events with `count`,
-    And remove duplicates with `distinct`.

More importantly, you started thinking like an analyst. The goal isn't just to write queries, it's to extract meaning. You also got your first exposure to real-world workflow issues, like null fields, timestamps, and understanding your environment before diving in. Don't underestimate how important that is.

# Section 2: "Welcome to Valdoria"
## Question 1:
Now the story starts. You are introduced as an incident responder to the Valdorian Times. Extract the Newspaper Printer's name out of the screenshot provided.

## Question 2:
This is the first question, where you are not given any query. The task is to figure out the Editorial intern's name.

First of all we should start our query with the `Employees` table and then filter for the `role` "Editorial Intern". The full query should look like this:

```kql
Employees
| where role == "Editorial Intern"
```
Copy the name you get into the answer field (**Ronnie McLovin**).

## Question 3:
This time we should figure out when Ronnie McLovin was hired. If you still have the query from last question copy the field `hire_date` exactly.

## Question 4:
This time we're getting some juicy new information. It seems like Ronnie forgot to send the final draft to `Clark Kent`, but Clark is certain that the final draft came from Ronnie on `January 31, 2024`. Note that date, because I have a feeling we'll find someone impersonating Ronnie.

To answer the question we have to figure out how many total emails `Clark Kent` received. For that we would have to find any Emails, which were sent to Clarks Email address and use the count function.

First of all we should get Clark Kent`s Email. We can just lookup the email address in the Employee table.
```kql
Employees
| where name == "Clark Kent"
```
His Email address is `clark_kent@valdoriantimes.news`. Time to build the final query.
```kql
Email
| where recipient == "clark_kent@valdoriantimes.news"
| count
```
Run the query and write the result in the answer field.

## Question 5:
This time we should figure out what the subject was on the email sent to him on Jan 31 2024.
This can be done by just listing all Emails, where the recipient is `clark_kent@valdoriantimes.news`, but I think that there should be a better way to do this, especially when you have millions or billions of logs per day.

The first idea I had was that one could also limit the time you search with timestamps. For that the between operator should be helpful.

After googling for `kql timestamp comparison` I found a reddit thread (https://www.reddit.com/r/AzureSentinel/comments/18a8jjo/question_on_how_to_query_a_specific_date_in_kql/) and there was one comment, which gave me a hint to use the datetime data type (see https://learn.microsoft.com/en-us/kusto/query/scalar-data-types/datetime?view=microsoft-fabric). In order to get the time range I used the between operator (see https://learn.microsoft.com/en-us/kusto/query/between-operator?view=azure-data-explorer for documentation).

Here is the query that I used:
```
let startdate=datetime("2024-01-31");
let enddate=datetime("2024-02-01");
Email
| where recipient == "clark_kent@valdoriantimes.news" and timestamp between (startdate .. enddate)
```
To answer the question copy the subject row to the answer field.

## Question 6:
In Order to answer this question copy the sender value of the previous questions query in there. Looks like Ronnie sent the mail.

## Question 7:
This time we should get the name of the docx file that was sent in this email. The only field which could have the document would be in the body of the email, but we do not have that. The column `link` should have this somewhere.
Copy the name of the document (`OpEdFinal_to_print.docx`) and write it down in your report.

## Question 8:
After questioning Ronnie you get the answer that she did not send the email and does not recall any unusual emails or weird activity on her computer. This suggests the sender may have been spoofed. Let's write that down as a hypothesis.

Answer the question with `yes`.

## Section summary
This section introduced the initial incident and gave you your first real investigation targets. You pulled user metadata, email addresses, and timelines and learned how to start validating or challenging assumptions.

Takeaways:

-    Most investigations begin with incomplete information.
-    You used simple queries to prove/refute who sent what, and when.
-    You built intuition on how attackers may try to spoof identities or cover tracks.

This is how real investigations work.

# Section 3: Plenty of Phish
This is where things start getting real. We're no longer just poking around benign data, because we're uncovering signs of real malicious activity. Suspicious emails, document downloads, external infrastructure. Those are the classic hallmarks of a phishing campaign and they are all here.

Expect to do deeper correlation work in this section: tracking a single email to multiple recipients, connecting it to network activity, and building timelines. You'll also start working like an actual threat hunter — not just answering what happened, but asking who else might've been affected?

Also, expect to make mistakes. I missed a whole set of emails the first time through and that's okay. Real analysts make mistakes, double back, and learn from them. That's part of the process.
## Question 1:
This time `Sonia Gose` hints to you that she has something to help your investigation.
This time we want to know `Sonia Gose`'s job role. For that we can look at the `Employee` table and look at the `role` column.
```kql
Employees
| where name has "Sonia Gose"
```
Type in her role and proceed to the next question.

## Question 2:
Now things get quite interesting. Sonia got a suspicious email a few weeks before the article was published.
The email came from `newspaper_jobs@gmail.com` and has several signs, which are typical for phishing messages. The email has some grammar issues, as well as a prominently placed link with a generic message.

There is also a mismatch with the job mentioned in the header and in the message of the email. Any good recruiting agency or company uses their own domain instead of a free mail service like gmail.

## Question 3:
Now that we have figured out that the email came from `newspaper_jobs@gmail.com` we should look at the timestamp when it was sent.
For that you can use the query
```kql
let startdate=datetime("2024-01-10");
let enddate=datetime("2024-01-11");
Email
| where recipient =="sonia_gose@valdoriantimes.news" and sender == "newspaper_jobs@gmail.com"
```

Before answering with the timestamp, it's worth checking whether similar emails were sent to other employees.

A quick search with 
```kql
Email
| where sender == "newspaper_jobs@gmail.com"
```
reveals that Sonia was not the only person targeted. The other targets were `Steve Jobs`, `Tom Brokaw`, `Chad Niles`, `Linus Torvalds` and `Kenneth But`. Looking their roles up we have IT specialists, Congressional Reporters and other roles. 

You can do that with the query
```kql
let suspicious_mails=
Email
| where sender == "newspaper_jobs@gmail.com"
| distinct recipient;
Employees
| where email_addr in (suspicious_mails)
```
To me it seems that this was not a targeted attack. The spam filter flagged links coming from that email address as suspicious at least after the email to Sonia.

## Question 4:
You can answer that with the same query you used to find the timestamp in the last question. Just copy the link.

## Question 5:
Sonia does not remember if the clicked on the link. Hopefully we have some indicators in our logs. For that we need to know Sonias IP address. The IP address can be found in the `Employees` table.
```kql
Employees
| where name has "Sonia Gose"
```
If there is no IP address then we need to figure it out with other means, for example by pinging the hostname with the program `ping`.

## Question 6:
Now that we know Sonias Ip address we can answer if she clicked on the link. For that we need the table OutboundNetworkEvents.
With the query 
```kql
let employee_ip=
Employees
| where name has "Sonia Gose"
| distinct ip_addr;
OutboundNetworkEvents
| where src_ip in (employee_ip) and url has "https://promotionrecruit.com/" 
```
we can figure out if she clicked on the link. There seems to be one entry in the result, which means that she clicked on the link. Copy the timestamp to the answer field. 

Unfortunately there is no status code to figure out if it was successful, but in this case we can live without it. The organization should make sure that the status code is always logged.

Let's see if the other colleagues clicked on the link.
```kql
let employee_ip=
Employees
| where name in ("Sonia Gose", "Steve Jobs", "Tom Brokaw", "Chad Niles", "Linus Torvalds", "Kenneth But") 
| distinct ip_addr;
OutboundNetworkEvents
| where src_ip in (employee_ip) and url has "https://promotionrecruit.com/"
```
It seems like someone else clicked on the link. Let's look who it is.
```
Employees
| where has_ipv4(ip_addr, "10.10.0.79")
```
It seems like `Linus Torvalds`, the `IT Specialist` clicked on the link as well. This warrants more phishing awareness training.

## Question 7:
This time we should figure out the file name of the docx that Sonia clicked. For that we have to look at the url column of the results and copy everything after the last slash.

## Question 8:
We are suspecting that the file was not just viewed, but automatically downloaded to Sonia's host. For that we'd have to figure out the hostname. Luckily the `Employees` table has the column `hostname`.

Run the query
```kql
Employees
| where name has "Sonia Gose"
```
to figure out the host and copy it into the answer field (`UL0M-MACHINE`). If there was no hostname you can try to look it up with `nslookup`, but it can fail, depending on the configuration of the DNS server.^You can also try to get the hostname from the asset inventory if you have one.

Let's also figure out the hostname of Linus Torwalds. With the query
```kql
Employees
| where name has "Linus Torvalds"
```
we figure out that his hostname is `8E37-LAPTOP`. Note that down just in case we want to investigate further.

## Question 9
This time we should figure out when the docx file was downloaded onto Sonia's machine.

First of all we should check if we have logs for the creation of files. It seems like we do, because we have a table with the name `FileCreationEvents`. Now we have to filter for the hostname and the filename, which we have answered in previous questions.
The final query should look like this:
```kql
FileCreationEvents
| where hostname has "UL0M-MACHINE"and filename == "Valdorian_Times_Editorial_Offer_Letter.docx"
```

Copy the timestamp (`2024-01-05T10:24:04Z`) into the answer field, however we should clarify if `Linus Torvalds` did also download the file. For that we just have to replace the hostname in our query.
```kql
FileCreationEvents
| where hostname has "8E37-LAPTOP"and filename == "Valdorian_Times_Editorial_Offer_Letter.docx"
```
It looks like Linus did also download the docx. Note down the timestamp `2024-01-08T10:53:27Z` for your report. You should ask Linus why he downloaded it as well.

## Question 10
If you still have the query open from last question just copy the value in the path column.
You may want to write that down for your report, but it's not that important.

## Question 11
Now just copy the sha256 column into the answer field (**60b854332e393a6a2f0015383969c3ac705126a6b7829b762057a3994967a61f**).
It would be interesting to see if Linus also got the same sha256 value for the document he downloaded.
Running the query 
```
FileCreationEvents
| where hostname has "8E37-LAPTOP"and filename == "Valdorian_Times_Editorial_Offer_Letter.docx"
```
reveals a different hash (**49f0fabe89ffbf9c8f56f110db31d1f2b0961ea810179451089531e45e1284be**). This can mean one of the following:
 
 - A completely different payload
 - The same payload with added padding
 - The same payload with a different encoding

since a good hash changes completely if even one bit changes in the file that was hashed.

## Question 12:
This time we are asked to figure out the name of the `.ps1` file that was written to disk immediately after the docx was downloaded. For that we should modify our query a bit to search around the timestamp. 

I would suggest from my personal experience to start with a time span of about one minute and expand if you don't find anything. If you find too much or the query takes too long you may want to shrink the time span instead. 

Sometimes the logs have some delay until they are ingested into the solution you use and you may want to try again after a few minutes or longer time periods (sometimes up to 30 minutes or an hour).

Here is the query I used:
```kql
FileCreationEvents
| where hostname has "UL0M-MACHINE"and timestamp between (datetime(2024-01-05T10:24:04) .. datetime(2024-01-05T10:25:04))

```
In the case of Sonia, the dropped file is called `hacktivist_manifesto.ps1`.

Let's see if the same happened at Linus machine:
```kql
FileCreationEvents
| where hostname has "8E37-LAPTOP"and timestamp between (datetime(2024-01-08T10:53:04) .. datetime(2024-01-08T10:54:04))
```
And we see the same file has been dropped It has even the same hash, so we can cross out the completely different payload option in question 11.

## Question 13:
Just copy the timestamp of the ps1 file.

## Question 14:
You can solve this quickly by googling `ps1 file extension`. For me it liked to `https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_scripts?view=powershell-7.5`, which explains in detail that **PowerShell scripts** have the `.ps1`file extension.

## Question 15:
Luckily the forensics you did yielded the copy of the powershell script. 

This looks to me like a simple downloader and the attacker does not have good operational security, which makes life easier for us as defenders. Not only did they forgo the option to go fileless, but also dropping it in the clear, so that you can analyze it. Additionally announcing that you are doing something nefarious and not doing it silently is screaming script-kiddie at best.

You can already note down the link `https://the.earth.li/~sgtatham/putty/latest/w64/plink.exe` and the ip `205.129.146.36` as indicators of compromise down in your report.

To answer the question copy the string in line 19 to the answer field.

## Question 16:
Line 11 of the power shell script will give you the answer to that question.

## Question 17:
To answer that question you should look at the powershell script and figure out the program that it tries to download (`plink`)

## Question 18:
This time we should figure out how many Process Events are related to the PowerShell script on Sonias machine. For that we should look in the table of `ProcessEvents`.
Using the hint we should look at the proccess_commandline column to see if it contains the powershell script. The final query should look like this:
```kql
ProcessEvents
| where hostname has "UL0M-MACHINE" and process_commandline has "hacktivist_manifesto.ps1"
| count
```

## Question 19:
For this question we'd have to remove the count and look at the second event, which is using schtasks to create Persistency. Write down in your final report that `T1053.005` was used for persistency. 

It also seems that the task is created in a 5th hour, because it has the parameters `\sc hourly` set with the modifier `/mo 5`.
Copy the `process_commandline` into the answer field.

## Question 20:
This time we should figure out the execution policy used in the execution of the powershell script. For that we will have to look near the `-ExecutionPolicy` argument. It is set to `Bypass`, so it will run with no restrictions set, regardless of what the machine's global or user-level execution policy is being set.

## Question 21:
This time we should figure out what IP address is used whn plink was executed on Sonias machine. This time we have to modify our query again to check for plink instead of powershell.
The resulting query will look ike this:
```kql
ProcessEvents
| where hostname has "UL0M-MACHINE" and process_commandline has "plink"
```
It seems like the IP changed from the initial execution to `136.130.190.181`. Write that IP down as an indicator of compromise.

Let's look at Linus machine again to see if there are more IPs associated with this.
```kql
ProcessEvents
| where hostname has "8E37-LAPTOP" and process_commandline has "plink"
```
It seems like the associated IPs change with each execution or machine. For Linus machine we found the IP `25.105.41.53`. This is exactly why IPs are not good indicators, because they can be changed easily.

## Question 22:
This time we want to know which username the attacker used when connecting via plink.
For that we need to dissect the commandline again, focusing this time near the `-l` argument (`$had0w`). 

## Question 23:
This time we want to have the password of the user `$had0w`. It is near the `-pw` argument.

## Question 24:
This time we are tasked to find a command with six letters that can be used to figure out which user the attacker is logged on is. For that we should look at the ProcessEvents table of Sonias machine and narrow down the timeframe by selecting all events at the time plink was run and afterwards. 

That gives us too much results. Usually all shell commands are run with the parent process name `cmd.exe` . 

Here is the final query:
```kql
ProcessEvents
| where hostname has "UL0M-MACHINE" and parent_process_name has "cmd" and timestamp >= datetime(2024-01-06T02:39:35Z)
```
Out of the results we get there is only one commandline that has exactly six letters (`whoami`). Enter that into the answer field.

Let's also look what happened to Linus pc.
After checking the timestamp when plink was executed and using the query
```kql
ProcessEvents
| where hostname has "8E37-LAPTOP" and process_commandline has "plink"

ProcessEvents
| where hostname has "8E37-LAPTOP" and parent_process_name has "cmd" and timestamp >= datetime(2024-01-09T03:33:33Z)
```
we see that nothing happened after plink was started. We definitively need to reimage/ clean up both Linus and Sonias machines.

## Question 25:
This time we should figure out how many discovery commands were run on Sonias machine. For that you can use the previous questions query.

if you are not sure if it is a discovery program just google the commandline.
In total there should be 5 discovery commands there. 

Those are `whoami` to figure out the currently logged on user, `ipconfig`to figure out network adapters and their connection status together with some addresses, `arp -a` to list the address resolution protocol cache, `tasklist /svc` to display active processes along with the services hosted by each process, while `net view` displays a list of computers, devices or shared resources on a network.

## Question 26:
We hit a dead end. The logs on Sonias machine are uninteresting. It seems that the attackers didn't find what they were looking for there. The question is if we should stop the investigation there. My gut feeling and the evidences that we found before (infection of Linus Torvalds PC) suggest that we should definitively continue.

## Section summary
This was your deep dive into phishing tradecraft. You tracked suspicious emails, extracted IOCs, confirmed link clicks via outbound network traffic, and validated file drops via file creation logs. You even compared hashes and investigated differences.

You also saw:

-    Not all users behave the same (some clicked, some didn't).
-    Hash changes don't always mean new malware.
-    Indicators like domains, hashes, and IPs must be collected methodically.

This section mirrors what a real threat hunter or SOC analyst does after a phishing alert - not just reacting, but expanding the blast radius to find who else was hit.

# Section 4: A scandal
Now that you've got the basics of KQL under your belt, it's time to start putting it to work in an actual scenario. In this section, the investigation kicks off. You're being brought in to support an internal incident at the Valdorian Times.

The questions here start light, but they teach an important point: how to pivot from open-ended objectives (“who sent this?” or “when was this file sent?”) into specific queries that give you answers. This mimics how investigations often begin in the real world — someone flags an issue, and it's your job to turn vague concerns into concrete leads.

## Question 1:
Now we should use what we have learnt to find other victims of the incident. This time we should figure out how many emails `valdorias_best_recruiter@gmail.com` was sending to our colleagues. For that a simple query is sufficient:
```kql
Email
| where sender has "valdorias_best_recruiter@gmail.com"
| count
```
Run that query and type in the result in the answer field. 

It seems I have made a mistake in Section three, where I forgot to check the `reply_to` field in the email table and as therefore missing these 18 emails. Mistakes *will* happen to you. Making mistakes is often the best way to learn. If you are embracing them and learn from them you will grow more than you think.

For now we should figure out which Employees got email from `valdorias_best_recruiter@gmail.com` and the domains in the links.

For the affected employees I will use the query:
```kql
let affected_employees = 
Email
| where sender has "valdorias_best_recruiter@gmail.com"
| distinct recipient;
Employees
| where email_addr in (affected_employees)
```
Remember that query for later steps.

For the domains I will use the query
```kql
let domains =
Email
| where sender has "valdorias_best_recruiter@gmail.com"
| distinct link
```
Write down the domains of the links in the report as indicators of compromise and defang them. Defanging protects you and the reader from accidentally clicking on malicious IP addresses and links that could lead to infection. Defanging is done by surrounding any dots or colons with brackets.

## Question 2:
This time we ant to figure out when `valdorias_best_recruiter@gmail.com` sent an email to `Ronnie McLovin`.
For that we can use the query
```kql
Email
| where sender has "valdorias_best_recruiter@gmail.com" and recipient == "ronnie_mclovin@valdoriantimes.news"
```
Copy the timestamp into the answer field.

## Question 3:
Copy the link out of the last query and leave the domain in there.

## Question 4:
Copy the subject out of the last query into the answer field.

## Question 5:
Now we should check if Ronnie clicked on the link. For that I built a template where we just need to replace the name of the employee. because we might need it for other employees.
```
let colleague_name= "name";
let colleague= 
Employees
| where name==colleague_name
| distinct email_addr;
let mail_link =
Email
| where sender has "valdorias_best_recruiter@gmail.com" and recipient in (colleague)
| distinct link;
let colleague_ip =
Employees
| where name==colleague_name
| distinct ip_addr;
OutboundNetworkEvents
| where src_ip in(colleague_ip) and url in (mail_link)
```

Copy the timestamp to the answer field and note it down in your report.

Here I also built a query that returns everyone that got an email from `valdorias_best_recruiter@gmail.com` and clicked on the provided link.

``` kql
let affected_employees = 
Email
| where sender has "valdorias_best_recruiter@gmail.com"
| distinct recipient;
let ips=
Employees
| where email_addr in (affected_employees)
| distinct ip_addr;
let domains =
Email
| where sender has "valdorias_best_recruiter@gmail.com"
| distinct link;
let event_ips=
OutboundNetworkEvents
| where src_ip in(ips) and url in(domains)
| distinct src_ip;
Employees
| where ip_addr in (event_ips)
| distinct name, role
```
and the result is terrifying to say the least:

| Name           | Role                        |
|----------------|-----------------------------|
|Ronnie McLovin  | Editorial Intern            |
|Seymour Hersh   | Lead Investigative Reporter |
|Larry Page      | IT Specialist               |
|Mark Zuckerberg | IT Specialist               |
|Barbara Walters | Director of News Operations |
|Craig Zimmerman | Congressional Reporter      |
|Kathleen Hopper | Congressional Reporter      |
|Dan Rather      | Director of News Operations |
|Peter Parket    | Director of News Operations |
|Ida Tarbell     | Lead Investigative Reporter |
|Bob Woodward    | Lead Investigative Reporter |
|Tom Brokaw      | Director of News Operations |
|Nene Leaks      | Editorial Director          |
|Carl Bernstein  | Lead Investigative Reporter |
|Bill Gates      | IT Specialist               |
|Tyler Byers     | Congressional Reporter      |

It seems that out of the 16 recipients everyone clicked on the link. Valdorian Times has 100 employees and this warrants a phishing awareness training for the whole company, since this click rate is too high.

## Question 6:
This time we should extract the filename out of the url. For Ronnie it would be `Editorial_J0b_Openings_2024.docx`. Let's also build a table for the other colleagues that clicked on the link using the previous question table was a basis nd the first KQL query of question 5.

| Name           | File                                        | when_clicked         |
|----------------|---------------------------------------------|----------------------|
|Ronnie McLovin  | Editorial_J0b_Openings_2024.docx            | 2024-01-10T08:55:07Z |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:03:21Z |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:40:16Z |
|Larry Page      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:22:10Z |
|Mark Zuckerberg | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:05:30Z |
|Barbara Walters | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:58:13Z |
|Barbara Walters | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:35:27Z |
|Craig Zimmerman | Editorial_J0b_Openings_2024.docx            | 2024-01-12T11:38:55Z |
|Kathleen Hopper | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:11:51Z |
|Dan Rather      | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:35:36Z |
|Peter Parket    | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:34:45Z |
|Ida Tarbell     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:19:58Z |
|Bob Woodward    | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:00:51Z |
|Tom Brokaw      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:09:50Z |
|Nene Leaks      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T08:48:23Z |
|Carl Bernstein  | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:55:17Z |
|Bill Gates      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:52:08Z |
|Tyler Byers     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T09:35:48Z |

## Question 7
Now we should figure out when the docx were downloaded. The question asks for `Ronnie McLovin` only, but we'll do it for everyone we have in the table.

For the query I used the project operator (https://learn.microsoft.com/en-us/kusto/query/project-operator?view=azure-data-explorer) to only get the columns i wanted instead of the distinct operator, which will discard duplicates.
```kql
let colleague_name = "Ronnie McLovin";
let file = "Editorial_J0b_Openings_2024.docx";
let when_clicked = datetime(2024-01-10T08:55:07Z);
let machine_name =
Employees
| where name has colleague_name
| project hostname;
FileCreationEvents
| where hostname in (machine_name) and filename has file and timestamp >= when_clicked
| project timestamp
```
For Ronnie it was downloaded at `2024-01-10T08:55:17Z`.

Let's redo the table with the downloaded time and their sha256 hashes. For that include `,sha256` after the timestamp in the last query.

| Name           | File                                        | downloaded           | sha256                                                           |
|----------------|---------------------------------------------|----------------------|------------------------------------------------------------------|
|Ronnie McLovin  | Editorial_J0b_Openings_2024.docx            | 2024-01-10T08:55:17Z | fa092856280dbddbc08d48ca996ac58eda22f1db978960c9c92ad0bd13ee197e |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:03:39Z | ecf7011bdd3fe16b6af6e35de8297ae20021dacce431a04cb692a8b363e82ca8 |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:40:40Z | 44158b15ce4d61211a6e584a77ebd4f634af5bc587f321c6de9484db0fe721ef |
|Larry Page      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:22:12Z | c4584eee4224e73097dce14321e489418cdbb5e70eee9b648b82554a034fbb80 |
|Mark Zuckerberg | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:05:35Z | 47eefdc06144552978b90231acc05903f19da7dd08429a2fe5785d9c26f5f737 |
|Barbara Walters | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:58:59Z | 42991c2abf947fe8e502e74c3149c98b3e954c619881e74f37e23c02321c109b |
|Barbara Walters | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:36:12Z | da5edbf67dc2e9b46e95dee8c2cbacf674bdea42acedabfb63c03e68242a4dcd |
|Craig Zimmerman | Editorial_J0b_Openings_2024.docx            | 2024-01-12T11:39:02Z | 6a6d260236b9d8f5a1b77a4778cced5a9162d3fe0f874e4b8c25a11b0fc69b67 |
|Kathleen Hopper | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:11:58Z | 18ffc409d889bc9e5f3d6201485a3d58b204c66f3e3a8c759fe350924733dd86 |
|Dan Rather      | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:36:20Z | 6f27b43bcbcf67b6b489ff2c3a1795ef931222abb1a24f603f382728961c6f13 |
|Peter Parket    | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:34:50Z | 09ad01734509e6edde6df79aadd7b539d8bf39d5066af987fd34eecb87974a8e |
|Ida Tarbell     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:20:56Z | c815025508a1ba3c7b68276194cac51b62526aa09c70a7157d971a84f31c3e12 |
|Bob Woodward    | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:01:44Z | d146844f2ccc728a41c597b539716e5f2aae21390742879937d668f0a2f6a934 |
|Tom Brokaw      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:10:12Z | ed66f757fc7b3f929f2414a7f5ea3823feea06f1a30d98dfd5253152eb82eabe |
|Nene Leaks      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T08:48:29Z | 04a7f37b3e4da005f46b7bd53578f9165c7fb5eeafea469a77fa4695d1aa51fc |
|Carl Bernstein  | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:56:11Z | 916e38cdf1e622c83426c94ecae63f44d4fde33ad571dc26a3d2846e8ceeaaa7 |
|Bill Gates      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:52:10Z | 2a2b1606666523699311e46ad1dc6677d710aae96ad03395136abd10a60db0d1 |
|Tyler Byers     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T09:36:13Z | 215eac85821dea858beea40e5538c89b3728a39ad84bf5c533da4585ed01e623 |

Write down those hashes in your report as indicators of compromise, however you should be aware that those are easy to manipulate. Lets also check if there are any security alerts associated with any of the downloaded files, since sometimes endpoint protection or email protection appliances are picking that up. For that we'll use the query
```kql
let file="name";
SecurityAlerts
| where description has file or indicators has file
```

There are indeed high-severity alerts for `Valdorian_Times_Editorial_Offer_Letter.docx` Those were fired at `2024-01-05T09:59:24Z` and `2024-01-08T08:20:33Z` respectively and should have started an investigation. One of the timestamps is near enough to the timestamp where Barbara Walters downloaded the document. The other time it was marked it mysteriously appeared on Tom Brokaws machine, before he downloaded the `Stop_Being_So_Broke_Get_Money_Now.docx`.

The query
```kql
let colleague =
Employees
| where name has "Tom Brokaw"
| project email_addr;
Email
| where recipient in (colleague) and link has "Valdorian_Times_Editorial_Offer_Letter"
```
showa that `newspaper_jobs@gmail[.]com` had such a file in the link field, which was received at `2024-01-08T05:16:17Z`. No we have to update our tables again.

| Name           | File                                        | when_clicked         |
|----------------|---------------------------------------------|----------------------|
|Ronnie McLovin  | Editorial_J0b_Openings_2024.docx            | 2024-01-10T08:55:07Z |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:03:21Z |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:40:16Z |
|Larry Page      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:22:10Z |
|Mark Zuckerberg | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:05:30Z |
|Barbara Walters | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:58:13Z |
|Barbara Walters | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:35:27Z |
|Craig Zimmerman | Editorial_J0b_Openings_2024.docx            | 2024-01-12T11:38:55Z |
|Kathleen Hopper | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:11:51Z |
|Dan Rather      | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:35:36Z |
|Peter Parket    | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:34:45Z |
|Ida Tarbell     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:19:58Z |
|Bob Woodward    | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:00:51Z |
|Tom Brokaw      | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-08T08:19:42Z |
|Tom Brokaw      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:09:50Z |
|Nene Leaks      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T08:48:23Z |
|Carl Bernstein  | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:55:17Z |
|Bill Gates      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:52:08Z |
|Tyler Byers     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T09:35:48Z |


| Name           | File                                        | downloaded           | sha256                                                           |
|----------------|---------------------------------------------|----------------------|------------------------------------------------------------------|
|Ronnie McLovin  | Editorial_J0b_Openings_2024.docx            | 2024-01-10T08:55:17Z | fa092856280dbddbc08d48ca996ac58eda22f1db978960c9c92ad0bd13ee197e |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:03:39Z | ecf7011bdd3fe16b6af6e35de8297ae20021dacce431a04cb692a8b363e82ca8 |
|Seymour Hersh   | Editorial_J0b_Openings_2024.docx            | 2024-01-10T09:40:40Z | 44158b15ce4d61211a6e584a77ebd4f634af5bc587f321c6de9484db0fe721ef |
|Larry Page      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:22:12Z | c4584eee4224e73097dce14321e489418cdbb5e70eee9b648b82554a034fbb80 |
|Mark Zuckerberg | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:05:35Z | 47eefdc06144552978b90231acc05903f19da7dd08429a2fe5785d9c26f5f737 |
|Barbara Walters | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:58:59Z | 42991c2abf947fe8e502e74c3149c98b3e954c619881e74f37e23c02321c109b |
|Barbara Walters | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:36:12Z | da5edbf67dc2e9b46e95dee8c2cbacf674bdea42acedabfb63c03e68242a4dcd |
|Craig Zimmerman | Editorial_J0b_Openings_2024.docx            | 2024-01-12T11:39:02Z | 6a6d260236b9d8f5a1b77a4778cced5a9162d3fe0f874e4b8c25a11b0fc69b67 |
|Kathleen Hopper | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:11:58Z | 18ffc409d889bc9e5f3d6201485a3d58b204c66f3e3a8c759fe350924733dd86 |
|Dan Rather      | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:36:20Z | 6f27b43bcbcf67b6b489ff2c3a1795ef931222abb1a24f603f382728961c6f13 |
|Peter Parket    | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:34:50Z | 09ad01734509e6edde6df79aadd7b539d8bf39d5066af987fd34eecb87974a8e |
|Ida Tarbell     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T07:20:56Z | c815025508a1ba3c7b68276194cac51b62526aa09c70a7157d971a84f31c3e12 |
|Bob Woodward    | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T10:01:44Z | d146844f2ccc728a41c597b539716e5f2aae21390742879937d668f0a2f6a934 |
|Tom Brokaw      | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-08T08:20:00Z | e49b603f55f459570f9c0c7f6c76cc6b0119f28f4617cf5c2716d132f1406c16 |
|Tom Brokaw      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:10:12Z | ed66f757fc7b3f929f2414a7f5ea3823feea06f1a30d98dfd5253152eb82eabe |
|Nene Leaks      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-03T08:48:29Z | 04a7f37b3e4da005f46b7bd53578f9165c7fb5eeafea469a77fa4695d1aa51fc |
|Carl Bernstein  | Valdorian_Times_Editorial_Offer_Letter.docx | 2024-01-05T09:56:11Z | 916e38cdf1e622c83426c94ecae63f44d4fde33ad571dc26a3d2846e8ceeaaa7 |
|Bill Gates      | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T08:52:10Z | 2a2b1606666523699311e46ad1dc6677d710aae96ad03395136abd10a60db0d1 |
|Tyler Byers     | Stop_Being_So_Broke_Get_Money_Now.docx      | 2024-01-09T09:36:13Z | 215eac85821dea858beea40e5538c89b3728a39ad84bf5c533da4585ed01e623 |

## Question 8:
For this question we can reuse the following query:
```kql
let colleague_name = "Ronnie McLovin";
let file = ".ps1";
let when_clicked = datetime(2024-01-10T08:55:17Z);
let machine_name =
Employees
| where name has colleague_name
| project hostname;
FileCreationEvents
| where hostname in (machine_name) and filename has file and timestamp >= when_clicked
| project filename,timestamp,sha256,process_name
```
Copy the timestamp of the result in the answer field. It seems that there are two files which were dropped ( `hacktivist_manifesto.ps1` and `Add-Numbers.ps1`) of which only the former is known to us from our investigation so far. Let's update the table for each of our colleagues.


| Name           | File                     | created              | sha256                                                           | process      |
|----------------|--------------------------|----------------------|------------------------------------------------------------------|--------------|
|Ronnie McLovin  | hacktivist_manifesto.ps1 | 2024-01-10T08:55:17Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Ronnie McLovin  | Add-Numbers.ps1          | 2024-01-11T13:25:58Z | d2ad5c1a02a7b37b0a6a0847ecfd28ff8d5f85514aedbcc1879d515fa46ba3f9 | explorer.exe |
|Seymour Hersh   | hacktivist_manifesto.ps1 | 2024-01-10T09:04:39Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Seymour Hersh   | hacktivist_manifesto.ps1 | 2024-01-10T09:41:37Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Seymour Hersh   | chocolateyInstall.ps1    | 2024-01-10T14:01:33Z | 01a120d3e32f92f8e14671e93045efb9f76bc0f49b5f0c20216a6634801bc088 | wuauclt.exe  |
|Larry Page      | hacktivist_manifesto.ps1 | 2024-01-03T07:22:45Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Mark Zuckerberg | hacktivist_manifesto.ps1 | 2024-01-03T07:06:20Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Barbara Walters | hacktivist_manifesto.ps1 | 2024-01-09T08:36:43Z | 42991c2abf947fe8e502e74c3149c98b3e954c619881e74f37e23c02321c109b | explorer.exe |
|Craig Zimmerman | hacktivist_manifesto.ps1 | 2024-01-12T11:39:29Z | 6a6d260236b9d8f5a1b77a4778cced5a9162d3fe0f874e4b8c25a11b0fc69b67 | explorer.exe |
|Kathleen Hopper | hacktivist_manifesto.ps1 | 2024-01-03T07:12:43Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Dan Rather      | hacktivist_manifesto.ps1 | 2024-01-05T10:37:15Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Peter Parket    | hacktivist_manifesto.ps1 | 2024-01-03T07:35:24Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Ida Tarbell     | hacktivist_manifesto.ps1 | 2024-01-03T07:21:26Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Ida Tarbell     | ContainExactly.Tests.ps1 | 2024-01-06T10:22:48Z | 8137d9fd3d42d5d1cfd35685964b49f5873c41432ac9a7e5dd73b156bb4a0afc | wuauclt.exe  |
|Bob Woodward    | hacktivist_manifesto.ps1 | 2024-01-05T10:02:25Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Tom Brokaw      | hacktivist_manifesto.ps1 | 2024-01-08T08:20:00Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Nene Leaks      | hacktivist_manifesto.ps1 | 2024-01-03T08:48:44Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Carl Bernstein  | hacktivist_manifesto.ps1 | 2024-01-05T09:57:10Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Bill Gates      | hacktivist_manifesto.ps1 | 2024-01-09T08:53:05Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Tyler Byers     | hacktivist_manifesto.ps1 | 2024-01-09T09:37:05Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |

It seems like there are several different campaigns running. For `hacktivist_manifesto.ps1`alone there are three different hashes. For the hash starting with 1c we know that it will download plink and create a shell that allows attackers to run any command. For the other to hacktivist_manifestos I am assuming it does the same.
Looking up the hash starting with 1c on VirusTotal will bring up an EICAR file, which is a test of any anti virus programs. Same seems to be for the hash starting ith 0e and 4c. 

The hacktivist_manifesto hash starting with 42 can't be found, same goes for 6a.

The `chocolateyInstall.ps1` script installs chocolatery, a software management solution. Somehow this is being distributed by Windows update, which is concerning. My understanding of Windows is not that advanced as of writing this report, so any help would be appreciated.

The powershell script `Add-Numbers` is distributed by Microsoft, as well as `ContainExactly.Tests`. Those seem to be part of the powershell examples and can be ignored. The updated table will look like this:

| Name           | File                     | created              | sha256                                                           | process      |
|----------------|--------------------------|----------------------|------------------------------------------------------------------|--------------|
|Ronnie McLovin  | hacktivist_manifesto.ps1 | 2024-01-10T08:55:17Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Seymour Hersh   | hacktivist_manifesto.ps1 | 2024-01-10T09:04:39Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Seymour Hersh   | hacktivist_manifesto.ps1 | 2024-01-10T09:41:37Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Seymour Hersh   | chocolateyInstall.ps1    | 2024-01-10T14:01:33Z | 01a120d3e32f92f8e14671e93045efb9f76bc0f49b5f0c20216a6634801bc088 | wuauclt.exe  |
|Larry Page      | hacktivist_manifesto.ps1 | 2024-01-03T07:22:45Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Mark Zuckerberg | hacktivist_manifesto.ps1 | 2024-01-03T07:06:20Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Barbara Walters | hacktivist_manifesto.ps1 | 2024-01-09T08:36:43Z | 42991c2abf947fe8e502e74c3149c98b3e954c619881e74f37e23c02321c109b | explorer.exe |
|Craig Zimmerman | hacktivist_manifesto.ps1 | 2024-01-12T11:39:29Z | 6a6d260236b9d8f5a1b77a4778cced5a9162d3fe0f874e4b8c25a11b0fc69b67 | explorer.exe |
|Kathleen Hopper | hacktivist_manifesto.ps1 | 2024-01-03T07:12:43Z | 1c3ef0407d5714037504c52f7abfa86c081fd7a021b52e2abe8a669f92413252 | explorer.exe |
|Dan Rather      | hacktivist_manifesto.ps1 | 2024-01-05T10:37:15Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Peter Parket    | hacktivist_manifesto.ps1 | 2024-01-03T07:35:24Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Ida Tarbell     | hacktivist_manifesto.ps1 | 2024-01-03T07:21:26Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Bob Woodward    | hacktivist_manifesto.ps1 | 2024-01-05T10:02:25Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Tom Brokaw      | hacktivist_manifesto.ps1 | 2024-01-08T08:20:00Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Nene Leaks      | hacktivist_manifesto.ps1 | 2024-01-03T08:48:44Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Carl Bernstein  | hacktivist_manifesto.ps1 | 2024-01-05T09:57:10Z | 4c199019661ef7ef79023e2c960617ec9a2f275ad578b1b1a027adb201c165f3 | explorer.exe |
|Bill Gates      | hacktivist_manifesto.ps1 | 2024-01-09T08:53:05Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |
|Tyler Byers     | hacktivist_manifesto.ps1 | 2024-01-09T09:37:05Z | 0e7e0e888f22b5cc83ce5f2560f9f331d89b8e02875e98ace822e074f2ee486b | explorer.exe |

By now you should have reached Level 9 if you followed my guides in order.

## Question 9
This time we should find out what the IP address was used for plink.

For that we can use the query:
```kql
let host=
Employees
| where name has "Ronnie McLovin"
|distinct hostname;
ProcessEvents
| where hostname in (host) and process_commandline has "plink"
```
Just copy the part of the process_commandline which contains an IP to the answer field.

For your information, there is also a port forwarding involved, using one of the ports commonly associated with Remote Desktop Protocol (RDP, see https://en.wikipedia.org/wiki/Remote_Desktop_Protocol).

Let's look if every variant of the `hacktivist_manifesto.ps1` executes plink. For that you can grab the unique sha256s and enter one of the names.

After a check with Barbara Walters, Dan Rather and Peter Parkets ProcessEvents we can be sure that plink is executed everywhere, therefore making the script equivalent, even though they have different hashes.

Let's build up a table for each of the plink executions and extract their Ip adresses as well as their timestamps.

| Name           | executed_plink       | ip                    | username | passord            |
|----------------|----------------------|-----------------------|----------|--------------------|
|Ronnie McLovin  | 2024-01-11T03:08:12Z | 168[.]57[.]191[.]100  | $had0w   | thruthW!llS3tUfree |
|Seymour Hersh   | 2024-01-10T09:49:17Z | 57[.]125[.]53[.]219   | $had0w   | thruthW!llS3tUfree |
|Seymour Hersh   | 2024-01-10T11:25:12Z | 152[.]88[.]81[.]202   | $had0w   | thruthW!llS3tUfree |
|Larry Page      | 2024-01-03T09:02:20Z | 168[.]57[.]191[.]100  | $had0w   | thruthW!llS3tUfree |
|Mark Zuckerberg | 2024-01-03T08:58:06Z | 194[.]148[.]124[.]175 | $had0w   | thruthW!llS3tUfree |
|Barbara Walters | 2024-01-09T10:14:12Z | 213[.]149[.]230[.]149 | $had0w   | thruthW!llS3tUfree |
|Craig Zimmerman | 2024-01-13T03:02:55Z | 57[.]125[.]53[.]219   | $had0w   | thruthW!llS3tUfree |
|Kathleen Hopper | 2024-01-03T09:07:40Z | 213[.]149[.]230[.]149 | $had0w   | thruthW!llS3tUfree |
|Dan Rather      | 2024-01-06T04:27:15Z | 136[.]130[.]190[.]181 | $had0w   | thruthW!llS3tUfree |
|Peter Parket    | 2024-01-03T09:21:16Z | 152[.]88[.]81[.]202   | $had0w   | thruthW!llS3tUfree |
|Ida Tarbell     | 2024-01-03T10:21:51Z | 193[.]224[.]154.119   | $had0w   | thruthW!llS3tUfree |
|Bob Woodward    | 2024-01-05T11:40:11Z | 25[.]105[.]41[.]53    | $had0w   | thruthW!llS3tUfree |
|Tom Brokaw      | 2024-01-09T09:09:28Z | 142[.]9[.]214[.]186   | $had0w   | thruthW!llS3tUfree |
|Nene Leaks      | 2024-01-03T11:06:17Z | 193[.]224[.]154[.]119 | $had0w   | thruthW!llS3tUfree |
|Carl Bernstein  | 2024-01-05T11:53:08Z | 213[.]149[.]230[.]149 | $had0w   | thruthW!llS3tUfree |
|Bill Gates      | 2024-01-09T11:26:01Z | 152[.]88[.]81[.]202   | $had0w   | thruthW!llS3tUfree |
|Tyler Byers     | 2024-01-09T11:05:34Z | 213[.]149[.]230[.]149 | $had0w   | thruthW!llS3tUfree |

As you can see we have 11 unique IPs, which were usd in the campaigns. Note those down in the report. They are `136[.]130[.]190[.]181`, `213[.]149[.]230[.]149`, `25[.]105[.]41[.]53`, `193[.]224[.]154[.]119`, `57[.]125[.]53[.]219`, `168[.]57[.]191[.]100`, `152[.]88[.]81[.]202`, `204[.]132[.]149[.]128`, `195[.]238[.]111[.]77`, `142[.]9[.]214[.]186` and `194[.]148[.]124[.]175`. 

The next step would be figuring out if there was any traffic coming inbound or outbound to/from those IP addresses. This will be done in the Bonus part of this writeup in order to progress the questions.

## Question 10

This time extract the username, which is always `$had0w` and enter it into the answer field.

## Question 11
Just enter the password `thruthW!llS3tUfree`

## Question 12
To answer that question you should use the query:
```kql
let host=
Employees
| where name has "Ronnie McLovin"
|distinct hostname;
ProcessEvents
| where hostname in (host) and timestamp >= datetime(<timestamp>)
```

Fill in the timestamp of the download (you can find that in question 8's answer) and look for processes. In this case the answer should be `5`. I had originally thought I should start looking after the plink has been executed, but found none. The discovery commands that can be found on Ronnies machine were `whoami`, `ipconfig`, `arp -a`, `tasklist /svc` and `net view`.

Let's repeat this for all the Employees we have found in Question 8 in the Bonus section.

## Question 13

Here we need to figure out the IP address of Ronnie. For that I will use the query
```kql
let emp =
Employees
| where name has "Ronnie McLovin"
|distinct ip_addr;
OutboundNetworkEvents
| where src_ip in (emp) and url has "fakestory.docx"
```
That way we have both his ip address and other interesting data. Copy the `src_ip` into the answer field to continue. You should also note down the timestamp (`2024-01-31T09:47:51Z`) for your report.

## Question 14
Copy the `url` field from the previous questions query in the answer field.

## Question 15
To answer that question run the quer
```kql
Employees
| where name has "Ronnie McLovin"
```
and copy the `hostname` into the answer field.

## Question 16
To answer that you can use the query
```kql
let emp =
Employees
| where name has "Ronnie McLovin"
|distinct hostname;
FileCreationEvents
| where hostname in (emp) and filename has "fakestory.docx"
```
and copy the `sha256` field into the answer field.

## Question 17
Use the previous query and copy the timestamp (`2024-01-31T09:47:51Z`).

## Question 18
To figure out the new path for the fakestory there are two paths. Either you are looking at the process_commandline, which should contain `fakestory.docx` or you can just look at all ProcessEvents created after the timestamp. I chose the latter, because I might detect other suspicious commands being run then.

```kql
let emp =
Employees
| where name has "Ronnie McLovin"
|distinct hostname;
ProcessEvents
| where hostname in (emp) and timestamp >= datetime(2024-01-31T09:47:51Z)
```
At `2024-01-31T10:26:20Z`the renaming was done. You can find the new name in the process_commandline. The move command has the follwing syntax: `move from to`.

There are some suspicious 7z commands and an exfiltration attempt, but that will be covered most likely in later questions.

## Question 19
Copy the timestamp of the move command from the previous question.

## Question 20
You can answer the question with the following query:
```kql
Email
| where sender has "ronnie_mclovin@valdoriantimes.news" and link has "OpEdFinal_to_print.docx"
```
and just copy the timestamp (`2024-01-31T11:11:12Z`).

## Question 21
This time we should figure out how many minutes elapsed between renaming and when the email was sent. For that , we'll use the `datetime_diff` function. Here is my query:
```kql
let renamed= datetime(2024-01-31T10:26:20Z);
Email
| where sender has "ronnie_mclovin@valdoriantimes.news" and link has "OpEdFinal_to_print.docx"
// use datetime diff function and substract one minute to test for one-off error
| project timestamp, diff = datetime_diff('minute', timestamp, renamed) -1
```
Copy the diff into the answer field.

## Question 22
Use the query from question 20 and copy the `subject` into the answer field.

## Question 23
Well... we already found more things happening on Ronnies machine back in question 18, so the answer should be clear.

## Question 24
Here you just need to copy the domain out of the picture. If you can't see the domain here it is defanged: `hirerecruit[.]com`

## Question 25
Here you need to use the given query in the question and replace the hostname with Ronnie's hostname. In this question you learn how to timebound a query. You can also add a count statement to make answering this question a bit easier or look at the rows returned counter.

## Question 26
You can use the query from question 18 to answer that question. I do diagree with the meme, because there was an exfiltration of business documents along with the memes at `2024-02-01T02:14:32Z`.

## Question 27
Look at `2024-01-31T11:44:58Z`and extract the third argument out of the `process_commandline`.

## Question 28
Repeat that for `2024-01-31T11:48:33Z`

## Question 29
The password is located near the end of the `proccess_commandline`.

## Question 30
If you are using the query from question 18 it is the last row of the results. Copy the whole `process_commandline`.

## Question 31
Now extract the domain out of the `process_commandline`.

## Question 32
If you look in the Bonus section, we have already searched if there were suspicious events from any device. There was no other device that had any data uploaded to the domain.

## Question 33
Just type in `wooo` and continue.

## Question 34
Just type in `shadows` to finish the module and get that badge. It is hinting that you may have only gotten them partly. Let's hope the Valdorian Times implements the suggestions.

## Section summary
The full attack chain comes into focus here. You went from email delivery to lateral movement and eventual data exfiltration. You correlated multiple artifacts: files, processes, usernames, passwords, network flows, and even organizational structure.

You also uncovered:

-    Multiple attack waves using the same payloads but slightly altered artifacts.
-    Security alerts that were missed or ignored — leading to longer dwell time.
-    Gaps in access control (SharePoint open to the internet?!), egress filtering, and user awareness.

By this point, you weren't just solving challenges — you were documenting an incident in a way that could feed into an actual IR report. That's the level we're aiming for.

# Bonus
In this section we will handle the part of the investigation, where we could sidetracked easily.

## Section 4, Question 9
In Section 4, Question 9 we figured out the ip addresses of the attackers.

We should check if there are any Inbound connections from those IP addresses.
Here is the query I used:
```kql
InboundNetworkEvents
| where has_any_ipv4(src_ip, "136.130.190.181", "213.149.230.149", "25.105.41.53", "193.224.154.119", "57.125.53.219", "168.57.191.100", "152.88.81.202", "204.132.149.128", "195.238.111.77", "142.9.214.186", "194.148.124.175")
```

And indeed there are 157 inbound events coming from those IPs. Unfortunately we are unable to see the status codes of those requests. After asking in Discord (https[:]//discord[.]com/channels/1097702760411045989/1097730279357026304/1350827542742958123), we can assume that in this case all requests came through successfully.

Extracting the distinct urls and counting the hits give us the following table:

|url                                                                                                               | count |
|------------------------------------------------------------------------------------------------------------------|-------|
|https[:]//sharepoint[.]valdoriantimes[.]news/press_release_drafts/2024/high_priority/                             |   17  |
|https[:]//sharepoint[.]valdoriantimes[.]news/employee_records/editorial_team_access_logs/2024/                    |   18  |
|https[:]//sharepoint[.]valdoriantimes[.]news/publication_logs/2024/election_day_article_publication_details[.]log |   14  |
|https[:]//sharepoint[.]valdoriantimes[.]news/HR_files/disciplinary_actions/editorial_department_2024/             |   10  |
|https[:]//sharepoint[.]valdoriantimes[.]news/management_meetings/strategy_discussions/election_coverage_2024/     |   13  |
|https[:]//sharepoint[.]valdoriantimes[.]news/confidential_drafts/reviewed/article_final_drafts/                   |   16  |
|https[:]//sharepoint[.]valdoriantimes[.]news/IT_department/server_access_records/2024/                            |   15  |
|https[:]//sharepoint[.]valdoriantimes[.]news/editorial_workflow/approvals/edictorial_process_2024[.]docx          |   15  |
|https[:]//sharepoint[.]valdoriantimes[.]news/legal_notices/internal/policy_violations_2024/                       |   17  |
|https[:]//sharepoint[.]valdoriantimes[.]news/editorial_meeting_minutes/2024/Q1/                                   |   16  |
|https[:]//valdoriantimes[.]news/search=Luffy+D[.]+Monkey                                                          |    1  |
|https[:]//valdoriantimes[.]news/search=Valdorian+Times+Strike+over+low+pay                                        |    1  |
|https[:]//valdoriantimes[.]news/search=Valdorian+Times+Intern+class+of+2024                                       |    1  |
|https[:]//valdoriantimes[.]news/search=Ronelle+Mclovin                                                            |    1  |
|https[:]//valdoriantimes[.]news/search=webmaster+%40+valdy+times                                                  |    1  |
|https[:]//valdoriantimes[.]news/search=Luffy+Monk                                                                 |    1  |

There are glaring weaknesses in the sharepoint of the Valdorian Times. It seems like it is accessible through the public internet and open to anyone. I strongly suggest implementing basic access controls to prevent leakage of internal or confidential information to the outside. Additionally the Valdorian times needs to put in place a detection that triggers, when sharepoint sites are accessed from outside the internal network.


We should also check whether the attackers attempted to authenticate as one of our users. For that I used the query
```kql
AuthenticationEvents
| where has_any_ipv4(src_ip, "136.130.190.181", "213.149.230.149", "25.105.41.53", "193.224.154.119", "57.125.53.219", "168.57.191.100", "152.88.81.202", "204.132.149.128", "195.238.111.77", "142.9.214.186", "194.148.124.175")
```
It seems that there were authentication events and sometimes they were successful. This indicated a password spraying attack. Lets see which users passwords were cracked:
```kql
let users=
AuthenticationEvents
| where has_any_ipv4(src_ip, "136.130.190.181", "213.149.230.149", "25.105.41.53", "193.224.154.119", "57.125.53.219", "168.57.191.100", "152.88.81.202", "204.132.149.128", "195.238.111.77", "142.9.214.186", "194.148.124.175")
| where result has "AuthResults.SUCCESSFUL_LOGIN"
| distinct username;
Employees
| where username in (users)
```

It seems like they were successful for `Seymour Hersh`, `Jim McKay`, `Ida Tarbell`, `Bob Woodward`, `Howard Cosell`, `Ernie Johnson`, `Carl Bernstein`, `Bob Costas` and `Stephen A. Smith`. Most of them are Sports reporter, followed by Lead Investigative Reporters. All of those users were not part of any known phishing campaign so far. `Jim McKay`,  `Howard Cosell`, `Ernie Johnson`, `Bob Costas` and `Stephen A. Smith` were victimized by other means.

Let's see if there were multiple passwords cracked by each person:
```kql
AuthenticationEvents
| where has_any_ipv4(src_ip, "136.130.190.181", "213.149.230.149", "25.105.41.53", "193.224.154.119", "57.125.53.219", "168.57.191.100", "152.88.81.202", "204.132.149.128", "195.238.111.77", "142.9.214.186", "194.148.124.175")
| where result has "AuthResults.SUCCESSFUL_LOGIN"
//use summarize to aggregate, dcount for counting only distinct elements
| summarize UniqueHashCount = dcount(password_hash) by username
```
It seems like everyone except `Ernie Johnson` had their passwords cracked multiple times. The attackers must have infiltrated the organization quite deeply for that. The Valdorian Times should enforce Multi-Factor Authentication, raise more awareness about cybersecurity (especially about phishing) and build up a more robust cybersecurity program, since there have been security alerts, which were apparently ignored.

The next step is a dangerous one and should only be done when you have explicit written consent by senior management and the customer if you are doing this for an customer. Otherwise you might land in jail and/or get terminated.

Now let's figure out if the users were compromised because of a weak password. For that we will use an external password recovery tool called hashcat. It uses password lists and rules to crack passwords. 

For an usage guide please go to the manual pages of hashcat. First identify what type of hash it could be. This can be done with `hashcat --identify hashes.txt`. After identifying the possible hash types I went through some password lists (rockyou and weakpass_4) and used several rulesets to extend the already big password lists. 

After several days of computing none was successfully cracked. That means the passwords were either salted (meaning there was a random string added to them) or there is a good password policy.  Unfortunately we are not able to

## Section 4 Question 12

For `Seymour Hersh` the commands took place after the second infection and over several hours (`2024-01-11T04:19:19Z` till `2024-01-11T07:36:18Z`). For `Larry Page` the commands took place over several hours and started two days after the infection (`2024-01-05T05:48:41Z` till `2024-01-05T07:00:22Z`). For `Mark Zuckerberg` the commands took place only a day after first infection (`2024-01-04T05:33:49Z` till `2024-01-04T08:11:21Z`). There is later a suspicious powershell command being run with a base64 encoded string, but it looks like a software update trigger. 

For `Barbara Walters` this happened inside of a 24 hr window (`2024-01-10T07:59:19Z` till `2024-01-10T10:46:27Z`). For `Craig Zimmerman` it starts almost immidiately after the manifesto was opened. For `Kathleen Hopper` it starts after about a day. 

For `Dan Rather` it starts about an hour after infection, while for `Peter Parker`it begins after about 2.5 hours. For `Ida Tarbell` it starts about 4 hours after infection. For `Bob Woodward` it starts 18 hours after infection. 

For `Tom Brokaw` it starts about 2.5 hours after infection. For `Nene Leaks` it startsabout 1.5 days after infection. For `Carl Bernstein` it takes about a day. For `Bill Gates` it took under 30 minutes. For `Tyler Byers` it took about 19 hours before the commands started.

# Final remarks

This investigation into the attack on the Valdorian Times has revealed serious gaps in both cybersecurity awareness and defensive capabilities within the organization. The breach was not an isolated event but rather a coordinated effort involving multiple attack vectors, primarily phishing and credential compromise. 

The attackers were able to infiltrate critical systems, exfiltrate sensitive data, and manipulate the publication of information, all while operating largely undetected until deeper forensic analysis was conducted.

Several key takeaways stand out

## Phishing awareness is critical
Over **20% of employees** clicked on malicious links, demonstrating a need for regular phishing training and simulated phishing exercises. The high click rate shows that attackers did not need highly sophisticated social engineering skills. Just persistence and volume were enough to get access.

## Detection without response is ineffective
Multiple security alerts were triggered, but no effective action was taken to mitigate the threats. Security teams must prioritize alert triage and escalation processes to prevent attacker dwell time. 

According to Mandiants M-Trends 2024 (https://cloud.google.com/blog/topics/threat-intelligence/m-trends-2024?hl=en) the global medialn dwell time of attackers are about 10 days. In some cases of this attack the dwell time was about 30 days - more than 2.5 times the median. 

## Access control weaknesses
Publicly accessible SharePoint documents and internal records were retrieved by external attackers. Proper access restrictions and network segmentation are needed to limit exposure.

## Credential theft and password hygiene
Nine employees had their credentials compromised, possibly through password spraying or reuse. The Valdorian Times should enforce Multi-Factor Authentication (MFA) across all accounts and implement stricter password policies.

## Lack of network egress monitoring
Attackers exfiltrated documents without triggering alarms. Implementing data loss prevention (DLP) and better outbound traffic monitoring would help detect and block unauthorized transfers.

## Persistence & Post-Exploitation Activity
Remote shells were established on nearly 20% of company devices, allowing prolonged access. Attackers moved laterally within the network and likely established multiple backdoors. The organization should perform a full forensic review of all potentially compromised systems and implement host-based monitoring to detect future persistence techniques.

# Next steps
The Valdorian Times urgently needs a structured cybersecurity program. Without proactive security investments, another breach is not a question of if, but when.

## Incident Response & Remediation
Immediately contain compromised accounts and devices, reset credentials, and review network logs for additional persistence mechanisms.

## Security Awareness Training
Conduct mandatory training on phishing and social engineering tactics.

## Implement MFA & Password Policies
Require strong, unique passwords and enforce MFA across all accounts.

## Improve Logging & Monitoring
Deploy SIEM (Security Information and Event Management) solutions that actively monitor authentication logs, process execution, and suspicious network activity.

## Harden infrastructure
Restrict external access to sensitive internal systems and apply least privilege principles.
