# Lab Report 3 - Jacob Roner
---

## Researching Commands - grep

---

## 1. Case Insensitive grep search: grep -i

  ```
  $ grep -i 'CAPPS' ~/stringsearch-data/technical/911report/chapter-1.txt
  ```
  **Note: In the termnial, the instances of 'CAPPS' are bolded and colored**
  ```
  When he checked in for his flight to Boston, Atta was selected by a computerized prescreening system known as CAPPS (Computer Assisted Passenger Prescreening System), created to identify passengers who should be subject to special security measures. Under security rules in place at the time, the only consequence of Atta's selection by **CAPPS** was that his checked bags were held off the plane until it was confirmed that he had boarded the aircraft. This did not hinder Atta's plans.
    While Atta had been selected by CAPPS in Portland, three members of his hijacking team-Suqami, Wail al Shehri, and Waleed al Shehri-were selected in Boston. Their selection affected only the handling of their checked bags, not their screening at the checkpoint. All five men cleared the checkpoint and made their way to the gate for American 11. Atta, Omari, and Suqami took their seats in business class (seats 8D, 8G, and 10B, respectively). The Shehri brothers had adjacent seats in row 2 (Wail in 2A, Waleed in 2B), in the firstclass cabin. They boarded American 11 between 7:31 and 7:40. The aircraft pushed back from the gate at 7:40.
    Shehhi and his team, none of whom had been selected by CAPPS, boarded United 175 between 7:23 and 7:28 (Banihammad in 2A, Shehri in 2B, Shehhi in 6C, Hamza al Ghamdi in 9C, and Ahmed al Ghamdi in 9D). Their aircraft pushed back from the gate just before 8:00.
    Hani Hanjour, Khalid al Mihdhar, and Majed Moqed were flagged by CAPPS. The Hazmi brothers were also selected for extra scrutiny by the airline's customer service representative at the check-in counter. He did so because one of the brothers did not have photo identification nor could he understand English, and because the agent found both of the passengers to be suspicious. The only consequence of their selection was that their checked bags were held off the plane until it was confirmed that they had boarded the aircraft.
    When the local civil aviation security office of the Federal Aviation Administration (FAA) later investigated these security screening operations, the screeners recalled nothing out of the ordinary. They could not recall that any of the passengers they screened were CAPPS selectees. We asked a screening expert to review the videotape of the hand-wanding, and he found the quality of the screener's work to have been "marginal at best." The screener should have "resolved" what set off the alarm; and in the case of both Moqed and Hazmi, it was clear that he did not.
    Newark: United 93. Between 7:03 and 7:39, Saeed al Ghamdi, Ahmed al Nami, Ahmad al Haznawi, and Ziad Jarrah checked in at the United Airlines ticket counter for Flight 93, going to Los Angeles. Two checked bags; two did not. Haznawi was selected by CAPPS. His checked bag was screened for explosives and then loaded on the plane.
```
- In this example, grep -i is used to find every instance of 'CAPPS' in the chapter-1.txt file. The -i command returned any lines that had 'CAPPS' regardless of case, as the command searches for case-isensitive appearences of the given input.
- This can be extremely helpful when looking for an instance of a word or letters that might be capitalized or not
- Found and taken from : [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)


 ```
  $ grep -i 'Lawyer' ~/stringsearch-data/technical/government/Media/5_Legal_Groups.txt
 ```
 **Note: In the termnial, the instances of 'Lawyer' are bolded and colored**
 
 ```
 from Utah lawyers and foundations, was the first joint fund-raising
 the Multi-Cultural Legal Center, the Senior Lawyer Volunteer
 ```
 -This example shows how the word lawyer can be searched in order to find two examples of titles in which only one has the word 'Lawyer' capitalized.
 - Found and taken from : [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-  in-linux-unix/)
 
 
 
 ## 2. Look for all files in the current directory: grep -r
 
 ```
 grep -r 'conversations' ~/stringsearch-data/technical
 ```
 **Note: In the termnial, the instances of 'conversations' are bolded and colored**
 
 ```
 /home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-1.txt:    In their testimony and in other public accounts, NORAD officials also stated that the Langley fighters were scrambled to respond to the notifications about American 77,178 United 93, or both. These statements were incorrect as well. The fighters were scrambled because of the report that American 11 was heading south, as is clear not just from taped conversations at NEADS but also from taped conversations at FAA centers; contemporaneous logs compiled at NEADS, Continental Region headquarters, and NORAD; and other records. Yet this response to a phantom aircraft was not recounted in a single public timeline or statement issued by the FAA or Department of Defense. The inaccurate accounts created the impression that the Langley scramble was a logical response to an actual hijacked aircraft.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.4.txt:                intended target of the attack). On KSM/Yousef phone conversations, see Intelligence
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.4.txt:                phone conversations with Yousef were social in nature, but that Yousef did discuss
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.4.txt:            31. Even before learning of Abdullah's alleged jailhouse conversations, we attempted
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-3.txt:                signals environment. Its analysts listen to conversations between foreigners not
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-3.txt:                conversations. But since the tribals seemed to know where Bin Ladin was or would be,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-5.txt:                had numerous telephone conversations during which Yousef discussed his progress and
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-5.txt:                speaking only in Arabic to conceal the content of their conversations. 87 When the
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-6.txt:                will need to make some decisions NOW." He told us he held several conversations with
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-6.txt:                be very costly. This was the context for earlier conversations, when in March Tenet
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-8.txt:                Moussaoui in two passing hallway conversations but only in the context that he might
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                They had two brief conversations. In the first, the senior lobby chief gave the
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1472-684X-2-1.txt:        patients and their families, conversations about care must
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1472-684X-2-1.txt:        avoid difficult, seemingly time-intensive conversations
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1472-684X-2-1.txt:        postpone or avoid potentially goal-defining conversations
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1472-684X-2-1.txt:        postponing conversations regarding goals of care may
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/Progress_report.txt:Diversity in the Legal Services Community conversations took
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/Progress_report.txt:Association (NLADA), LSC launched a series of conversations on
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/Progress_report.txt:diversity in 2001. Over the year, eight separate conversations on
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/State_Planning_Report.txt:Keeping alive the conversations begun in 1998 as a
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/Strategic_report.txt:LSC's 2001 national conversations on diversity.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/Strategic_report.txt:candid conversations and exercises on fostering inclusion,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/diversity_priorities.txt:reports issued following those conversations.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/diversity_priorities.txt:difficult conversations.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/Letter_Walkeraug17let.txt:conversations with the Vice President«s representatives. However,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/Letter_Walkeraug17let.txt:in these conversations, the Vice President«s representatives have
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/May1998_ai98068.txt:practices being employed. After initial conversations with a number
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/Oct15-2001_d0224.txt:include a violator in sensitive conversations. One participant
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/Oct15-2001_d0224.txt:relied primarily on regular mail and telephone conversations to
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/ai9868.txt:practices being employed. After initial conversations with a number
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/d01186g.txt:conversations); or other formats so long as the documents are
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/pe1019.txt:such as Gerald A. Office in these conversations but did not say we
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/plos/journal.pbio.0020419.txt:        good theory of brain function. We know of these conversations, as the probing of Marr by
 ```
- In this example, grep -r is used to search technical and all its subdirecories for files that contain the word given in the command line input. The output is every file that contains the word "conversation."
- This can be helpful when trying to find a set of files in a larger directory that have a specific keyword.
- Found and taken from : [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)

```
$ grep -r '911' ~/stringsearch-data/technical
```
**Note: In the termnial, the instances of '911' are bolded and colored**

```
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                received by civilians in the towers based on (1) calls to NYPD 911 from or
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                September 11, 2001 (hereafter "Commission analysis of 911/PAPD calls"). Everyone
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                Commission analysis of 911/PAPD calls; Civilian interview 17 (May 11, 2004);
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                analysis of 911/PAPD calls; Port Authority transcripts of recorded Port Authority
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            32. Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                2004); Civilian interview 14 (Apr. 7, 2004); Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                7 (Mar. 22, 2004); Commission analysis of 911/PAPD calls. For some emergency
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            36. For callers being disconnected, see Commission analysis of 911/PAPD calls. For
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                and terminations, see Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                callers, see Commission analysis of 911/PAPD calls. For standard operating
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                911/PAPD calls. For operators departing from protocol, see ibid.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            40. Commission analysis of 911/PAPD calls; Port Authority transcripts of recorded
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            43. For smoke rising and its effect, see Commission analysis of 911/PAPD calls. For
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                911/PAPD calls; Port Authority transcripts of recorded Port Authority calls and
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            67. Commission analysis of 911/PAPD calls; NYPD recordings, City Wide 1, Special
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                interview 4 (Mar. 16, 2004); Commission analysis of 911/PAPD calls. For events in
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                (Mar. 16, 2004); Civilian interview 3 (May 4, 2004); Commission analysis of 911/PAPD
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            87. For conditions in the 90s and 100s, see Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                floors, see Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            88. For the callers, see Commission analysis of 911/PAPD calls. There are many
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                from floors higher up as well. It is not known, however, whether 911 callers had a
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            89. Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                2004); Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            91. Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                Commission analysis of 911/PAPD calls.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            96. Commission analysis of 911/PAPD calls. It is not clear whether callers from below
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                simply calling to seek advice. In any case, the 911 operators and FDNY dispatchers
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            150. For the 911 call, see Commission analysis of 911/PAPD calls. For the inaccurate
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:            157. For information about 911 calls, see Commission analysis of 911/PAPD calls. For
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-13.5.txt:                www.whitehouse.gov/news/releases/2001/09/20010911-16.html).
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                Twin Towers. The 911 emergency call system was overwhelmed. The general evacuation
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                (which was not monitored by a dispatcher).17 The NYPD also supervised the city's 911
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                of emergency response. When a 911 call concerned a fire, it was transferred to FDNY
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                which had a center in each of the five boroughs. All 911 calls concerning fire
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            Civilians, Fire Safety Personnel, and 911 Calls
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            Within minutes, New York City's 911 system was flooded with eyewitness accounts of
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                had been advised to do in fire drills. Many called 911.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            The 911 system was not equipped to handle the enormous volume of calls it received.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                Some callers were unable to connect with 911 operators, receiving an "all circuits
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                emergencies to be transferred from 911 operators to FDNY dispatch operators in the
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            The 911 operators and FDNY dispatchers had no information about either the location
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            These critical decisions were not conveyed to 911 operators or to FDNY dispatchers.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                as advised by 911 operators. Others simply continued to work or delayed to collect
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            The 911 operators and FDNY dispatchers were not advised that rooftop rescues were not
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            Civilians, Fire Safety Personnel, and 911 Calls
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                calling 911 for direction.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            The 911 system remained plagued by the operators' lack of awareness of what was
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            In addition, the 911 system struggled with the volume of calls and rigid standard
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                impact zone and who stopped on the 31st floor in order to call 911, I told them when
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            Very few 911 calls were received from floors below the impact, but at least one
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                oxygen was running out. The last known 911 call from this location came at
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                repeated references in calls to 911 to having heard "announcements" to go down the
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            Those who called 911 from floors below the impact were generally advised to remain in
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                fire was above or below them, specifically asking if 911 operators had any
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                could only have come via 911. These workers were not trapped, yet unlike most
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                that 100 people were reported via 911 to be trapped on the 105th floor of the North
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            Interaction of 911 Calls and NYPD Operations.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            At 9:37, a civilian on the 106th floor of the South Tower reported to a 911 operator
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                conveyed inaccurately by the 911 operator to an NYPD dispatcher. The dispatcher
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                further confused the substance of the 911 call by telling NYPD officers at the WTC
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                complex that "the 106th floor is crumbling" at 9:52, 15 minutes after the 911 call
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:            The 911 calls placed from most locations in the North Tower grew increasingly
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                they will encounter during descent. Impact of 911 Calls on Evacuation. The NYPD's
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                911 operators and FDNY dispatch were not adequately integrated into the emergency
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                response. In several ways, the 911 system was not ready to cope with a major
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                911 operators and FDNY dispatchers, who for the next hour often continued to advise
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                impact zones. Nor were 911 operators or FDNY dispatchers advised that rooftop
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                upper floors of the South Tower who called 911 and were not told that their only
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                disasters, it is important to integrate those taking 911 calls into the emergency
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-9.txt:                receive and combine information from all first responders-including 911 operators.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2121-3-2.txt:        accession number Q09118) [ 2 ] was amplified by PCR using
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2156-4-9.txt:          other predicted F-box containing genes (CG4911, CG3428,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2164-2-7.txt:          and AI591193) that were identical at the 
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2164-3-15.txt:          flanked by inverted repeats, specifically, Us (1911 bp,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2199-3-12.txt:          on 911 cells [ 26 ] . Viral particles were determined by
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2199-4-4.txt:          on 911 cells [ 19 ] . Viral particles were determined by
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/1471-2407-2-17.txt:          by end point cytopathogenic effect (CPE) assay on 911
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/gb-2001-2-8-research0030.txt:          aat sequences are AY039113,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/gb-2002-3-12-research0080.txt:          AF132565-AF132567, AF160911-AF160913,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/gb-2002-3-12-research0080.txt:          AY070911-AY070913, AY071674,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/gb-2003-4-4-r24.txt:        TNF locus (MIM *191160) has been
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/gb-2003-4-4-r26.txt:          AW589050-AW589115, AW735503-AW735730, AW782981-AW783662,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/gb-2003-4-5-r34.txt:          = 0.911 and 0.910 using average linkage or complete
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/biomed/rr196.txt:          numbers MA3-91 and MA3-911; Affinity BioReagents, Inc.,
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/State_Planning_Special_Report.txt:19881989199019911992199319941995199619971998199920002001
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/About_LSC/commission_report.txt:S16911 (Oct. 17, 1986) (statement of Sen. Kennedy); March Comments
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Env_Prot_Agen/tech_adden.txt:children, 911
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/Oct15-1999_gg00026t.txt:512-9110, and for information regarding GAO's work on GSA, please
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:Commission's Rules To Ensure Compatibility with Enhanced 911
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:Emergency Calling Systems (Wireless E911 Rules)
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:Rules To Ensure Compatibility with Enhanced 911 Emergency Calling
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:Systems (Wireless E911 Rules)" (FCC-96-264). We received the rule
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:requirements for basic wireless 911 services and establishes a
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:framework for improving wireless 911 services. The Commission
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:For basic wireless 911 services, the Order requires covered
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:carriers to transmit to public safety personnel all 911 calls
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:transmitting wireless 911 calls made by hearing-or speech-impaired
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:The Order also requires covered carriers to offer certain 911
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:cell site receiving a 911 call. Within the next 5 years, the Order
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:incorporated into enhanced 911 systems in the future.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:OF THE COMMISSION'S RULES TO ENSURE COMPATIBILITY WITH ENHANCED 911
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:EMERGENCY CALLING SYSTEMS (WIRELESS E911 RULES) (FCC-96-264)
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:of 911 and enhanced 911 services through certain technologies.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:Enhanced 911 Emergency Calling Systems, CC Docket No. 94102, 9 FCC
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:analysis describes how this Report and Order will make 911 and
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:enhanced 911 services for users of wireless telephones more widely
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Gen_Account_Office/og96034.txt:comments and reply comments regarding the wireless 911 issues. The
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Media/Law-school_grads.txt:Denver and $24,911 elsewhere in the state.
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Media/Marylands_Legal_Aid.txt:founded in 1911 and today recognized nationally for its leadership
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/plos/pmed.0020034.txt:        for hay fever in 1911, the studies on hay fever prevalence by Ratner and Silverman in New
```
- In this example, grep -r is used to pull every path that contains a file with the string '911' in it.
- This can be helpful when trying to find a set of files in a larger directory that have a specific keyword.
- Found and taken from : [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)


## 3. Number of times a string appears: grep -c

```
$ grep -c 'CAPPS' ~/stringsearch-data/technical/911report/chapter-1.txt
```
```
6
```
- In this example, the grep command -c is used to count how many times the string 'CAPPS' appears in the given file. 
- This can be extremely helpful when trying to track and record the appearences of certain strings in relation to other files.
- Found and taken from : [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)

```
grep -c 'Lawyer' ~/stringsearch-data/technical/government/Media/5_Legal_Groups.txt
```
```
1
```
- In this example, the grep command -c is used to count how many times the string 'Lawyers' appears in the given file. 
- This can be extremely helpful when trying to track and record the appearences of certain strings in relation to other files.
- Found and taken from : [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)


## 4. Display file name only: grep -l

```
$ grep -l 'Lawyer' ~/stringsearch-data/technical/government/Media/
```
```
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/government/Media/5_Legal_Groups.txt
```
- In this example, grep -l is used to return all the files in a directory that contain the word 'Lawyer.' This can be helpful for situations in which you want to keep the terminal simple and clear, as the command only returns the name of the file and not the lines.
- Found and taken from : [https://www.geeksforgeeks.org/grep-command-in-unixlinux/#](https://www.geeksforgeeks.org/grep-command-in-unixlinux/#)

```
$ grep -l 'CAPPS' ~/stringsearch-data/technical/911report/
```
```
/home/linux/ieng6/cs15lsp23/cs15lsp23mw/stringsearch-data/technical/911report/chapter-1.txt
```
- In this example, grep -l is used to return all the files in a directory that contain the word 'CAPPS.' This can be helpful for situations in which you want to keep the terminal simple and clear, as the command only returns the name of the file and not the lines.
- Found and taken from : [https://www.geeksforgeeks.org/grep-command-in-unixlinux/#](https://www.geeksforgeeks.org/grep-command-in-unixlinux/#)


## LINK FOR SOURCES:
- [https://www.geeksforgeeks.org/grep-command-in-unixlinux/#](https://www.geeksforgeeks.org/grep-command-in-unixlinux/#)
- [https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)




