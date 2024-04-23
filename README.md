<h1>So you want to be a SOC Analyst? - SOC homelab</h1>

<h2>Description</h2>
A job simulation by Datacom hosted on www.forage.com.
<br />
<br />
Scenario: <br />
One of our leading tech corporation clients has fallen prey to a sophisticated cyberattack by a notorious Advanced Persistent Threat (APT) group known as APT34. The attack, believed to be sponsored by a foreign government, has left the organisation's network compromised, and valuable customer data and intellectual property has been stolen.
<br />
<br />
Objective: <br />
Help our client conduct an initial investigation into APT34 and evaluate the potential impact of the attack on the organization. As a result, you will need to produce a comprehensive report documenting your findings and outlining key recommendations for improving the organisation's cybersecurity posture.
<br />
<br />

<h2>Lab walk-through:</h2>

<!-- <p align="center"> -->

<b>Task 1- Research & information gathering:</b> <br />
Knowing that the group name is APT34, I began my research by navigating to www.crowdstrike.com and searched for APT34. The search returned with a blog about HELIX KITTEN as November 18, 2018 adversary of the month. Here I learned that the group involved with HELIX KITTEN is believed to be APT34. Prominent attack techniques are stated to be well-structured phishing emails and backdoor implants. This blog mentions that other names for APT34 can include Oilrig, Helminth, Clayside, and IRN2. <br />
<img src="https://i.imgur.com/6AmsNT3.png" width="80%" alt="blog about APT34 on crowdstrike"/>



I then found myself on a blog post by MANDIANT about various APTs. MANDIANT mentions that APT34 is suspected to have ties to Iran with a broad targeting of a variety of industries. Finance, energy, telecommunications, chemical, government are such industries listed. <br /><img src="https://i.imgur.com/je5tmxL.png" width="80%" alt="blog about APT34 on MANDIANT"/>



Another blog on www.darkreading.com goes into some detail about Oilrig's custom backdoor malware which take advantage of shared email/cloud storage accounts as a way to gain information and execute files. <br />
<img src="https://i.imgur.com/YgO8B52.png" width="80%" alt="blog about APT34 on DARKREADING"/>


Now that I knew a bit more about out attack group, I decided to search for more information from the MITRE ATT&CK framework. In this framwork, I learned that Oilrig and APT34 are confidently labeled as groups with high overlap of activity and have been active since 2014. The framework also confirms that it is highly suspected that this group is associated woth an Iranian threat group. Looking into the attack techniques used, spear phishing and masking malicious executables behind emails and attatchments seem like prominent techniques used by APT34. <br />
<img src="https://i.imgur.com/s17RmU6.png" width="80%" alt="MITRE ATT&CK framework on Oilrig"/> <br />
<img src="https://i.imgur.com/yBkuHrO.png" width="80%" alt="MITRE ATT&CK framework on Oilrig"/> <br />
<img src="https://i.imgur.com/AOKURkR.png" width="80%" alt="MITRE ATT&CK framework on Oilrig"/> <br />



Next, I navigated to the Defenses tab in the framework. Knowing that ATP34 primarily uses social engineering and executables, I looked for defensive techniques for these TTPs. <br />
<img src="https://i.imgur.com/iWCN855.png" width="80%" alt="MITRE ATT&CK framework defenses"/> <br />
<img src="https://i.imgur.com/RFpSWlV.png" width="80%" alt="MITRE ATT&CK framework defenses"/> <br />
<img src="https://i.imgur.com/yQ4cFPr.png" width="80%" alt="MITRE ATT&CK framework defenses"/> <br />


<br />
<br />
Questions:
<br />

1. What is their history? <br />
   APT34 is a group also known as OilRig, Helix Kitten, Cobalt Gypsy, Crambus, and MuddyWater. This group has been active since 2014 and is known for state-sponsored cyber espionage based out of the Middle East. <br />

2. Which nation/state are they associated with? <br />
   APT34 is believed to be associated with Iran. <br />

3. Do they target specific industries? <br />
  APT34 is known for targeting various industries including finance, telecommunications, and energy. <br />
  
4. What are their motives? <br />
   APT3 is suspected to be primarily about carrying out reconnaissance to obtain benefcial information for any Iranian efforts. <br />
   
5. What are the TTPs they use to conduct their attacks? <br />
   APT34's known TTPs include spear phishing and malware delivery via custom malware such as OilCheck and OilBooster which both have their own methods of getting access to shared accounts in Microsoft systems. </ br>

7. What security measures could the client implement to defend against cyberattacks conducted by this APT? <br />
   To mitigate against these type of attacks, one can incorporate measures such as: <br />
   - Employee training which can help mitigate against social engineering techniques including spear phishing. <br />
   - Implementing antivirus solutions to better protect end points can help stop infiltration of systems via malware infections. <br />
   - Implementing code signing will stop unsigned, unauthorized code from being execuuted. <br />
   - Having an incident response plan will help with the speed and efficiency in which incidents are handled.

<br />

Sources: <br />
- Elizabeth Montalbano, C. W. (2023, December 14). Iran-linked “Oilrig” cyberattackers target Israel’s critical infrastructure, over & over. Dark Reading. https://www.darkreading.com/ics-ot-security/iran-oilrig-cyberattackers-target-israel-critical-infrastructure <br />

- Mandiant. (n.d.). Advanced persistent threat (APT) Groups & Threat Actors. https://www.mandiant.com/resources/insights/apt-groups <br />

- Meyers, A. (2018, November 27). Helix kitten: Threat actor profile: Crowdstrike. crowdstrike.com. https://www.crowdstrike.com/blog/meet-crowdstrikes-adversary-of-the-month-for-november-helix-kitten/ <br />

- Mitigations - ICS | MITRE ATT&CK®. (n.d.). https://attack.mitre.org/mitigations/ics/ <br />

- Oilrig. OilRig, COBALT GYPSY, IRN2, APT34, Helix Kitten, Evasive Serpens, Group G0049 | MITRE ATT&CK®. (n.d.). https://attack.mitre.org/groups/G0049/ <br />
