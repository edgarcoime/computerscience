# NotPetya Ransomware
## Executive Summary
## Introduction
The evolution of ransomware can be traced back to its early, simplistic forms with the 1989 AIDS Trojan also known as PS Cyborg. Where biologist Joseph L. Popp sent 20,000 infected physical diskettes to attendees of the WHO's international AIDS conference. This trojan after 90 seconds hid directories and encrypted the names of the files of the customer's computer. To regain access the user would have to send $189 to post office box in Panama. Today, ransomware no longer needs a disc or a physical device, rather all it needs is a simple click through an unverified link or attachment in a user's email. After this seemingly innocent click the user's computer is then compromised.

One of the largest forms of ransomware ever released was called NotPetya. Almost movie-like in scale NotPetya was an infamous ransomware released in June 2017. fit would first spread through a single computer then aggregate towards the rest of the computers with in a network rendering everyone of the systems crippled and unrecoverable. The virus first spread in Ukraine through a company which became ground zero and quickly spread worldwide affecting millions of people and costing upwards of billions of dollars worth of damages. We will be examining the importance of this cyberattack and how it has shaped the current world of cybersecurity and changed how nations and organizations view ransomware and security in this modern age.
## Body
### Historical Analysis
Ransomware first started off simple such as the first one... As the technological age continued with their advancement of technology. The malicious pieces of technology evolved to keep up with the times especially ransomware viruses. 

A year before the release of NotPetya another ransomware named WannaCry was the first that spread like waves and put viruses in the global radar. It did this and that and provided. This virus was would be the stepping stone that would set the foundation for the later virus that would cripple the country of Ukrain only a year later. 

But before diving into a detailed analysis of how the NotPetya ransomware expanded upon the stepping stones of Wanna cry. It is important to establish the geopolitical context surrounding the conflict between Ukraine and Russia. 

Ukraine and Russia's relationship was destroyed through the annexation of Crimea in 2014. Engaged in an ongoing war ever since then the blatant annexation of Crimea to the dismay of the united nations eventually led up to the dispute of the Ukrainian region of Donbass. Ever since the dawn of the conflict in 2014 over 14,000 Ukrainians have died in the conflict. Characterizing their relationship as fraught would be an understatement. As tensions between the two countries eventually led to a boiling point with Russia launching their cyberattack against Ukraine through the deployment of the NotPetya ransomware. This historical context is necessary to understanding the motivations behind the cyberattack.
### Technical Analysis
n NotPetya overwrites the Master Boot record of the system with a malicious payload. It then attempts to force a "Hard Error" within windows to reboot the system. If that fails it then tries to create tasks on the windows system to initiate a reboot after a set delay. Upon reboot, the code inserted into the MBR executes and encrypts user files on the system. NotPetya ingeniously exploits two major security vulnerabilities which were EternalBlue (MS017-010) and Mimikatz. 

EternalBlue is an exploit created by the NSA which took advantage of a vulnerability in the Windows Server Message Block (SMB) protocol. This exploit allowed attackers to execute arbitrary code in the target system without requiring authentication as well as gain access to other computers connected to the same network. Even though Microsoft released a security patch for the vulnerability in March 2017 many computers around the world had not yet been patched. As demonstrated by the WANNACRY cyberattack that happened a month prior to NotPetya that affected over 150 countries costing millions of dollars in damages.

Mimikatz was an older invention by a french security researcher in 2011 which was created as a proof of concept to demonstrate to Microsoft how its authentication protocols were vulnerable to attack. Mimikatz is an open-source application that allows users to view and save authentication credentials such as passwords within ram. So if hackers could gain access to guest or limited access to a computer they could then use Mimikatz to find other users' passwords and hack into other computers using those credentials. 

These exploits combined were the perfect recipes of disaster for NotPetya. By taking advantage of these two vulnerabilities the virus could use the EternalBlue vulnerability to infect computers that aren't patched then grab information using Mimikatz from patched computers. This meant that patched and unpatched systems were not safe from the attacks. Attacking all the systems connected to the same network allowed NotPetya to spread rapidly. All it needed was an entry point to start. 

MEDOC was the perfect entry point for the virus as it was the defacto Ukrainian tax preparation program. It had approximately 400,000 customers across Ukraine and represented about 90% of the country's domestic firms. Earlier in the spring of 2017 another cyberattack targeted the company and hijacked their update servers. They then used these servers as a backdoor to hundreds of thousands of Ukrainian households and businesses through the MEDOC software update, following which the ransomware attack began to appear. Spreading first through the MEDOC software, then all of Ukraine, and finally the rest of the world.
### Impact Analysis
NotPetya was a global crisis that affected countries all across the globe, within the day spreading to France, Germany, Italy, Poland, and the United States. But the majority of the infections were targeted in Ukraine where 80% of the reported attacks were located. The attack disrupted the operations of critical infrastructure such as Electrical grids, banking, and telecommunications systems. The founder of the Oktava Cyber Protection company, Oleksandr Kardakov, stressed the impact of the virus stating that the attack stopped a third of Ukraine's economy for three days. Which resulted in losses of more than $400 million dollars. It was clear that this was a targeted attack aiming to cripple Ukraine's critical infrastructure. 

As NotPetya infiltrated Ukraine and began to spread, its footprint grew so quickly that it even attacked Global companies infrastructures that were connected to Ukraine such as Maersk, Marck, and Saint Gobain. These multinational companies suffered immense losses: $300 million from the global shipping company Maersk, $870 million lost from the Pharmaceutical giant Merck, $400 million to FedEx's European subsidiary TNT express. 

It was clear that NotPetya had carved its mark in history as one of, if not, the most costly cyberattack in history. With former Homeland security cybersecurity expert, Tom Bossert, even estimating the total damages across the globe to be around $10 billion dollars. This attack highlighted the need for a change globally in the cybersecurity sector to implement better best practices.
### Responses and Changes
Cybersecurity sectors of government around the world were quick to respond trying to contain the virus as much as they could. Europol said that it was aware of and urgently responding to reports of cyberattack in the member states of the European Union. The United States Department of Homeland Security was actively involved with coordinating with international and local partners to prevent any further damage. In response to this attack a United States congressman even wrote a letter to the NSA demanding that the agency collaborate more actively with technological companies to notify them of future and current software vulnerabilities. Instead of witholding information like EternalBlue, sharing potential vulnerabilities with technology companies would help prevent future attacks based on malware created by the NSA.

In the aftermath of such a devastating attack directed not only at Ukraine but across the whole globe. Organizations around the globe, across all sectors of Technology recognized the pressing need for proactive cybersecurity measures to increase their overall resilience against a cyberattack. Some Key lessons from the attack include but are not limited to:

Patch Management: NotPetya exploited a known vulnerability in MeDoc software mainly through EternalBlue which Microsoft released a security patch just a couples month before the attack. Organizations must prioritize timely software updates and prioritize security patches to prevent similar attacks from occurring again. 

Defense-in-Depth: This incident demonstrated the flaws of solely relying on perimeter defenses instead of multi-layered security measures. A traditional security system focuses on defending the network's outer boundaries such as firewalls and NotPetya easily bypassed this type of defense system. Multi-layered security measures involve dividing networks into smaller more isolated segments (Network Segmentation) that limit the spread of malware if one segment is compromised. As well as Zero-trust models that assume a threat already exists both inside and outside the network which required continuous verification of users and devices. 

Cybersecurity Awareness: Training and Education of employees are crucial elements to any cybersecurity strategy. Many cyberattacks including NotPetya involve human interaction which exploit human weaknesses. At times the weakest link to any cybersecurity strategy are employees who can fall victim to phishing scams or opening malicious attachments. Companies need to recognize be proactive with educating their employees with best practices to avoid falling victim to such schemes. This is vitally important as technology continues to evolve because as a result more nefarious cyberattacks are bound to surface. 

Incident Response and Recovery: NotPetya also highlighted the importance of an immediate response and strong recovery strategy for any organization. Organizations need to plan and teach employees the steps they should take when a cyber attack occurs. This includes identifying the attack, containing the threat, eradicating the malware, and recovering affected systems. Therefore the only way to effectively train the personnel is through regular drills and simulations. By being prepared organizations can respond swiftly to minimize damage. 

International Cooperation: This global security attack displayed how Cyber threats do not respect national borders. Cyberwarfare against another country's critical infrastructure even shutting their parts of their economy is no longer an abstract concept from a Science Fiction movie. It is important that everyone realizes the global nature of cyber threats. Therefore increased international cooperation and information sharing between governments and private entities are essential to combating and containing global cyber threats. 

The NotPetya cyber attack was a wakeup call for many governments, organizations and individuals worldwide. It underscored the importance of cybersecurity preparedness and the need to implement proper procedures to increase resilience against future threats. 
### Ethical and Political Considerations
The NotPetya attack is often attributed towards Russian state sponsored malicious actors. With this attack occuring against the backdrop of ongoing conflict between Russia and Ukraine. 

Even the nature of the mischaracterized ransomware shows malicious intent. NotPetya like all other ransomware encrypts files and demanded a ransom. However its purpose was far more nefarious as it was not for financial gain. With Notfpetya there was no key that existed to decrypt the users files and even the attacker's email address had been shutdown; so there was no way to communicate to recover data. It was clear that the virus was built for the purpose of maximum destruction.

This was clearly an act of Cyberwarfare and no doubt Ukraine was the primary target of the cyberattack. Not only did NotPetya on the eve of June 27, 2017 which is the Ukrainian holiday constitution day. It also specifically shutdown critical sectors of infrastructure including disruptions to the Chernobyl Nuclear power plant which emphasized the far-reaching consequences of this cyber assault. 

This attack marked a turning point in the realm of cyberwarfare as it reshaped governments' understanding of destructive cyber attacks. It blurred the lines between traditional ransomware and state-sponsored cyber operations. The international sentiment towards the NotPetya cyberattack was overwhelmingly negative. With the US government and the UK denouncing the attack and even emphasizing the need to cooperate and build more robust defence against such threats. In response to the attack many countries asked for clearer mechanisms and guidelines to attributes cyberattacks to state actors. They even increased their overall spending towards cybersecurity infrastructure and training towards new agencies focused on cyber defence. The reactions to the NotPetya attack highlighted the growing recognition of cyber threats as a critical component of national security. 
### Counterarguments and debates
While many agree on NotPetya's consequences locally in Ukraine as well as worldwide many still have differing perspectives with regards to attribution or association with a nation or the effectiveness of security measures against such widespread attacks. 

One of the most contentious issues surrounding the Cyberattack is the question of attribution. Proving and determining the true origin of cyberattacks is difficult and has many challenges. With the anonymous nature of the digital landscape as well as the many workarounds to deceive and misdirect attribution especially in the world wide web. It is very difficult to link attack to a nation-state. There is also the debate of if attribution has been proven nations could use cyberattacks as justification for more extreme retaliatory measures. This could be a very dangerous path for everyone in the world if this dynamic fosters an environment if mistrust which would further strain global relations.

Another critical area for debate is based on the effectiveness of security measures in the first place. Many critics argue that organizations often adopt a more reactive approach to cybersecurity. Countermeasures are only set in place after an attack has been launched and the damage has already done rather than proactively investing in cybersecurity. Proactive strategy advocates push for more employee training, emphasizing the importance of regular updates, and more advanced detection technologies. The NotPetya incident has only raised concerns about the efficiency of such measures, questioning whether they genuinely lead to improved security or how they just create a false sense of safety. 
## Conclusion
The NotPetya cyberattack on July 2017 is a constant reminder to the world about the dangerous and evolving landscape of cyberthreats and the threat it can bring to nations and organizations around the world. A historical analysis of the origins of NotPetya demonstrated how strained relationships and geopolitics can lead to nations using cyberwarfare. Which can result to malicious state backed actors exploiting vulnerabilities to cripple systems and infect even more users through their own networks. The impact this cyberattack had also went beyond just immediate financial loss as it undermined and questioned the cybersecurity practices of organizations across various industries around the whole world. 

As a response nations and organizations had to act and adapt quickly. Prompting significant advancements in operational security measures to increase their resilience to further cyberthreats in the future. Nations also started to understand how important cyber security was. As well as the ethical and political ramifications it has when linked towards the growing unstable relationship between Russia and Ukraine. 

Overall the NotPetya ransomware has left a permanent record revealing the far reaching consequences of cyberattacks of this nature. As technology continues to grow and and become more sophisticated, the threats will grow along with those same advancements. This is the beginning of a new age of warfare where attacking an enemy nation does not have to be physical but digital as well. Therefore our defensive measures against such future state-backed attacks or otherwise must also evolve accordingly. By learning from past incidents and preparing for the future we can better combat the challenges that lie ahead in the realm of cybersecurity.

Therefore our defensive measures against such attacks must also evolve accordingly. NotPetya has taught us that there is no such thing as being too prepared. 


As the threat of ransomware continues to loom in the foreseeable future 

impact on the world has left a permanent record in the 

NotPetya's impact on Ukraine's infrastructure revealed the far reaching consequences of cyberattacks of this nature. This is a beginning of a new age of warfare, attacking an enemy nation not only physically but digitally as well. This was one the most terryfying and most costly act of cyberattack to have ever occurred


In response to the attack 



In conclusion, the NotPetya malware incident is a reminder of the constantly evolving landscape of cyber threats and the profound consequences they can have on global systems and Infrastructure. We analyzed the historical context revealing how geopolitical tensions can result in cyber warfare, while the technical analysis demonstrated the exploitation of known vulnerabilities which enabled its rapid spread and devastating impact worldwide. NotPetya had consequences which extended beyond financial loss as it crippled sectors of Ukraine's economy and infrastructure as well highlight the vulnerabilities in cybersecurity practices across industries. 

NotPetya's impact on Ukraine's infrastructure highligthed the far reaching consequences of cyberattacks of this nature. This is a beginning of a new age of warfare, attacking an enemy nation not only physically but digitally as well. This was one the most terryfying and most costly act of cyberattack to have ever occurred

## Reference
## Appendices

# NotPetya Ransomware Guidelines
## Body
1. What
	1. Classic ransomware screen 
		1. Repairing file system on c not to turn computer off
		2. ransomware screen, pay 300 dollars of bitcoin to decrypt the files
	2. Petya was discovered in March 2016
		3. named Petya after the soviet weapon satelite in golden eye
	3. NotPetya 
		1. Main difference was it was created to spread quickly
		2. By the second you saw it the data center would've been gone
	4. The NotPetya
		1. 10billion in damages 
		2. wannacry attack only led to 4-8 million in damages 
	5. Often with ransomware you don't know if by paying the ransomware will give users access to their files again
		1. But with NotPetya there was no key that existed to unecrypt the content
		2. This virus was built only for one thing, maximum desctuction
		3. This was clearly an act of cyberwarfare from Russia towards Ukraine
2. where
	1. First started off in Ukraine then the globe
		1. Within a single day the virus had spread to france, germany, italy, polansd, united states
		2. But the majority of infections targeted ukraine
		3. 80% was in Ukraine
	2. LINKOS group was ground zero for the virus
		1. They maintained medoc which was an accounting software similar to turbotax
		2. spring of 2017 had targeted this company and hijacked their update servers
		3. they used these servers as a backdoor to thousands of ukrainian hoseholds through the medoc software the accounting software that thousandsd of ukrainians used
3. when
	1. Wannacry attack happened a month before infecting over 150 countries. causing millions of dollars in damages
	2. June 27, 2017 Ukrainian holiday constitution day 
	3. On October 20, 2020 charged 6 russian government charges with the notpetya attack 
4. why
	1. Spread like wildfire even to customers who operated branches in ukraine
	2. This was not accidental, it was designed to send a political message
		1. "if you do business in ukraine bad things are going to happen to you"
	3. Some worldwide companies affected
		1. Maersk
		2. Marck
		3. Saint-Gobain
	4. Russia and Ukraine have been engaged in an ongoing war since early 2014
		1. Key moments 
			1. was the annexation of crimea in 2014
			2. surrounding the status of the ukrainian region of donbass
		2. Around 13000 Ukrainians have died since conflict broke out in early 2014
	5. Since 2014 russia has been engaging cyber warfare with ukraine
		1. attacked the ukrainian power grid in the winter
		2. attacked railways and critical infrastructure
		3. rigged election websites
	6. Cyberspace has been one of the main fronts in this war
5. How
	1. Notpetya spread so quickly because it took advantage of 2 explits
	2. Eternal blue
		1. Exploit created by the NSA which took advantage of a vulnerability in windows Sever Message Block (SMB) protocol
		2. EternalBlue was leaked to the world in early 2017
		3. although Microsoft had released a patch to the vulnerability many computers around the world had not yet been patched
		4. **Very important to patch systems with security patches**
	3. MemeCats
		1. older invention by a french security researcher in 2011
		2. it was released to show that windows passwords could be found deep within ram
		3. if hackers could gain access to guest or limited access to a computer
			1. They could use memecats to find other users' passwords and hack into other computers using those credentials
	4. Combined together
		1. can infect computers that aren't patched then grab the passwords from those unpatched computers
		2. Meaning that even patched computers were not even safe from the virus
		3. The virus was especially effective within networks with multiuser computers 
			1. because it would automatically jump between one computer to the next within lightning speeds 
6. What have we learned from NotPetya?
	1. Ransomware is not going away and these attacks are bound to get more and more sophisticated
	2. Best course of action is to assume that an attack is inevitable and its going to happen
	3. Companies need to have plans in place and know how to execute these plans
		1. Know how long it would take to get back up and running
		2. Training disaster recovery for these scenarios are vitally important
		3. so that everyone involved knows their roles and responsibilites in the case of an attack coming.
	4. The importance of businesses taking backups seriously was highlighted especially by the shipping comany Maersk
		1. they did not have proper backups in place
		2. Only reason they were saved was because there was a power outage in one of their remote offices in jghana
		3. A total fluke in west africa had left 1 domain controller safe from the destructive forces of notpetya
	5. We need to be regularly backing up our data and it is good practice to use different encryption keys for our backups
	6. Biggest takeaway from Notpetya 
		1. Cyberwarfare against a country's critical infrastructure is not an abstract concept from scifi again
		2. Cyberweapons have already been used by governments against other nations
		3. It is a real issue that is occuring today and it will only become more prevelent
	7. NotPetya's impact on fukraine's infrastructure highlighted the far reaching consequences of cyberattcks of this nature
		1. Previous attacks have shown that healthcare ingrastructure can be vulnerable as well.
		2. This is a beginning of a new age of warfare attacking an enemy nation not only physically but diligitally as well
		3. this was one of the most terrifying and most costly and most deadly to have occured
	8. Its clear that countries need to be putting resources into trying to protect critical infrastructure from attacks
		1. Planning for disaster recovery when such attacks do occur
7. How does this effect and what can ...
	1. Countries learn from this attack...
	2. Businesses learn from this attack...
	3. We as customers and humans learn from this attack...

## Executive Summary
- Key Focus: This section concisely summarizes the essay, encapsulating its significant themes and findings. It highlights the central issue or phenomenon, its pivotal aspects, and the conclusions drawn.
- Essence of Analysis: The summary distills the critical analyses undertaken in the essay, summarizing the exploration of the subject's various dimensions, including its historical background, technical aspects, impact, and the responses or changes it has instigated.
- Conclusion and Future Outlook: This part briefly restates the thesis, summarizing the essay's main findings and offering perspectives or predictions about future developments or challenges related to the topic.
## Introduction
- Background: Provides a brief overview of the topic, setting the context for the reader.
- Thesis Statement: This statement clearly states the central argument or purpose of the essay, outlining what the essay aims to analyze or demonstrate.
- Scope of the Essay: Outlines the key areas the essay will cover, framing the structure and focus of the analysis.
## Body
### Section 1 (e.g. Historical Analysis)
- Discusses the topic's origins, development, or historical context.
### Section 2 (e.g. Technical Analysis)
- It breaks down the technical or specific aspects of the subject, providing a detailed examination.
### Section 3 (e.g. Impact Analysis)
- Examines the effects or implications of the topic on relevant areas or systems.
### Section 4 (e.g. Responses and Changes)
- How has the field, industry, or world responded to the topic, including policy, practical, or theoretical changes?
### Section 5 (e.g. Ethical and Political Considerations)
- Addresses the ethical and political dimensions associated with the topic.
### Section 6 (e.g. Counterarguments and debates)
- Presents alternative viewpoints and critiques related to the topic, providing a balanced perspective.
## Conclusion
- Summary of Findings: Concisely recaps the main points and findings of the essay, reinforcing the thesis.
- Restate Thesis: Reemphasizes the central argument or findings of the essay.
- Future Outlook: Discusses potential future developments, challenges, or unanswered questions in the topic area.
## Reference
## Appendices (Optional)

## Questions to answer
1. Overview
	1. What
	2. Who
	3. When
	4. Where
	5. How
2. What is it in greater detail 
	1. Detail 
	2. Simple? Complicated?
	3. How easy was it to get infected?
3. How did the world react?
4. What other software expanded from it?
	1. Did it create a new family of viruses?
5. How does this effect and mean for us?
	1. Software affects our lives everyday
	2. Be aware that anything can go down
	3. Protect ourselves from online threats as much as we can
	4. Software effects ourselves and humans. It is our duty to be responsible with its use
		1. As we discussed if it can cause so much damage to infrastructure

## Rubric requirements
### Objective

- To conduct a detailed analysis of the NotPetya malware, focusing on its delivery mechanisms, capabilities, impacts, and potential preventive measures.
- To demonstrate and apply comprehensive knowledge of network security concepts in the context of a sophisticated and historically significant cybersecurity threat.
### Learning Outcomes
- Advanced Network Security Understanding: You will gain a thorough comprehension of complex cybersecurity principles, particularly malware operation and defence strategies.
- Analytical Skills in Cybersecurity: Develop the ability to critically analyze and dissect significant cybersecurity incidents, understanding their multifaceted impacts on technical, political, and ethical levels.
- Research Proficiency: Enhance skills in conducting detailed research using varied, credible sources and effectively synthesizing this information to form a well-informed viewpoint.
- Technical Communication Excellence: Improve the ability to clearly and effectively communicate intricate technical information, ensuring it is accessible to an audience with a background in network security.
- Reflective Practice in Cybersecurity: Critically reflect on cybersecurity practices, drawing lessons from historical incidents and considering their implications for current and future security strategies.
### Details
- This essay is intended for readers with a background in network security.
- Assume your audience is familiar with technical jargon and advanced cybersecurity concepts.
#### Introduction to NotPetya
- A brief overview of NotPetya and its significance in cybersecurity.
- Historical context: discovery, initial impressions, and the geopolitical landscape during its emergence.
#### Technical Analysis
- Delivery Mechanisms: Detail how NotPetya was distributed and infiltrated systems. Discuss any exploitation methods, vulnerabilities used, and network propagation tactics.
- Capabilities: Examine the malware’s functionality. Focus on its ability to disrupt systems, encrypt data, manipulate processes, and evade detection.
- Payload and Impact: Discuss NotPetya’s intended and actual effects on affected organizations or industries. Explore its destructive capabilities, impact on critical infrastructure, and differences from other malware types (e.g., ransomware or espionage tools).
#### Preventive Measures
- Analyze potential strategies that could have been employed to prevent NotPetya’s success. Consider network segmentation, patch management, intrusion detection systems, and employee training.
- Reflect on the lessons learned from NotPetya regarding securing critical infrastructure and mitigating large-scale attacks. Broader Implications and Conclusions
- Discuss the broader implications of NotPetya on global cybersecurity policies, the ethics of state-sponsored cyber warfare, and the future of cyber-physical security.
- Conclude with your perspective on the long-term impact of NotPetya on network security.

## Bibliography
- https://www.youtube.com/watch?v=KUKeZuIU74Y&t=11s
- https://www.researchgate.net/publication/353072644_Case_Study_The_NotPetya_Campaign
- https://www.hypr.com/security-encyclopedia/notpetya
- https://www.cloudflare.com/en-ca/learning/security/ransomware/petya-notpetya-ransomware/
- https://gallery.logrhythm.com/threat-intelligence-reports/notpetya-technical-analysis-logrhythm-labs-threat-intelligence-report.pdf
- https://www.brookings.edu/articles/how-the-notpetya-attack-is-reshaping-cyber-insurance/
- https://en.wikipedia.org/wiki/Petya_(malware_family)
- https://www.statista.com/statistics/1293492/ukraine-war-casualties
- https://www.cybereason.com/blog/blog-a-quick-recap-on-notpetya
- https://www.wallarm.com/what/what-is-mimikatz
- https://en.wikipedia.org/wiki/EternalBlue
- https://www.varonis.com/blog/what-is-mimikatz
- https://en.wikipedia.org/wiki/Mimikatz
- https://www.digitalguardian.com/blog/cost-malware-infection-maersk-300-million
- https://www.ibm.com/topics/incident-response
- https://www.pwc.com/sg/en/services/reimagine-digital/cybersecurity/cyber-incident-response-recovery.html
- https://www.provendata.com/blog/notpetya-ransomware
- https://rgs-ibg.onlinelibrary.wiley.com/doi/full/10.1111/area.12728
- https://www.armis.com/blog/reflecting-on-notpetya-a-milestone-in-cyberwarfare-history/
- https://www.bbc.com/news/technology-40428967
- https://www.varonis.com/blog/a-brief-history-of-ransomware
