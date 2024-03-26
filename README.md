# Artemis
artemis-pentest-walkthrough

Phase 1. Perform Reconnaissance

The goal of this initial phase of the pen test is gathering info on Artemis, the fictional company based in France that supplies industrial gas to major customers in the chemicals, petrochemicals, refining, and steel industries. Building a profile on Artemis will include the company’s technology stack, email addresses, phone numbers, resumes, and more. 

Firstly, one major piece to use that will help kick off my search is the very “Client Overview” section for this assignment: Artemis’s region is identified, as well as other metrics such as the number of customers it serves, and even how many employees work at the company. We also learn what industries Artemis’s customers inhabit, as well as the city and state that its operations control center resides in. Though this is general information, these details will help inform me in the next resource I will use. 

OSINT is the next tool following the information gleaned from the client overview section; I will perform Google searches to find public information on Artemis, its specific operations in Houston, Texas. Moreover, LinkedIn will be the perfect place to find specific names of individuals within the organization, and I would be sure to check if emails or phone numbers are kept public on any profiles. I would also go as far as to check sites like GlassDoor and other job board/review sites to see if any anonymous users have carelessly left any details in their posts. 

Using the names and details gathered from my research on sites like LinkedIn, GlassDoor, and Indeed, I would transition to more informal social media sites such as Facebook, Instagram, TikTok, and Twitter. I would first check to see if Artemis has a prominent social media page on any of the social media sites, and cross-reference any names I’ve found from prior searches as well as find new ones. From here, I would type the names that I’ve found into Facebook, Instagram, TikTok, and Twitter, and look for any posts where Artemis or specific users are tagged.

I plan on leveraging this loop of search engines and social media sites to extract as much information as possible; by posing as a prospective employee for Artemis, I can “network” and add connections and even conduct interviews to ask questions about the industry and even get connected with more individuals. Viewing public posts on LinkedIn will expose me to more names, emails and phone numbers (if possible), and even resumes (I’ve seen users on LinkedIn post resumes on their wall seeking comments and criticisms). This info could then be fed into social media sites like Instagram and Facebook, and some careless employees may have valuable information posted on their profiles. I can exploit this loop until I am satisfied with the information I have amassed. 

Another source I could use is YouTube; after searching for videos that have anything to do with Artemis, the comments may provide a potential source of information. Employees past and present may share anecdotes in comment sections that may or may not be relevant to my profile building, but are a welcome source regardless. Similar to YouTube, forums like Reddit and 4chan may also be sites full of potential information; privacy and freedom of speech on these platforms empower users to speak their mind. If I’m lucky/quick enough, I may find some posts that have not already been deleted by moderators that share a little too much information on the inner workings of Artemis. 

With regards to domain information, I could plug in any of the emails I’ve found (and even Artemis’s primary website URL) into a reverse whois lookup engine to drill down on domains owned by an individual or company. Collecting additional domains gives us alternative attack surfaces to perform vulnerability tests, further aiding our efforts in penetration testing Artemis overall. 

The following tools will aid in performing deep scans on the Artemis server and search for vulnerabilities: port scanners (like Nmap), URL fuzzer,  Website Recon, and web application firewall (WAF) detector. 

Port scanners such as Nmap enable us to perform scans on the target host to see if: the host is live, what services are running, what ports are open, and other details such as what operating system is being utilized by the host. Scanning for a live host ensures that the scan is optimal, as searching for open ports on a “dead” host is a waste of time. If we find a live host, we can then identify what services are being used and what ports are open; this is crucial information as certain vulnerabilities are tied to specific services and ports, and we can tailor our pen testing approach according to what is being utilized. Lastly, specific operating system details are of utmost importance because it helps inform which vulnerabilities we can focus on, as again, vulnerabilities can be tied to specific OSs. 

A URL fuzzer allows us to type in a specific server URL and discover hidden files and directories that may be hidden away on that server.

Website Recon is a tool that allows us to discover the tech stack used by the target web application, both server-side and client-side. If we know the tech stack, we can have a more focused vulnerability testing approach later on. 

The WAF detector determines if a web application is being protected by a firewall; knowing what firewalls are in place will enable us to adapt our attacks for a successful bypass. 

Lastly, I would check Pastebin to see if any data dumps yield information on Artemis; users can anonymously upload and share text on Pastebin. Though legitimate posts of beneficial code from developers and long form updates from Twitter users may be posted on the site, illegitimate content such as malware code, information on specific exploits, and other confidential data may be shared. 
