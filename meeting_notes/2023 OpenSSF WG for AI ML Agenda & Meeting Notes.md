<h2>2023 OpenSSF WG for AI/ML Agenda and Meeting Notes</h2>


**Meeting Link:** [https://zoom.us/j/94945593977](https://zoom.us/j/94945593977#success) (as per the meeting invitation)

Note: You will need a login to [https://lfx.linuxfoundation.org/](https://lfx.linuxfoundation.org/) for this link to work.

(In the event of IT difficulties, links dropping out etc., we still have the **old** link [here](https://zoom.us/j/94945593977))

**Time: **Every other Monday, 18:00 UTC

**WG Proposal Link:** 

**Slack channel:** [#wg_ai_ml_security](https://openssf.slack.com/archives/C0587E513KR) 

**Mailing list:** ​​[https://lists.openssf.org/g/openssf-wg-ai-ml-security](https://lists.openssf.org/g/openssf-wg-ai-ml-security) 

**Repo:** [https://github.com/ossf/ai-ml-security](https://github.com/ossf/ai-ml-security) 

**Shared Drive**: [https://drive.google.com/corp/drive/folders/1zCkQ_d98AMCTkCq00wuN0dFJ6SrRZzNh](https://drive.google.com/corp/drive/folders/1zCkQ_d98AMCTkCq00wuN0dFJ6SrRZzNh) 

**Facilitators**: Mihai Maruseac, Jay White

Please use the[ 2024 Meeting Notes](https://docs.google.com/document/d/1YNP-XJ9jpTjM6ekKOBgHH8-avAws2DVKeCpn858siiQ/edit?usp=sharing)

<h2>2023-12-11</h2>


<h3>Attendees:</h3>


Put an “X” in the “Present” column if present


<table>
  <tr>
   <td>Present
   </td>
   <td>Name
   </td>
   <td>Organization
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Mihai Maruseac 
   </td>
   <td>Chair, Google GOSST
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Jay White
   </td>
   <td>Chair, Microsoft
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Dana Wang
   </td>
   <td>OpenSSF
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Victor Lu
   </td>
   <td>Independent
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>David A. Wheeler
   </td>
   <td>OpenSSF
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Jorge VARGAS
   </td>
   <td>Independent
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Yotam Perkal
   </td>
   <td>Rezilion
   </td>
  </tr>
</table>


<h3>Introduction/Welcome New Friends!</h3>




* 

<h3>Agenda/Meeting Notes</h3>




* Note: OpenSSF Day Japan & AIxCC Kickoff was last week - some may be recovering
* AixCC - [https://aicyberchallenge.com/](https://aicyberchallenge.com/) - kickoff was last week
    * DARPA’s Artificial Intelligence Cyber Challenge (AIxCC) will bring together the best and brightest in AI and cybersecurity to defend the software on which all Americans rely.
    * AIxCC is excited to have Anthropic, Google, Microsoft, OpenAI, the Linux Foundation, the Open Source Security Foundation, Black Hat USA, and DEF CON as collaborators in this effort.
    * $ millions in prize money
    * More details will be coming soon
    * David A. Wheeler is involved, but cannot share some details at this time due to NDA. However, we want many people to compete in this competition!
* Informational - OpenSSF TAC election timeline:
1. Nominations Open: NOW
2. Nominations CLOSE: Dec 15
3. Voting Starts: December 16
4. Voting Stops:  December 30
5. New members seated: January 1 \
To request a ballot that we sent through [OpaVote please fill out this google form](https://forms.gle/7suYexAnPxndvX856). \
To run for the TAC:
1. [SCIR Member GB Nomination Form](https://forms.gle/ZZkC6zK3T7Ww43uC9)
2. [TAC Community Seat Self-Nomination Form](https://docs.google.com/forms/d/e/1FAIpQLSdMkN_H3zVFW7NfZzsanF5isga3PNVUQj7-8VPlVPhb2F2iYQ/viewform)
* Had meeting with LF AI Data
    * Plan to have joint meetings, agreed on this last Thursday
* Anyone have any other business to add?
    * : threat modeling for data, models
        * Start from OWASP, work with Dana
* Plans for future conferences in 2024
    * Plans for OSS NA?
        * Model transparency
        * Panel discussion
        * Supply Chain track
* AIs:
    * Mihai working on making the repo more readable
        * Expect PR soon
        * Making the Repo Human Readable: - Sal
            * What elements do we want to include on the repo? I’ll be borrowing some style from [this repo](https://github.com/finos/zenith) to focus it on projects/papers
        * OS specific recommendations doc - Sal
        * Identify targets for security slam with AI - Sal
        * Create MSVR doc - Jay
        * Update Charter doc from original mission statement - Dan
        * Try to find owners for docs - Nigel
            * 
            * 
    * Reach out to other working groups
        * Cloud Security Alliance AI WG
        * Montreal institute for Ethics in AI
* We will NOT meet 2023-12-25.
* What is the next step? Code / data / model
    * OWASP list: [https://owasp.org/www-project-top-10-for-large-language-model-applications/assets/PDF/OWASP-Top-10-for-LLMs-2023-v05.pdf](https://owasp.org/www-project-top-10-for-large-language-model-applications/assets/PDF/OWASP-Top-10-for-LLMs-2023-v05.pdf) 
    * Henry is systematically threat modeling for data
    * Audrey (OWASP) looking at model
    * What about minimum viable security (MVP)?
        * We will need to define this in this group
    * Need to identify the problems
        * OWASP only covers LLM
        * Maybe we should get a meeting to discuss to cover the gaps?
        * A lot of these are research tasks, we need solutions, and in most cases we have no solutions.
        * David: You might look here as a starting point/ input my presentation [https://dwheeler.com/secure-class/presentations/AI-ML-Security.ppt](https://dwheeler.com/secure-class/presentations/AI-ML-Security.ppt)
            * Includes a simple taxonomy of threats & some discussion about what’s known
                * Do [Infer] the wrong thing (“Evasion”)
                    * Technical term: Adversarial inputs / adversarial examples
                * Learn the wrong thing (“Poisoning”)
                    * Technical term: data poisoning/Trojan attack
                * Reveal the wrong thing (“Lose Confidentiality”), Further broken down into 3 sub-categories
                    * Extraction: the attacker extracts the parameters or structure of the model from observations of the model’s predictions [Tabassi 2019]
                    * (Membership) inference: the attacker uses target model query results to determine if specific data points belong to the same distribution as the training dataset [Tabassi 2019]
                    * (Model) inversion: the attacker is able to reconstruct (some) data used to train the model, including private and/or secret data [Tabassi 2019]
        * Mihai: There are probably teams working on it, but I’ll need to look
        * Jay: It’s been put on the backburner in some sense, trying to limit what the systems can do
            * David: That’s great when you can, e.g., “don’t give it the launch codes” - but limiting what the systems can do really limits what the systems can do
            * Accidents can happen, leading to big problems. Example: a folder included a lot of private information, so you could see private/secret information. Prompts can often lead to this kind of revelation.
        * There are AI/ML specific risks, and then there are general risks.
            * David: Agreed, but people want to give ML systems tools that blur the line, e.g., give LLM access to a Python interpreter.
        * It’s reasonable to divide model, data for training the model, and the code for running the model (system that uses the inference system). However, it gets rather mixed/muddled in implementation.
            * David: I prefer the taxonomy listed above - users don’t care _where_ the problem happened
* Next meeting: 2024-01-08. David will present his presentation on AI/ML and security for group feedback

<h2></h2>


<h3>Attendees:</h3>


Put an “X” in the “Present” column if present


<table>
  <tr>
   <td>Present
   </td>
   <td>Name
   </td>
   <td>Organization
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Mihai Maruseac 
   </td>
   <td>Chair, Google GOSST
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Jay White
   </td>
   <td>Chair, Microsoft
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Mads R. Havmand
   </td>
   <td>Chainalysis
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Laurent Simon
   </td>
   <td>Google
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Pedro Ferracini
   </td>
   <td>Mercado Libre OSPO
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Aubrey King
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Jeff Borek
   </td>
   <td>IBM
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Dana Wang
   </td>
   <td>OpenSSF
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Victor Lu
   </td>
   <td>Independent
   </td>
  </tr>
</table>


<h3>Apologies:</h3>




* 

<h3>Introduction/Welcome New Friends!</h3>




* Welcome Laurent Simon, Aubrey, Dana, Mads
    * Aubrey from OWASP Top 10 for LLMs

<h3>Old Actions</h3>




* Mihai to reach out to Maximilan Huber for licensing
    * Please reach out under [maximilian.huber@tngtech.com](mailto:maximilian.huber@tngtech.com)
    * Include Jay in the reach out emails, see what legal we can include
* Mihai to reach out to Sarah for the charter and related docs
* Mihai working on making the repo more readable
    * Expect PR soon
    * Making the Repo Human Readable: - Sal
        * What elements do we want to include on the repo? I’ll be borrowing some style from [this repo](https://github.com/finos/zenith) to focus it on projects/papers
    * OS specific recommendations doc - Sal
    * Identify targets for security slam with AI - Sal
    * Create MSVR doc - Jay
    * Update Charter doc from original mission statement - Dan
    * Try to find owners for docs - Nigel
        * 
        * 
        * Need more
* Governance: working on charter and related docs is a priority
    * After this, we can sync with Montreal Institute for Ethics in AI, etc.

<h3>Topics </h3>




* New meeting time, hopefully stable
* [From Sarah]:
    * AI/ML +OSS+ Security. Need Venn diagram of "our sweet spot" to be industry leaders in OpenSSF. Otherwise, we risk not being really impactful amongst AI/ML and Security.
        * [1:39 PM] Definition: "venn diagram" AI/ML + OSS + Security
        * Improve secure development using OpenSSF tools/guides
        * Improve secure consumption using OpenSSF tools/guides.
    * Sarah and Jay chatted about this before Thanskgiving break
* Model transparency
    * Talk at ScaleByTheBay and [GitHub SLSA Bay Area Meetup](https://resources.github.com/github-slsa-meetup-nov16/)
    * Need to identify industry partners to work together on standardizing what needs to be included in the provenance
        * MUST vs SHOULD
        * Datasets, pretrained models, hashing scheme
* Still working on deconfliction with LF Data & AI WG
    * Meeting this thursday (30th Nov)
    * Need to update charter, refine and fill in current gaps
    * This is at 6AM Pacific, ask Mihai to be added to invite
* Minimum security baseline
    * Laurent: some existing security baseline [https://mvsp.dev](https://mvsp.dev) 
    * 
* 30th Nov: Jay will be doing a panel discussion at OASIS AI Panel (organized by OASIS and Cisco)
    * AI vulnerability disclosures
    * 11 AM Pacific
    * Need to register: [https://aisecuritysummit.org/](https://aisecuritysummit.org/)
* Holiday break incoming
    * 11th Dec is last member of the year
    * We should have a 360 outline for going into January
    * Plans for OSS NA?
        * Model transparency
        * Panel discussion
    * Build up on the momentum for the next conference season
    * Figure ways to fully integrate with the other teams
    * Maybe include this in the SupplyChain track?
* Telemetry paper ()
    * Need to reach out to Sal again
    * Or try dusting it off and bringing up to date
* Start a new doc with what we want to do in this WG and what we complement with other groups
    * SLSA, GUAC, Supply chain, S2C2F
    * Best practices
        * Complement Top 10 OWASP
        * Create guide together
    * End User Groups has done great job for threat modelling
        * Will need to be extended to include data/model parts
    * Need to also define what we are not touching, what is outside of scope
        * Risk of scope creep
* OWASP meetings
    * [Link to meeting wiki page](https://github.com/OWASP/www-project-top-10-for-large-language-model-applications/wiki/Meetings)
    * Meeting recordings also posted on YouTube : [https://www.youtube.com/@LLMTop10](https://www.youtube.com/@LLMTop10)

<h3>New actions</h3>




* [Jay] Reach out to Dana for MVSP / baseline
* [Mihai/Jay] Check/make sure we have a Google Drive for the WG
* [Victor] Template/start for the docs about threat modeling, 

<h2>2023-11-8</h2>


<h3>Attendees:</h3>


Put an “X” in the “Present” column if present


<table>
  <tr>
   <td>Present
   </td>
   <td>Name
   </td>
   <td>Organization
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Mihai Maruseac 
   </td>
   <td>Chair, Google GOSST
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Sarah Evans
   </td>
   <td>Dell Technologies
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Matt Rutkowski
   </td>
   <td>IBM (he/him)
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Cheuk Ting Ho
   </td>
   <td>OpenSSF
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Maximilian Huber
   </td>
   <td>TNG Technology Consulting
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Eoin Wickens
   </td>
   <td>HiddenLayer
   </td>
  </tr>
</table>


<h3>Apologies:</h3>




* Kathleen Goeschel, Red Hat

<h3>Introduction/Welcome New Friends!</h3>




* Welcome Max, Eoin, and Cheuk

<h3>Old Actions</h3>




* Making the Repo Human Readable: - Sal
    * What elements do we want to include on the repo? I’ll be borrowing some style from [this repo](https://github.com/finos/zenith) to focus it on projects/papers
* Anyone willing to be an expert for the OSI AI licence definition? 
    * This would be an informal, internal AmA style with their legal experts. 
    * Maximilian Huber comes from the license compliance side!
        * Please reach out under maximilian.huber@tngtech.com
* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal
* Create MSVR doc - Jay
* Update Charter doc from original mission statement - Dan
* Try to find owners for docs - Nigel
    * 
    * 
    * Need more

<h3>Topics </h3>




* NIST U.S. ARTIFICIAL INTELLIGENCE SAFETY INSTITUTE [https://openssf.slack.com/archives/C0587E513KR/p1699310525828439](https://openssf.slack.com/archives/C0587E513KR/p1699310525828439) 
    * Link to news: [https://www.commerce.gov/news/press-releases/2023/11/direction-president-biden-department-commerce-establish-us-artificial](https://www.commerce.gov/news/press-releases/2023/11/direction-president-biden-department-commerce-establish-us-artificial)
    * Link to LOI Submission: [https://www.nist.gov/artificial-intelligence/artificial-intelligence-safety-institute](https://www.nist.gov/artificial-intelligence/artificial-intelligence-safety-institute)
    * We need volunteers to take on writing the letter
* Model transparency
    * Repo: [https://github.com/google/model-transparency](https://github.com/google/model-transparency) 
    * Blog post: [https://security.googleblog.com/2023/10/increasing-transparency-in-ai-security.html](https://security.googleblog.com/2023/10/increasing-transparency-in-ai-security.html)
    * Talk at PackaginCon: [https://docs.google.com/presentation/d/1YAQ0nUE7e-liWzeVeqRGiICpQLXFnQDKlkt2b-Tb0Ag/edit?pli=1#slide=id.g2949fd23bf8_0_3072](https://docs.google.com/presentation/d/1YAQ0nUE7e-liWzeVeqRGiICpQLXFnQDKlkt2b-Tb0Ag/edit?pli=1#slide=id.g2949fd23bf8_0_3072)	
    * Eoin has been working on a group for this, chatting with Laurent
        * HiddenLayer, NVidia
        * Standard for signing all files in a model
        * Extend to multiple PKIs
    * Working on scaling hashing and ensuring integrity of all files that compose a model
    * How to handle a mix of proprietary and open models?
* Still working on deconfliction with LF Data & AI WG
    * Need to update charter, refine and fill in current gaps
* SLSA Bay Area GitHub Meetup: [https://resources.github.com/github-slsa-meetup-nov16/](https://resources.github.com/github-slsa-meetup-nov16/) 
* Two approaches we can take:
    * Helping industry
    * Helping developers / data scientists
        * There’s a lot of improvement we can do here: training, tooling, documentation
        * E.g. improvements to Jupyter Notebook
    * Scorecards for ML workflows?
    * We need to decide if we do this work in this WG or find another one
    * Sarah will work with Jay to put these in the Charter
* Security telemetry 
* Governance committee
    * Work with TAC
    * Review membership for associate level applications
        * There is Montreal Institute for Ethics in AI
            * Should sync with us
    * **Makes working on charter and related docs a priority**

<h3>New actions</h3>




* Mihai to reach out to Max for licensing
* Mihai to reach out to Sarah for the charter and related docs

<h2>2023-10-25</h2>


<h3>Attendees:</h3>


Put an “X” in the “Present” column if present


<table>
  <tr>
   <td>Present
   </td>
   <td>Name
   </td>
   <td>Organization
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Nigel Brown
   </td>
   <td>Stacklok
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Pedro Ferracini
   </td>
   <td>Mercado Libre OSPO
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Mihai Maruseac 
   </td>
   <td>Chair, Google GOSST
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Victor Lu
   </td>
   <td>Independent
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>David A. Wheeler
   </td>
   <td>Linux Foundation
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Kathleen Goeschel
   </td>
   <td>Red Hat
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Enoch Kaxada
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Matt Rutkowski
   </td>
   <td>IBM
   </td>
  </tr>
</table>


<h3>Introduction/Welcome New Friends!</h3>




* Kathleen Goeschel, Red Hat
* Enoch Kaxada - learned about OpenSSF, looking into learning more about these meetings

<h3>Old Actions</h3>




* Making the Repo Human Readable: - Sal
    * What elements do we want to include on the repo? I’ll be borrowing some style from [this repo](https://github.com/finos/zenith) to focus it on projects/papers
* Anyone willing to be an expert for the OSI AI licence definition? 
    * This would be an informal, internal AmA style with their legal experts. 
* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal
* Create MSVR doc - Jay
* Update Charter doc from original mission statement - Dan
* Try to find owners for docs - Nigel
    * Need more

<h3>Topics </h3>




* FYI: LF Member Summit is today, we may not have some people today
* (Technical issues - audio issues on Zoom)
* Still need to walk through Old actions
    * Need to get experts on legal for OSI AI
    * Need to identify owners of documentation
* Any other business (AOB)

<h3>New actions</h3>




* Mihai: Google has been working on doing SLSA provenance & signing with Sigstore for ML, using GitHub
    * [https://github.com/google/model-transparency/](https://github.com/google/model-transparency/) 
    * Expect to announce tomorrow, 2023-10-25
* David: Presentation about security and ML
    * [https://dwheeler.com/secure-class/presentations/AI-ML-Security.ppt](https://dwheeler.com/secure-class/presentations/AI-ML-Security.ppt) 
    * Will be updated, workshop
    * Need to:
        * Update WG repo so that it looks properly when linking to it from the workshop
            * More information, documents, MSVR doc
        * What other topics to include in the presentation?
            * email to dwheeler at linuxfoundation . org
* Meeting time - do we want to move it?
    * Let’s wait briefly to see who else joins, then consider rescheduling
* Meet with LF AI
    * Talk to LF AI TAC on Thu Nov 30, 2023 2pm - 3pm (GMT) 15 min
        * OpenSSF brainstorming collaboration with LF AI & Data
        * Couple of slides (1 week before)
            * Who are we?
            * How can we contribute to your projects?
* We need to identify this WG’s specific outputs
    * What’s important, what do we think we can actually accomplish?
    * It’s okay/necessarily to work incrementally
* One option: Guidance for software developers who are using ML to generate code - what can they do to increase the likelihood of generating/deploying *secure* code? (Better prompts, how to examine for common ML mistakes, etc.)
* Mihai: I have AI experience, Supply chain security. I’m interested in strengthening the AI supply chain - not just signing pipeline, but that the resulting ML model is safe
* Victor Lu: Other groups seem to be focused on a consulting focus. OpenSSF is focused more on a fundamental solution perspective, that’s unique.
* Kathleen: group focused on integrity of data used to train the ML; working in supply chain security at RedHat; focus on foundational models
* Mihai: Google has doc on security for models - Secure AI Framework - [https://blog.google/technology/safety-security/introducing-googles-secure-ai-framework/](https://blog.google/technology/safety-security/introducing-googles-secure-ai-framework/) 

<h2>2023-10-11</h2>


<h3>Attendees:</h3>


Put an “X” in the “Present” column if present


<table>
  <tr>
   <td>Present
   </td>
   <td>Name
   </td>
   <td>Organization
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Nigel Brown
   </td>
   <td>Chair, stacklok
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Mihai Maruseac 
   </td>
   <td>Google GOSST
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Christine Abernathy
   </td>
   <td>F5
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Sarah Evans
   </td>
   <td>Dell Technologies
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Dan Appelquist
   </td>
   <td>Snyk
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Mike Lieberman
   </td>
   <td>Kusari
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Dana Wang
   </td>
   <td>OpenSSF
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Amanda Martin
   </td>
   <td>Linux Foundation
   </td>
  </tr>
</table>


<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Making the Repo Human Readable: - Sal
    * What elements do we want to include on the repo? I’ll be borrowing some style from [this repo](https://github.com/finos/zenith) to focus it on projects/papers
* Anyone willing to be an expert for the OSI AI licence definition? 
    * This would be an informal, internal AmA style with their legal experts. 
* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal
* Create MSVR doc - Jay
* Update Charter doc from original mission statement - Dan
* Try to find owners for docs - Nigel
    * Need more

<h3>Topics </h3>




* Voting results for co-leads
    * THANK YOU to everyone who was willing to be lead. We are VERY grateful! We had an awesome set of candidates, and we’re lucky to have any of them.
    * The winning co-leads per [https://github.com/ossf/ai-ml-security/issues/5](https://github.com/ossf/ai-ml-security/issues/5) are:
        * Jay White - GitHub @camaleon2016
        * Mihai Maruseac - GitHub @[mihaimaruseac](https://github.com/mihaimaruseac)
            * Started on TensorFlow, working on [SAIF](https://blog.google/technology/safety-security/introducing-googles-secure-ai-framework/), lots of overlap so it’s good to be involved here!
            * Welcome aboard!
    * Congratulations new co-leads!
    * HUGE thanks to Nigel Brown for successfully getting us to this point - please stick around!
* We might choose to re-vote on the meeting time, the “winning” seems to cause some problems
* LF AI - Meeting with Ibrahim
    * Alejandro is main point of contact
    * Talk to LF AI TAC on Thu Nov 30, 2023 2pm - 3pm (GMT) 15 min
        * OpenSSF brainstorming collaboration with LF AI & Data
        * Couple of slides (1 week before)
            * Who are we?
            * How can we contribute to your projects?
        * Who is to do this?
            * Mihai can do it
    * David A. Wheeler: We need to keep working on connecting OpenSSF + LF AI & Data better
* MVSR progress
    * OpenSSF  - think it’s okay
    * [ossf/ai-ml-security/mvsr.md](https://github.com/ossf/ai-ml-security/blob/main/mvsr.md) 
* Charter progress
    * Dan: No progress but I've got the action - will happen before next week.
* Report back from section owners
    * 
    * 
    * Should we link to these draft documents from the GitHub README?
    * We should probably migrate these to GitHub for easier understanding of what’s changing
* David A. Wheeler: Updated draft presentation on my AI/ML presentation here, comments welcome: [https://dwheeler.com/secure-class/presentations/AI-ML-Security.ppt](https://dwheeler.com/secure-class/presentations/AI-ML-Security.ppt) - email to dwheeler at linuxfoundation . org
* Meeting time challenges.
    * Options: redo polls, alternate timezones
* Old Actions
    * Licensing?
        * Not sure what ask is
        * Christine: I’m helping to draft OSI AI document, to be shared next week
        * David: At least sharing the OSI draft would be great, then we can work with OSI or raise issues or whatever
* Any other business (AOB)

<h2>2023-09-27</h2>


<h3>Attendees:</h3>


Put an “X” in the “Present” column if present


<table>
  <tr>
   <td>Present
   </td>
   <td>Name
   </td>
   <td>Organization
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Nigel Brown
   </td>
   <td>Chair, stacklok
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Jeff Borek
   </td>
   <td>IBM
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Pedro Ferracini
   </td>
   <td>Mercado Libre OSPO
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Christine Abernathy
   </td>
   <td>F5
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Munawar Hafiz
   </td>
   <td>OpenRefactory
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>David A. Wheeler
   </td>
   <td>Linux Foundation
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Naasief Edross
   </td>
   <td>Google
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Mark Sturdevant
   </td>
   <td>IBM
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Csaba Zoltani
   </td>
   <td>Nokia
   </td>
  </tr>
  <tr>
   <td>X
   </td>
   <td>Sal Kimmich
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>x
   </td>
   <td>Sarah Evans
   </td>
   <td>Dell Technologies
   </td>
  </tr>
</table>


<h3>Apologies:</h3>




* Mihai Maruseac (Google GOSST): traveling
* Sanket Naik
    * Have a conflict at the meeting time tomorrow
    * Reviewed the AI Security Telemetry document and Slack channel threads. Awaiting feedback on the “purpose” section in the document to proceed further on section 1.

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal
* Create MSVR doc - Jay
* Update Charter doc from original mission statement - Dan
* Try to find owners for docs - Nigel
    * Need more

<h3>Topics </h3>




* Voting results
    * [https://github.com/ossf/ai-ml-security/issues/3](https://github.com/ossf/ai-ml-security/issues/3) co-leads
    * [https://github.com/ossf/ai-ml-security/issues/2](https://github.com/ossf/ai-ml-security/issues/2) lead
    * ~~Congratulations new co-leads!~~
    * Unfortunately, we accidentally had two separate voting processes. Our apologies to all. It’s not clear how to “fix” this irregularity.
    * We decided to Re run the process, with votes due in 2 weeks. That seems the safest.
* Meeting time [https://www.when2meet.com/?21348484-Fx6Gv](https://www.when2meet.com/?21348484-Fx6Gv)
    * 1 hour earlier seems to be favourite
    * Agree?
* David A. Wheeler: The WG repo <[https://github.com/ossf/ai-ml-security](https://github.com/ossf/ai-ml-security)> is very sparse. Please create pull requests to turn the very sparse README, etc., so it points to existing work, explains what’s going on, etc. [https://github.com/ossf/ai-ml-security/issues/4](https://github.com/ossf/ai-ml-security/issues/4) requests auditions (it’s okay if there are links to Google documents, we just want to make sure newcomers can find things).
    * Stub docs in github
        * [Ai_ml_telemetry.md](https://github.com/ossf/ai-ml-security/blob/main/telemetry/ai_ml_telemetry.md)
        * [ai_ml_landscape.md](https://github.com/ossf/ai-ml-security/blob/main/landscape/ai_ml_landscape.md) 
    * MSVR
        *  - OpenSSF-wide MVSR
        * [ai-ml-security/mvsr.md](https://github.com/ossf/ai-ml-security/mvsr.md) 
    * Charter
* David’s [presentation idea](https://lists.openssf.org/g/openssf-wg-ai-ml-security/topic/idea_i_give_my_presentation/101606838?p=,,,20,0,0,0::recentpostdate/sticky,,,20,2,0,101606838,previd%3D1695767014421714791,nextid%3D1694722639795369434&previd=1695767014421714791&nextid=1694722639795369434) - any thoughts? My hope is that it’ll encourage others to join this group.
    * Objections? No objections heard.
    * We want to improve our GitHub repo, so that when new visitors arrive they’ll learn more about the WG.
* Need to interact with other groups: Best Practices WG, SBOMs, etc. Hard to find a group that doesn’t have some interaction with AI/ML
* We need to ensure LF AI & Data foundation participates!
    * We have some, want more. Let’s talk with Ibrahim Haddad (Executive Director) to make sure this happens.
    * Nigel will talk with Ibrahim.
* One challenge: many participants are users, not experts & developers.
    * SME = subject matter expert
    * A big challenge: Having the data to analyze
* Do we have a comment on [Federal Register :: Artificial Intelligence and Copyright](https://www.federalregister.gov/documents/2023/08/30/2023-18624/artificial-intelligence-and-copyright)
    * Sounds like something we should have
    * Comment period that ends in 21 days. (10/18/2023) - alerting public 
    * Policy committee, share - Nigel
    * Probably not enough time for us to create a cogent combined response. However, if someone writes a comment, please feel free to share with the group so others writing responses can consider them.
* Security Slam
    * Is this related to [https://github.com/ossf/wg-securing-critical-projects](https://github.com/ossf/wg-securing-critical-projects) ?
* Report back from section owners (we’re out of time, there has been progress, we’ll pick this up next meeting)
    * 
    * 
* AOB
* Sal: We’re finalizing a definition of “open source definition of AI” at OSI, contact Sal K.

<h3>New actions</h3>




* Re-run the voting - David
* Making the Repo Human Readable: - Sal
    * What elements do we want to include on the repo? I’ll be borrowing some style from [this repo](https://github.com/finos/zenith) to focus it on projects/papers
* Change the meeting slot - Nigel
    * Requested and moved
* Anyone willing to be an expert for the OSI AI license definition? This would be an informal, internal AmA style with their legal experts. 
* Can we define a clear point of contact across LF groups? 
    * Talk to Ibrahim - Nigel
* [Federal Register :: Artificial Intelligence and Copyright](https://www.federalregister.gov/documents/2023/08/30/2023-18624/artificial-intelligence-and-copyright) - Policy committee, share - Nigel
    * Shared via Brian (couldn’t find another address)

<h2>2023-09-20</h2>


<h3>Canceled</h3>




* Some are in Spain

<h2>2023-09-13</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* David Edelsohn (IBM)
* Pedro Ferracini (Mercado Libre OSPO)
* Mihai Maruseac (Google GOSST)
* Christine Abernathy (F5)
* Sanket Naik (Palosade)
* Munawar Hafiz (OpenRefactory)
* Victor Lu (Independent)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal
* Create MSVR doc - Jay
* Update Charter doc from original mission statement - Dan
* Check new meeting time in slack - Nigel
    * Failed
    * ~~Try ~~~~ ~~<- scrap this
    * Here is the link to the meeting planner [https://www.when2meet.com/?21348484-Fx6Gv](https://www.when2meet.com/?21348484-Fx6Gv)
* Try to find owners for docs - Nigel
    * Need more

<h3>Topics </h3>




* Discussion “how AI risk differ from traditional software risk”
    * Victor to lead

        


        Summary: There are many AI/ML Topics we need to work on at OpenSSF and there


        will NOT be much overlap with work by other foundations such as LF AI


        The content of the above document can be merged into Landscape White paper

    * Feedback from Sanket:
        * Keeping in mind that the audience is OSS devs and OSS consumers, the deliverables could be:
            1. Common reference architecture / building blocks for ML  that will be used across OSSF
            2. Address the threats for each block
            3. Provide best practices (in current state) to protect against threats for each block
            4. Provide guidance to keep in mind for future dev
    * Define AI security terminology
    * Differentiate LFAI security mandate from OpenSSF AI/ML WG
    * Propose mitigation
* Report back from section owners
    * 
    * 
* Old actions
* Reminder about the vote
    * [https://github.com/ossf/ai-ml-security/issues/3](https://github.com/ossf/ai-ml-security/issues/3) co-leads
    * [https://github.com/ossf/ai-ml-security/issues/2](https://github.com/ossf/ai-ml-security/issues/2) lead
    * Nominations by 15th September 2023 please
    * Do we need more time for nominations?
* Meeting 20th - I’m unavailable
    * Cancel?
        * We will cancel
    * ~~Does anyone else want to chair?~~
* AOB

<h3>New actions</h3>




* 

<h2>2023-09-06</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Dan Appelquist (TAC, Snyk)
* Sanket Naik  (Palosade)
* Randall T. Vasquez (LF)
* David Edelsohn (IBM)
* Sal Kimmich (EscherCloud)
* Jason Keirstead (Pobal Cyber)
* Jay White (Microsoft)

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Blog - unassigned for now

<h3>Topics </h3>




* Tac, Sept 5th
    * We are now officially an [incubating](https://github.com/ossf/tac/blob/main/process/working-group-lifecycle.md) working group 
    * Still need more focus, but acknowledge this will come with time
    * We need election and co-leads
* New time slot and frequency
    * Various reasons
    * Proposed bi-weekly on Mondays at 15:00 (UK BST)
        * Alternative Thursday at 16:00 UK (11:00 US Eastern)
* Switching to github .md
    * [https://github.com/ossf/ai-ml-security](https://github.com/ossf/ai-ml-security) 
    * Review PRs rather than manual
    * Any volunteers to do this
        * Landscape
        * Telemetry
        * Charter.md in README.md
        * MVSR
* Review 
    * 
    * 
* AOB

<h3>Notes</h3>




* Jay: there should be a co-lead.
* Dan: agree.
* Nigel: Will set up a vote.
* Jay: 1st order of business - we need to drill down on the MVSR, charter… not a 2nd or 3rd thing. We need to do that first.
* Jay: MVSR - Mission, Vision, Strategy and Roadmap
    * Strategy - we do have some idea - let’s get something down on paper
    * Mission and vision we have something right now
* Dan: [https://github.com/ossf/ai-ml-security](https://github.com/ossf/ai-ml-security) 
* David: we need to nail down what we’re trying to achieve
* Jay: We have a mission … once we have a mission & vision then strategy gets clearer - then roadmap is according…
* David: we need have definitive purpose
* Dan: we have landscape and telemetry documents…
* Victor
    * On telemetry document – I can take the lead on this section… (4) we can use slack or zoom calls to coordinate.
    * Suggest people take the lead on each section…
* We discuss moving the Telemetry document over to github – with each section in its own Markdown document.
    * Alternatively we keep it in Google docs…
* Telemetry document:
    * Every section to have an owner.
    * Changes to be presented back to main group.
    * We keep it in google docs for now.
    * 16 sections including the appendix:
        * 1. Intro – Santek
        * 2. Victor
        * 3. “AI Security and Telemetry”– - Dan A.
        * 4. [missing] - Victor?
        * 5. (regulation) missing owner
        * 6. Ai Standards & best practices - missing owner
        * 
* Meeting time change - proposing **15:00 London Time (BST) on Mondays**.… (bi-weekly)
    * We’ll put this in the chat and give people a chance to object…
* Yotam: MITRE vulnerability risks database - can we get them to come speak to the group? [agreed] Also - 2 others presented at Defcon about open source LLMs - i will ping them as well.
    * I will e-mail the MITRE person and we can find a date.

<h3>Old actions</h3>




* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal

<h3>Actions</h3>




* Reinstate the vote for lead and co-leads of group - Nigel
    * [https://github.com/ossf/ai-ml-security/issues/3](https://github.com/ossf/ai-ml-security/issues/3) co-leads
    * [https://github.com/ossf/ai-ml-security/issues/2](https://github.com/ossf/ai-ml-security/issues/2) lead
    * Nominations by 15th September 2023 please
* Create MSVR doc - Jay
* Update Charter doc from original mission statement - Dan
* Check new meeting time in slack - Nigel
* Try to find owners for docs - Nigel

<h2>2023-08-30</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Sarah Evans (Dell Technologies)
* Pedro Ferracini (Mercado Libre OSPO)
* David A. Wheeler (LF)
* Mark Sturdevant (IBM)
* Sanket Naik (Palosade)
* Christine Abernathy (F5)
* Jeff Borek (IBM)
* Munawar Hafiz (OpenRefactory)

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Blog - unassigned for now

<h3>Topics </h3>




* Tac, Sept 5th [LF AI & DATA | ML security committee + OpenSSF proposal · Issue #188 · ossf/tac · GitHub](https://github.com/ossf/tac/issues/188) 
    * Lots of enthusiasm, light on work
    * Will report back to OpenSSF TAC, the good news is that we’re coordinating with the LF AI & Data
    * We’ll see what TAC has to say
    * Need more focus on OPEN SOURCE aspects of this, but need to keep context.
* Review 
* Review 
* AOB

<h3>New actions</h3>




* OS specific recommendations doc - Sal
* Identify targets for security slam with AI - Sal
* We need a change summary for the docs - Nigel

<h2>2023-08-23</h2>


<h3>Attendees:</h3>




* Nigel Brown  (Chair, stacklok )
* Pedro Ferracini (Mercado Libre OSPO)
* Sarah Evans (Dell Technologies)
* Christine Abernathy (F5)
* Dan Appelquist (Snyk) / TAC
* Andreas Fehlner (ONNX)
* Yotam Perkal (Rezilion)
* Jason Keirstead (Cyware)
* Munawar Hafiz (OpenRefactory)
* Allen Stewart (Microsoft)
* Csaba Zoltani (Nokia)
* Jay White (Microsoft)

<h3>Apologies</h3>




* Mihai Maruseac  (Google GOSST)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Blog - unassigned for now

<h3>Topics </h3>




* Possibly a very short meeting - little movement on the docs
* Review 
* Review 
    * Dan To take ownership of
* AOB
    * Whitehouse - mobilisation plan re-fresh -  
    * DARPA contest - around AI security - open source use of AI - DARPA came to OpenSSF… [Announced](https://openssf.org/press-release/2023/08/09/openssf-to-support-darpa-on-new-ai-cyber-challenge-aixcc/) at BlackHat. DARPA to pay for 2 OpenSSF staff members who will run this competition - intentionally kept apart from other things OpenSSF is doing. 
        * Question about the association of this with OpenSSF - unclear on the roadmap…
    * 

<h3>New actions</h3>




* Go back to the TAC
    * Contextualize the DARPA initiative - Sarah - Dan to support
    * Blog post on telemetry ← Sal

<h2>2023-08-16</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Pedro Ferracini (Mercado Libre OSPO)
* Mark Sturdevant (IBM)
* Csaba Zoltani (Nokia)
* Andres Orbe (Alpha-Omega)
* Sal Kimmich (GadflyAI)
* Jay White (Microsoft)
* Altaz Valani (DevSecOpsMentor.com)
* Sanket Naik (Palosade)
* Christine Abernathy (F5)
* Parag Patil (Palosade)
* Sarah Evans (Dell Technologies)
* Prachi Jadhav (Stacklok)

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Blog - unassigned for now

<h3>Topics </h3>




* Question: Has anyone signed an ML model?
    * Up/downloaded from e.g. Hugging Face
    * SPDX 3.0? Sigstore?
* Review 
* Review 
* AOB
    * Yotam blackhat
        * Hugging face vulnerability
        * AI attack
        * Mitre - ML vulnerabilites

<h3>New actions</h3>




* Collaboration Touch Point: There is a regularly meeting AI SBoMs for SPDX Every Wednesday, August 16**⋅**5:00 – 5:45pm EST: [https://zoom.us/j/92452702075](https://zoom.us/j/92452702075)
* Collaboration touch point - FINOS [https://www.finos.org/](https://www.finos.org/)
* Check selling pitch of mistral.ai - they got > 200 000 000 $ funding with selling pitch alone. It involves whitebox LLM
* Check with refact.ai if their LLM is whitebox. Their software is opensource and might be run in a docker container. Basically it’s a plugin like a Copilot

<h2>2023-08-09</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Pedro Ferracini (Mercado Libre OSPO)
* Christine Abernathy (F5)
* Cheuk Ho (OpenSSF)
* Michael Scovetta (Microsoft)
* Mark Sturdevant (IBM)
* Amanda Martin (LF)
* Allen Stewart (Microsoft)
* David Edelsohn (IBM)
* Brian Knight (Microsoft)
* Altaz Valani
* Victor Lu 

<h3>Apologies</h3>




* Mihai Maruseac  (Google GOSST)

<h3>Introduction</h3>




* Hello Pedro, Cheuk

<h3>Old Actions</h3>




* Blog - unassigned for now
* Deliverable matrix in landscape doc - Sal

<h3>Topics </h3>




* LF/AI update
    * Meeting Thursday, 4pm BST [https://lists.lfaidata.foundation/g/mlsecurity-committee/calendar](https://lists.lfaidata.foundation/g/mlsecurity-committee/calendar)
    * All welcome
* Review 
* Review 
* AOB

<h3>New actions</h3>




* Create an issue (Nigel)
    * [https://github.com/ossf/tac/issues/188](https://github.com/ossf/tac/issues/188) 

<h2>2023-08-02</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Sal Kimmich (GadflyAI)
* Christine Abernathy (F5)
* Mark Sturdevant (IBM)
* Fridolin Pokorny (Independent)
* Maya Costantini (Red Hat)
* Andreas Fehlner (ONNX, Trusted AI Committee of LF AI&Data)
* David Espejo (Union.ai)
* Allen Stewart (Microsoft)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Blog - unassigned for now
* Deliverable matrix in landscape doc - Sal
* Common function for LF AI and Openssf AI ML - Nigel
    * Waiting
* Get hugging face contact to Christine - Nigel
    * Waiting

<h3>Topics </h3>




* LF/AI update
    * Review 
    * No objections to this plan.
* Review 
* Review 
* Assign sections for [AI Security Telemetry ](https://docs.google.com/document/d/1J8M1F5ev9tXzMpA3dAFXqXYs2t-T10xt0_ObXnqNN04/edit?usp=sharing)
* AOB

<h3>New actions</h3>


<h2>2023-07-26</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Dan Appelquist  (Snyk)
* Sal Kimmich (EscherCloudAI)
* Pedro Ferracini (Mercado Libre OSPO)
* Sanket Naik (Palosade)
* Mark Sturdevant (IBM)
* Christine Abernathy (F5)
* Michael Gildein (IBM)
* Mihai Maruseac (Google GOSST)
* Sarah Evans (Dell Technologies)
* Brian Behlendorf (LF)
* Victor Lu (Independent) 

<h3>Introduction</h3>




* New Attendees 

<h3>Old Actions</h3>




* Blog - unassigned for now
* Deliverable [matrix in content backlog](https://docs.google.com/document/d/1B8UlF-CQUN9092DIjSjDEEBJUcR-QN8q-Sno_Eq-_SU/edit?usp=sharing) - Sal
* Common function for LF AI and Openssf AI ML - Nigel
    * Waiting
* Get hugging face contact to Christine - Nigel
    * Waiting

<h3>Topics </h3>




* Meeting overhead
* Review 
* AOB
* Deliverable [matix in content backlog](https://docs.google.com/document/d/1B8UlF-CQUN9092DIjSjDEEBJUcR-QN8q-Sno_Eq-_SU/edit?usp=sharing), and suggested blog posts
* Last week we had a call - Linux Foundation AI workstream attended
* Yotam: added some context in the landscape.
* Sal: Will add a specific deliverable for Security Telemetry, and get a whitepaper writing group for it. This is our highest priority deliverable, and can help to outline future community contributions 

<h3>New actions</h3>




* In alignment with the above work, the below content backlog would be a great way to republish from LF blog - or to publish directly for the "[Cyberscape Zine 2.0](https://www.gadfly.ai/post/call-for-submissions-cyberscape-zine-2-0-voices-and-visualizations-on-ai-greetings-creators)" contest, here are 10 article ideas focusing on AI and security:
        * 1. The Landscape of AI and Cybersecurity
        * 2. Securing AI Systems: Challenges and Solutions
        * 3. AI in Cybersecurity: Friend or Foe?
        * 4. The Ethics of AI in Security: Balancing Safety and Privacy
        * 5. Adversarial Attacks on AI: An Emerging Threat
        * 6. AI and Data Privacy: A Complex Relationship
        * 7. The Role of AI in Detecting and Preventing Cyber Attacks
        * 8. AI in Secure Communication: The Future of Privacy
        * 9. Securing the AI Supply Chain: Challenges and Solutions
        * 10. The Future of AI and Security: Predictions and Possibilities
* Review Yotam’s additions to the Landscape document
* Yotam to share learnings from Defcon
* Discussion on deliverables 
    * We produce guidelines and proposals
    * Possible to win “august of AI” on hackernoon.com <- $1000 for best article.
    * Provenance & Security Telemetry for AI systems … maybe an “**industry whitepaper**”
        * Sarah - licensing and how evolving the licensing is; security - how do you find out if your data contains vulnerabilities - having  a workflow in place to mitigate: a **whitepaper** would be very helpful. I would participate.
        * Nigel: I would like to see a document that says “these are the limitations - these are the problems you can’t solve”
        * Sal: SBOMs - usually composable - different weights / epochs … we have an opportunity - show people who are building pipelines - work with the top 50 open source LLMs. “Specific data protections / telemetry / communication.” Feedback loops from people doing the same in [OpenSSF member orgs].
        * Nigel: I think LF would be interested in this. 
        * ?Action: Sal to work on a first draft?

<h2>2023-07-19</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Pedro Ferracini (Mercado Libre OSPO)
* Zach Steindler (GitHub, TAC)
* Mihai Maruseac (Google GOSST)
* Mark Sturdevant (IBM)
* Luke Hinds (stacklok, OpenSSF GB)
* David Espejo (Union.ai)

<h3>Introduction</h3>




* New Attendees
* Hello Mark, Pedro

<h3>Old Actions</h3>




* Blog - unassigned for now
* Deliverable matrix in landscape doc - Sal
* Git issue for chair nominations - see [https://github.com/ossf/ai-ml-security/issues/1](https://github.com/ossf/ai-ml-security/issues/1) 

<h3>Topics </h3>




* [Nominations](https://github.com/ossf/ai-ml-security/issues/1) for chair?
    * Deferred after input from Brian
* LF working group - Nigel
    * Meeting
    * Alejandro
    * Openssf overview volunteer
* Ideas (Christine’s)
    * Hugging Face 2FA 
        * wg-securing-software repos did a survey of security capabilities software repositories should have: [https://github.com/ossf/wg-securing-software-repos/tree/main/survey/2022](https://github.com/ossf/wg-securing-software-repos/tree/main/survey/2022) 
        * Not open source (neither is github)
    * Scorecard extension
        * This would be good
        * Project Oak - only an idea
        * We’d like attestations on modelcards
* Review 
    * Discuss a section and its issues

<h3>New actions</h3>




* Common function for LF AI and Openssf AI ML - Nigel
    * Discuss coordination with OWASP
* Get hugging face contact to Christine - Nigel

<h2>2023-07-12</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Zach Steindler (GitHub, TAC)
* Dan Appelquist (Snyk)
* David A. Wheeler (Linux Foundation)
* Sal Kimmich (EscherCloud)
* David Edelsohn (IBM)
* Anna Jung (VMware)
* Luke Hinds (stacklok)
* Michael Scovetta (Microsoft)
* Jason Keirstead (Pobal Cyber)
* 

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)

<h3>Introduction</h3>




* Welcome Andrew
* 

<h3>Old Actions</h3>




* ~~Luke to find sponsor on TAC~~ Zac has joined
* ~~Git MD repo - Nigel~~ (David created one)
* Blog - unassigned for now

<h3>Topics </h3>




* Nominations for chair?
    * Do we want to vote before TAC approval?
        * Will set it up (see [https://github.com/ossf/ai-ml-security/issues/1](https://github.com/ossf/ai-ml-security/issues/1) )
    * Mechanism
        * David Wheeler will set up the repo, then
        * Sal will fill out the repo with group’s info, and add a github issue for voting 
            * Title suggestions for repo: AI-ML-Security
* [TAC feedback](https://docs.google.com/document/d/1706vJpuyq4NpHpVYsOTeU90j5RpoJREX7MRlhAo-CW4/edit)
    * Liked the scope doc
    * Zac Steindler (TAC) will join us on the 19th
    * ~~Generally negative~~ It was not as negative as I thought. I stand corrected (Nigel)
        * Don’t feel we are different enough
        * General hesitation
        * ~~Crob didn’t have time - nobody else stepped up~~ Zac did step up and came along
    * Chicken and egg situation
        * Yep, they said
    * Options?
        * Carry on regardless of approval?
            * Hard to allocate resources
        * Merge/move to [ML Security Committee](https://wiki.lfaidata.foundation/display/DL/ML+Security+Committee)? 
* Review 
    * Progress?
    * We need to focus on the deliverables - will do a matrix

<h3>New actions</h3>




* Create a repo - David
    * [https://github.com/ossf/ai-ml-security](https://github.com/ossf/ai-ml-security)
* LF working group - Nigel to report back next week
* Deliverable matrix in landscape doc - Sal
* Git issue for chair nominations - see [https://github.com/ossf/ai-ml-security/issues/1](https://github.com/ossf/ai-ml-security/issues/1) 

<h3>Notes</h3>




* Sal: We need a relationship with the TAC, Timeline inside of the next month
* Michael: it should be easier to create a working group - 
* Zach: that sounds like a special interest group - working groups are unbounded…  need common terminology
* Nigel: SIG needs to be under a wg…
* David: usually
* David E: let’s talk about AI/ML security and stop talking about process….

<h2>2023-07-05</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Zachary Newman (Chainguard)
* Gary White (Verizon)
* Sal Kimmich (EscherCloud)
* Michael Scovetta (Microsoft)
* Christine Abernathy (F5)
* Michael Gildein (IBM)
* David Espejo (Union.ai)
* Jay White (Microsoft)
* Brian Knight (Microsoft)
* Sanket Naik (Palosade)
* David Edelsohn (IBM)

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)

<h3>Introduction</h3>




* Hello Gary!

<h3>Old Actions</h3>




* New meeting link - done
* Luke to find sponsor on TAC
* Git MD repo - Nigel
* Blog - unassigned for now
* Deliverables - main topic
* Ownership - main topic

<h3>Topics </h3>




* Scope document agree?
    * Correct Link:  
    * Owners: Sal, Jay, Christine
    * Do we have clear blue sky between us and other groups?
        * Yes
        * We want to promote cooperation between groups
        * Developer using AI for development trying to secure consumption 
        * AI Pipeline Developer trying to secure production 
        * **What is unique about the mission: **
            * LFAI supports AI and Data open source projects through incubation, education, and best practices. However, their community is focused on exactly what most developer foundations must be: project acceleration, not security. OpenSSF is the foundation of security expertise, and we need to develop a cohort of security-first engineering practices. This can be done in tandem with LFAI, but it’s simple: the end users are LFAI, but the ability to mobilize security education, intervention and open source supply chain hardening for this evolving sector is clearly within the remit, and expertise, of OpenSSF. 
                * Very frankly, if we can get a sponsor for a security SIG/WIG in LFAI, that’s just as effective as out of OpenSSF, but until Linux is doing something real for open source AI pipeline production security, we’re losing ground on vulnerabilities every single, sunny, bureaucratic day. 
* TAC and tact - next week’s meeting
    * Show them the scope doc
    * Any other messages?
        * We want to be a sig or wg - but not nothing.
        * WG more autonomy
    * Do we keep going?
        * Regardless of approval? - Some will, yes but with fewer resources
        * Form a splinter cell?
* Review 
    * Consolidate interested parties from 6/21 meeting into the contributors/owners
    * Added in the doc
* Should we submit an abstract overviewing this work to OpenSSF Day?
    * What and who to submit?
    * Panel
    * Security implementation with openssf scorecard
        * Sal, Yotam

<h3>New actions</h3>




* Sal Openssf day talk submission
* Regular show and tell
* Nominations for next week
* Luke to produce a charter

<h2>2023-06-28</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* David Espejo (Union.ai)
* Michael Scovetta (Microsoft)
* Jay White (Microsoft)
* Victor Lu
* Sanket Naik (Palosade)
* Sal Kimmich
* Daniel Appelquist (Snyk)
* Alexander Beaver (RIT)
* David A. Wheeler (LF)
* Luke Hinds (SRIC/GB)
* Christine Abernathy (F5)
* Pieter van Noordennen (Slim.AI) 
* Mihai Maruseac (Google GOSST)
* Prachi Jadhav
* Allen Stewart (Microsoft)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Luke to find sponsor on TAC

<h3>Topics </h3>




* New meeting link
* TAC proposal [https://github.com/ossf/tac/issues/175](https://github.com/ossf/tac/issues/175) [feedback](https://docs.google.com/document/d/18BJlokTeG5e5ARD1VFDl5bIP75OFPCtzf77lfadQ4f0/edit#heading=h.2aalagtx9xzh)
    * We need a TAC sponsor
    * We need a more explicit charter
        * Define contents
    * We need to explicitly define our crossover/overlaps with
        * https://github.com/ossf/wg-best-practices-os-developers
        * [https://wiki.lfaidata.foundation/display/DL/ML+Security+Committee](https://wiki.lfaidata.foundation/display/DL/ML+Security+Committee) - Brian Behlendorf had worked out some meetings with them.
        * [https://owasp.org/www-project-top-10-for-large-langua	ge-model-applications/#](https://owasp.org/www-project-top-10-for-large-language-model-applications/#) 
        * Others?
            * [https://futurenetworks.ieee.org/roadmap/aiml-working-group](https://futurenetworks.ieee.org/roadmap/aiml-working-group)
            * [https://cloudsecurityalliance.org/research/working-groups/artificial-intelligence/](https://cloudsecurityalliance.org/research/working-groups/artificial-intelligence/)
            * [https://www.airsgroup.ai/](https://www.airsgroup.ai/) ?
            * [https://www.ncsc.gov.uk/blog-post/introducing-our-new-machine-learning-security-principles](https://www.ncsc.gov.uk/blog-post/introducing-our-new-machine-learning-security-principles) ?
            * [https://owasp.org/www-project-machine-learning-security-top-10/](https://owasp.org/www-project-machine-learning-security-top-10/) ?
            * [https://www.etsi.org/technologies/securing-artificial-intelligence](https://www.etsi.org/technologies/securing-artificial-intelligence) ?
            * [https://cs.lbl.gov/what-we-do/machine-learning/secure-machine-learning/](https://cs.lbl.gov/what-we-do/machine-learning/secure-machine-learning/) ?
            * 
    * Sal & Jay will work this, we need to be more specific.
        * Framework will cover OSSF umbrella, subscope, external groups - and clearly define distinct gap coverage in security for this group
            * [SIG Scope: Defining the Gap in AI/ML Security](https://docs.google.com/document/d/11tXIecCx-PHaLGJwqT_o31WbUVXHz7mR2auxArYwnjQ/edit?usp=sharing)
    * We could separate “where are the lanes”
        * David A. Wheeler: Maybe LF AI works on “securing AI components & legal issues in their use”, while we work on “how to securely bring AI into larger systems”
    * Our first step is fact-finding.
    * It’s better go on fact-finding first so we can figure out how what the WG should do.
* David A. Wheeler did fill in parts of security landscape [https://docs.google.com/document/d/1AyivzKsERoIZcyr4XrH6CrNeUoYHhpiswThHS0XrbSU/edit](https://docs.google.com/document/d/1AyivzKsERoIZcyr4XrH6CrNeUoYHhpiswThHS0XrbSU/edit)
* Big discussion about legal issues
    * At least ask models to record “where did they get the data from” including licensing etc. - traceability / provenance
    * Lots of people want clear information on what are the legal/licensing of the results. Problem is, there are conflicting interpretations.
    * Trace this as a “traceability challenge” instead of a legal issue.
    * Describe the threats, use cases, models.
    * ,OSI is working on white papers on legal interpretations.
    * Dan: I’m fine with reframing this as provenance/traceability
        * David: Should this be part of the landscape paper - [https://docs.google.com/document/d/1AyivzKsERoIZcyr4XrH6CrNeUoYHhpiswThHS0XrbSU/edit](https://docs.google.com/document/d/1AyivzKsERoIZcyr4XrH6CrNeUoYHhpiswThHS0XrbSU/edit)
        * Focus on “legal issues still being worked, so for now let’s focus on traceability”
* Work - Initially a doc (possibly a versioned whitepaper)
    * Add a ‘licensing AI’ section? (Where should this be done?) Probably worth partnering with [OSI AI efforts around licensing](https://deepdive.opensource.org/) that helps developers to implement best compliance practices around AI 
    * Add an ethical section?

<h3>New actions</h3>




* Change link and notify
* Deliverable #1: Define the scope of various groups to prevent undesired overlap
    * Owners: Sal, Jay, Christine
    * Contributors: 
    * Talk to other groups, figure out what they're doing, what they aren't doing, where we (OpenSSF) should focus.
    *  (_half page_, according to David W) - a few sentences explaining the scope of THIS group, a few sentences about the scope of other groups, and making it clear they don’t seriously overlap.
    * ??? description of current AI landscape within and beyond LF, speaking to the specific gap that this working group fills in representing security first development in AI/ML
    * 
* Deliverable #2: [AI Landscape Document](https://docs.google.com/document/d/1AyivzKsERoIZcyr4XrH6CrNeUoYHhpiswThHS0XrbSU/edit#heading=h.j7gx4ey3nk3k)
    * Owner: 
    * Contributors: Sanket Naik, Dan, David A. Wheeler, Mihai
    * Including threat models for data traceability 
* _ACTION_: Consolidate interested parties from 6/21 meeting into the contributors/owners above.

<h2>2023-06-21</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Luke Hinds (SCIR, stacklok)
* Zachary Newman (Chainguard)
* Jay White (Microsoft)
* Andres Orbe (Alpha-Omega)
* Brian Behlendorf (LF/OpenSSF)
* Parag Patil (Palosade)
* Mihai Maruseac (Google GOSST)
* David Espejo (Union.ai)
* David A. Wheeler (Linux Foundation)
* Michael Scovetta (Microsoft, Alpha-Omega)
* Christine Abernathy (F5)
* Munawar Hafiz (OpenRefactory)
* Jeffrey Borek (IBM)
* Victor Lu (Independent)
* Prachi Jadhav (stacklok)
* Allen Stewart  (Microsoft)
* Sal Kimmich (EscherCloud)
* 

<h3>Introduction</h3>




* Parag Patil (Palosade)
    * Excited to be here!!! Lot to learn from the community :)
* Zack Newman 
    * Excited to be here :)
* David Espejo (Union.ai)
* Andres Orbe (Alpha-Omega)
* Sal
* Jeff Borek
* Allen
    * Excited to work with the team

<h3>Old Actions</h3>




* Brian report on [LF AI Security committee](https://wiki.lfaidata.foundation/display/DL/ML+Security+Committee) (also [ML Security Committee](https://lfaidata.foundation/projects/ml-security-committee/)) , re: crossover
    * LF “AI & Data Foundation” - Ibrahim Haddad is GM (this is different from Pytorch foundation, also in LF)
    * They have an “ML Security Committee” - led by Alejandro Saucedo
    *  Brian Behlendorf will meet with Alejandro.
    * We want to discuss “how can we be helpful to each other & avoid overlap?”
    * It’s not clear they’re focused on applications.
    * It’s such a young space that the boundaries are not solid
    * One possibility: OpenSSF works on “how to securely bring in & use AI/ML in applications” while LF AI works on “how to select training data, train, develop the AI components”. That may not be the right division of work, but the idea would be to find ways to avoid duplication & instead work together.
    * What are their work products? Brian: not sure, we’d need talk to them. They’re probably chartered to develop advice.
* Luke to find sponsor on TAC
    * Should we wait on discussions from LF AI & Data?

<h3>Topics </h3>




* Work - Initially a doc (possibly a versioned whitepaper)
    * What sections?
    * Who would be interested in working on what sections?
* TAC sponsor
* TAC proposal [https://github.com/ossf/tac/issues/175](https://github.com/ossf/tac/issues/175) 27th June
* Proto doc 
* Timebox first release 

<h3>Blog Article</h3>




* Release this before the white paper to announce the working group, what we’re going to work on, solicit additional help, etc.
* Target date: _______
* Content Owner: _______

Seed the stage, first create a blog about the collaboration of the paper.

<h3>Purpose: ID Why the OpenSSF has created an AI/ML WG, what we intend to do, what we’d like people to do to participate, how we intend to operate, what products/resources we intend to create, how we intend to work with the LF AI & Data Foundation.</h3>


<h3>Potential Document Sections</h3>


Purpose of the document – let’s be clear on the goals/expected takeaways



* This is in the doc now.

Title: “Why is there an OpenSSF AI WG?”

White Paper



* Plan for quarterly releases?

<span style="text-decoration:underline;">Sections</span>



* Executive Overview 
    * Luke
    * Jay (not a starter but definitely a finisher)
* Introduction
* Landscape, eco-system overview (LF MI/AL group, OWASP etc).
    * Yotam
    * Christine
    * Jay (not a starter but definitely a finisher)
    * Victor 
    * Allen
    * Jeff B
* AI-related threats (as different from “ordinary” threats)
    * Luke
    * David Wheeler
    * Christine
    * Allen
    * Prachi
    * Parag Patil/Sanket Naik (Palosade)
    * Victor 
* How existing OpenSSF projects (and non-OpenSSF where they make sense) can be leveraged. 
    * Luke
    * Jay (not a starter but definitely a finisher)
    * Yotam
    * Parag Patil/Sanket Naik (Palosade)
* Personas
    * As a maintainer, you should…
    * As an AI security engineer, you should …
    * As a consumer of AI-enabled things, you should …
* External resources (e.g. CNCF, OWASP AI top 10, MITRE, etc.)
    * Christine
    * Victor 
    * Jeff B
* Resources 
* Contributors (list of all who have contributed)

<h3>New actions</h3>




* Git MD repo - Nigel
* Proto document - multiple
* Blog - unassigned for now

<h2>2023-06-14</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair, stacklok )
* Brian Knight (Microsoft)
* David A. Wheeler (Linux Foundation)
* David Espejo (Union.ai)
* Zack Newman (Chainguard, lurking :) )
* Michael Scovetta (Microsoft)
* Daniel Appelquist (Snyk)
* Jay White (Microsoft)
* Saswata Basu (Mastercard)
* Sanket Naik (Palosade)
* Allen Stewart (Microsoft)
* Munawar Hafiz (OpenRefactory)

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)
* Luke Hinds (Stacklok)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Brian to check if regulatory belongs here
* Luke to find sponsor on TAC - [https://github.com/ossf/tac/issues/175](https://github.com/ossf/tac/issues/175)

<h3>Topics </h3>




* Welcome new friends!
    * Saswata Basu (Mastercard) - we’re looking at how to apply this. We’re looking at ways to use AI/ML to manage massive amounts of data.
    * Daniel Appelquist (Snyk)
    * 
* Brian B: I’m in China, all *anyone* wants to talk about is security & AI
* Need to interact with the LF AI/Big Data Security WG
    * LF AI & Data which has several projects this proposal seems to overlap with, starting with the ML Security Committee: [https://lfaidata.foundation/projects/ml-security-committee](https://lfaidata.foundation/projects/ml-security-committee/)
    * Brian Behlendorf will talk with Ibrahim (GM of it) about that
    * We’ll explore options, one possibility is work out different scopes. the goal is to eliminate duplication.
* David to present his work on AI/ML security ([slides](https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt))
    * Another good talk: https://www.youtube.com/watch?v=P7XT4TWLzJw
* Review the  briefly.
* Work - Initially a doc (possibly a versioned whitepaper)
    * What sections?
    * Who would be interested in working on what sections?
* 
* TAC proposal - next time

<h3>New actions</h3>




* Brian to talk to LF AI Security committee and look for crossover

<h2>2023-06-07</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair nigel.brown@whitepool.co.uk, stacklok)
* David A. Wheeler (Linux Foundation)
* Michael Scovetta (Microsoft)
* Michael Gildein (IBM)
* Mihai Maruseac (Google, GOSST)
* Amanda Martin (Linux Foundation)
* Jay White (Microsoft)
* Anna Jung (VMware)
* Sarah Meiklejohn (Google)
* Brian Behlendorf (Linux Foundation)
* Victor Lu
* Christine Abernathy (F5)
* Prachi
* Luke Hinds (Stacklok)

<h3>Introduction</h3>




* New Attendees (new friends)
    * Sarah Meiklejohn (Google)
* 

<h3>Old Actions</h3>




* Debate the mission statement  
    * Anyone have any immediate comments
    * Some requests for clarification, we made a number of proposed changes.

<h3>Topics </h3>




* (Sudden Zoom meeting crashes. Restarting work.)
* Agree or defer the 
* Discuss the streams of work - who would be interested in working on what
    * Example [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/#) 
    * Regulatory probably out of scope.
    * Problem: the OWASP list is stretched, it really isn’t about LLMs or AI/ML at all, it’s just an attempt to list 10 things. A lot is just “general good software”
    * We put the initial proposed streams of work in the “mission” statement (broadened now to help people understand it).
* Discuss the timeslot
* David: At some point I’d be happy to share my presentation on AI/ML security. [https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt](https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt) 
    * We could do that next week 
* Should we send proposal to the TAC & request creating an official WG?
    * One more meeting and we’re at the official 5 meetings
    * Let’s propose to the TAC after meeting 5

<h3>New actions</h3>




* Brian to check if regulatory belongs here
* Luke to find sponsor on TAC

<h2>2023-05-31</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair nigel.brown@whitepool.co.uk )
* Christine Abernathy (F5)
* Anna Jung (VMware)
* Jay White (Microsoft)
* Sanket Naik (Palosade)

Please try [https://zoom.us/j/97349085860?pwd=S0JKamdpZGFSVVJOK25QNkhHZUhhdz09](https://zoom.us/j/97349085860?pwd=S0JKamdpZGFSVVJOK25QNkhHZUhhdz09)

<h3>Apologies</h3>




* Mihai Maruseac (Google GOSST)
* Dan Appelquist
* Luke Hinds (stacklok)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Next meeting poll - set this slot. Want async communications to be first class.
* Create a mission statement

<h3>Topics </h3>




* Agree and or complete the 
* Discuss the streams of work - who would be interested in working on what
    * Discussed a little in passing but no conclusions until we agree a mission statement.
* Discuss the timeslot
    * Not done, but will likely move at some point.

<h3>New actions</h3>




* Let the  ferment for a while - let people have their say.

<h2>2023-05-26</h2>


Note: There was a scheduled meeting at this time, but this time wasn’t the result of the Doodle poll. The attendees agreed that we need to let the poll run its course to find the best meeting time, and so this wasn’t a real meeting. We did briefly discuss meeting time logistics.

It’s been a challenge to find a common time, so we _may_ need to re-run the poll with more options. In particular, there’s a strong preference by some to avoid Fridays. AI/ML is worldwide, making any one time hard. David A. Wheeler suggested that we may want to rotate between two times to make it easier for people in different geographical locations to participate.

David A. Wheeler hinted that he’d be sharing some information in the new OpenSSF AI/ML Slack channel <[#wg_ai_ml_security](https://openssf.slack.com/archives/C0587E513KR)>. For the record, here they are:



* “Miscellaneous: Artificial Intelligence / Machine Learning (AI/ML), Science of Security, Malicious Tools (diverse double-compiling (DDC)), [Are you in] Control, Vulnerability Disclosure.” This is a slide deck from David A. Wheeler’s graduate class on developing secure software, including a lot of information about securing systems that include AI/ML: [https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt](https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt) 
* Unfortunately there are a lot of “approaches” in the academic literature for securing AI/ML systems, particularly to  counter adversarial inputs, that sound good but don’t work in practice. David knows of no way to fully counter adversarial inputs in a way that resists strong attack (he would _love_ to learn of one).
* If you must do something to counter adversarial inputs & it’s okay if an attacker can easily thwart it, the “Adversarial Robustness Toolbox” can help today: [https://adversarial-robustness-toolbox.org/](https://adversarial-robustness-toolbox.org/)
* If you’re serious about countering adversarial inputs, human-in-the-loop and the dual language model pattern are the only techniques I know of. These are limiting. I’d love to learn of more options. For more about the dual language model pattern, see: “Prompt Injection Explained” by Simon Willison, [https://simponwillison.net/2023/May/2/prompt-injection-explained/](https://simponwillison.net/2023/May/2/prompt-injection-explained/)   

<h2>2023-05-24</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair nigel.brown@whitepool.co.uk )
* Sanket Naik (Palosade)
* Mihai Maruseac (Google GOSST)
* Jay White (Microsoft)
* Prachi Jadhav (Stacklok)
* Laurent Simon (Google, GOSST)
* Luke Hinds (stacklok)

<h3>Introduction</h3>




* New Attendees

<h3>Old Actions</h3>




* Next meeting poll - set this slot. Want async communications to be first class.
* Create a slack channel [#wg_ai_ml_security](https://openssf.slack.com/archives/C0587E513KR) 
* Create a mail group [https://lists.openssf.org/g/openssf-wg-ai-ml-security](https://lists.openssf.org/g/openssf-wg-ai-ml-security) 
* Consolidated notes here 

<h3>Topics </h3>




* Discuss the streams of work composition
* Identify some owners
* How to address 

<h3>New actions</h3>




* Meeting links
* Luke Hinds  to check with Brian B if a whitepaper can be delivered from this group
* Define and overall mission statement for the group 
* Look at moving the meeting because there are still conflicts

<h2>19th May 2023</h2>


<h3>Attendees:</h3>




* Nigel Brown (Chair nigel.brown@whitepool.co.uk )
* Christine Abernathy (F5)
* Mihai Maruseac (Google) - Google Open Source Security Team, working on GUAC & AI
* Michael Scovetta (Microsoft) - OSS Security, AI Security, Alpha-Omega, Identifying Security Threats WG - michael.scovetta@microsoft.com
* David A. Wheeler (Linux Foundation) (part) - focus on security, but have also worked in AI/ML, including supporting the Joint AI Center (JAIC)
* Matt Rutkowski (IBM) (mrutkows@us.ibm.com)
* Luke Hinds (Stacklok) - been on OpenSSF TAC, now on OpenSSF GB luke@stacklok.com 
* Yolanda Robla (Stacklok)
* Maia Hamin (Atlantic Council) mhamin@atlanticcouncil.org
* Anna Jung (VMware)
* Jay White (Microsoft) - also leads Dashboard SIG
* Brian Behlendorf (OpenSSF/LF) - did give talk on AI
* Cindy Sutherland (Lockheed Martin)
* Prachi Jadhav (Stacklok)
* Ken Arora

<h3>Introduction</h3>




* Attendees
    * Who are you?
    * What do you want to get out of this WG? (notes above)
* Request: In the future, can we deconflict this with other OpenSSF meetings? (Dashboard in this case) - Khahil White can run a Doodle poll to help do this, that ok?
* FYI: David A. Wheeler teaches a course on developing secure software; one of his slide decks has a summary of some information on security & AI/ML:
    * See: [https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt](https://dwheeler.com/secure-class/presentations/Secure-Software-10-Misc.ppt)
    * <span style="text-decoration:underline;">One discouraging challenge: There are a lot of techniques that don’t work if you’re trying to prevent subversion of AI/ML systems. A lot of academics like to publish techniques that might work, but whether or not they actually work isn’t necessary for publication.</span>
    * <span style="text-decoration:underline;">CNSC keynote that Brian gave on AI and OSS security: https://www.youtube.com/watch?v=VU6OzuHuWQo&t=2s</span>
* <span style="text-decoration:underline;">FYI: SBOM formats are adding information about AI/ML</span>
    * Matt R - cyclone DX SBOM and AI group has some prior work “Model card++”
    * David W - SPDX also has an AI group, which is trying to capture information such as training data sources
* Target  [About OpenSSF](https://openssf.org/about/) 
* AI Security and OSS code and communities:
    * The OpenSSF mission states _“Developers can easily learn secure development practices and are proactively guided by their tools to apply those practices and automatically informed when action is needed to prevent, remediate, or mitigate security issues.” _
* One claim: among developers who have been using Codex since it went into beta later this year, the programming AI is said to have written 40% of the code checked into GitHub is now AI-generated and unmodified
    * Possible source: [https://the-decoder.com/github-ceo-thinks-ai-will-write-majority-of-code-in-just-five-years/](https://the-decoder.com/github-ceo-thinks-ai-will-write-majority-of-code-in-just-five-years/)
    * [https://github.blog/2022-06-21-github-copilot-is-generally-available-to-all-developers/](https://github.blog/2022-06-21-github-copilot-is-generally-available-to-all-developers/) 
        * _"Now Github CEO Thomas Dohmke is giving a glimpse of usage data on Codex: among developers who have been using Codex since it went into beta later this year, the programming AI is said to have written 40 percent of the code. So for every 100 lines of code, 40 are AI-generated."_
* Administrativa
    * Dedicate slack channel for this?
        * Can easily create one in OpenSSF
        * wg_ai_ml_security?
    * Where to store/share docs?
        * Notes, etc. => Google Docs, linked from here.
        * Work product / docs => GitHub Repo
    * Should we be a WG / SIG?

<h3>Potential Topics</h3>




* Proviso - at some point AI will surpass humans. All bets are off
    * Currently this is like having an army of (over-caffeinated) toddlers
    * Will be an army of Einsteins
    * Always 5 years away
* Security of AI models
    * Poisoning attacks on LLMs
    * How can it be attacked? (covered in [Trusted AI – LFAI & Data](https://lfaidata.foundation/projects/trusted-ai/) )
    * [Microsoft docs on AI security / threat modeling / failure modes / etc](https://learn.microsoft.com/en-us/security/engineering/threat-modeling-aiml): 
* Should we look at writing some best practices or guidelines on how open source developers can safely use AI, without leaking confidential information or introducing exploits into their software.
* How can AI attack general infrastructure?
* How is this different from any other scripting?
* How to modify AI generated code?
* How is AI best practice different from human attacker best practice?
    * Everyone needs best practice now - this lowers barrier
    * Quantitatively different, but is it qualitatively different?
* What can we do?
    * Doc search - use AI/ChatGPT
    * Compile more best practices
        * Located where?
    * Cut through hype?
    * Code?
        * Tool automation
        * Spot AI phishing
        * Spot network features
        * Spot supply chain issues

<h3>Potential Threads</h3>


Legal ramifications of chatgpt et al - snippet code.

* There are court courses that may resolve parts of this in the US (but only in the US)

* This is an area that many others are working on. We need to focus on security-focused areas, not generic issues like legal issues.

* AI leveraged to attack OSS communities (spoofing as a contributor)

* AI privacy concerns (leaking information to LLMs)

* AI used to improve security research (vulnerabilities) / AI as a Red Team (AiaaRT)

* AI produces insecure code. ([case in point](https://pbs.twimg.com/media/FuizbxaX0AElDa1?format=jpg&name=large))

Recommendation: Focus on security.

* Links to other working groups

Brian: avoid anthropomorphism, at least to make it clear that humans are in the end in control and accountable.

David: I suggest separating:

#1 How to wisely use AI/ML to generate secure code & secure supply chain (e.g., use AI/ML to detect vulnerabilities, how to take steps to reduce the likelihood of vulnerabilities in AI/ML generated code, how to counter traditional attacks that are being amplified by AI/ML such as spoofing, etc.).

#2 (perhaps never get there) - how to develop AI/ML systems that are themselves secure (that’s a research topic that is generally unsolved - it’s reasonable to do that, someone needs to, but that’s a MUCH bigger task - requires serious research funding for example)

Michael Scovetta: For all the reasons listed above, I think we should work on #2, we’re best placed for it (even though it’s hard!).

Maia: I like the split of #1 vs. #2. I like focusing on #1 at first, the OSS community has some specific equities b/c code is open (re: vuln scanning) and tool development 

How do we secure the AI/ML supply chain? E.g., counter poisoning of training models. David: Although unsolved broadly that is definitely something that has real solutions, we could work on that, perhaps as “item #3: How to select & process training data to counter data poisoning”

Mihai: Have experimented with adding AI training to SLSA.

Nigel Brown: I can work to organize into categories, discuss different ones on different weeks.**​**

<h3>Actions</h3>




* Next meeting - weekly
* Deconflict dashboard meeting (and other OpenSSF meetings) - David will ask operations (Khalil) to set up a Doodle poll for all who attended today, to work out a good meeting time. Meet weekly.
    * Please fill out this Doodle poll for a good meeting time for AI/ML:
    * [https://doodle.com/meeting/participate/id/bqlBpBpa](https://doodle.com/meeting/participate/id/bqlBpBpa)
* Let's create a slack channel (ai_ml_security) and we can rename to wg_ once it's officially a working group?
    * Slack Channel is wg_ai_ml_security. You can visit it here: https://app.slack.com/client/T019QHUBYQ3/C0587E513KR
* We also need a mail group
* Consolidate

<h3>Meeting Rules</h3>




* All participants in OpenSSF meetings are subject to the OpenSSF Code of Conduct. See: [https://openssf.org/community/code-of-conduct/](https://openssf.org/community/code-of-conduct/)
