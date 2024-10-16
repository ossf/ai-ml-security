# MVSR Artificial Intelligence/Machine Learning (AI/ML) WG
Our mission is to enable security for Open Source AI workflows (training
pipelines, AI deployments) and enable using AI for security of Open Source
software. We also maintain some focus on experimentation for tools and
techniques at the intersection of AI and security.

Our vision is to be the central place for collating any recommendations for
using AI securely ("security for AI" vision) and for using AI to improve
security of other OSS software products ("AI for security" vision).

The developing scope involves analyzing open source AI/ML data sets, data models
and OSS code mashups used in AI/ML to articulate the specific security concerns
and controls for the subset of OSS AI/ML workloads. This is important because
the accelerated adoption of AI/ML has an OSS and security component that is not
well understood, and OpenSSF can play an industry leading position.

Currently, we have a [model signing project](https://github.com/ossf/ai-ml-security/issues/10)
with the aim of creating a solution that can be used to sign ML models during
training and verify the integrity of these models before deploying them in
applications. This is at the foundation for any supply chain statement we can
make about AI/ML, and we are planning to extend this to datasets too.
Furthermore, we're exploring expanding the model signing work to cover in-toto,
witness, C2PA and other deeper integrations.

We are planning to potentially explore a “security slam” for existing OpenSSF
tooling to see how it protects/applies to OSS AIML workloads; develop OSS
security patterns for use cases where OSS AIML components are integrated in the
supply chain. This is similar to the discussion we've had about how OpenSSF
projects can be used in the context of NIST SP 800-218A standard for GenAI and
Dual-Use foundation models.

Finally, we are interlocking with various other groups, since new AI/ML
communities are continuously springing up. A summary of these groups and how we
relate to them is given below:

* **[OWASP Foundation](https://owasp.org/)**
  * _AI/ML Security work being done_: The OWASP foundation more broadly aims to improve the security of software through its community-led open source software projects. They have an [AI Security Guide](https://owasp.org/www-project-ai-security-and-privacy-guide/). [OWASP Project Machine Learning Security Top 10](https://owasp.org/www-project-machine-learning-security-top-10/) provides developer centered information about the top known cybersecurity risks for open source machine learning, with a description, example attack scenario, and a suggestion of how to prevent.
  * _Difference_: Content does not provide indepth technical recommendations for practical implementation within their security documentation. OWASP Large Language Model Applications Top 10 provides the same developer centered information for LLMs. These are all vulnerability descriptions, not developer best practices.
  * _Partnership/Collaboration Opportunity_: Education and outreach opportunities are critical here. Developers have to understand both how security, vulnerability and bugs impact their software security stance, which the OWASP Top 10s do well. Building technical best practices to prevent vulnerabilities is where OSSF can be an excellent partner in getting critical information about these unique vulnerabilities.
* **[The LFAI Security Committee](https://wiki.lfaidata.foundation/display/DL/ML+Security+Committee)**
  * _AI/ML Security work being done_: Focus on AI and ML security
  * _Difference_: LFAI does not focus on systemic problems of AI/ML and the Open Source Supply Chain, which is where OSSF’s WG would have the most critical impact. LFAI supports AI and Data open source projects through incubation, education, and best practices. However, their community is focused on exactly what most developer foundations must be: project acceleration, not security. OpenSSF is the foundation of security expertise, and we need to develop a cohort of security-first engineering practices. This can be done in tandem with LFAI, but it’s simple: the end users are LFAI, but the ability to mobilize security education, intervention and open source supply chain hardening for this evolving sector is clearly within the remit, and expertise, of OpenSSF.
  * _Partnership/Collaboration Opportunity_: Clear candidates for coordination for best practices for both end users, open source maintainers, and contributor communities.
* **[AI Alliance](https://thealliance.ai/)**
  * _AI/ML Security work being done_: This group has an AI Trust and Safety group that is focused on understanding potential trust and safety issues associatied with AI and developing mitigation strateigies for these.
  * _Difference_: This group is more focused on the Safety and Trustworthiness aspects of AI, with a smaller focus on Security.

For a full list, please see [this spreadsheet](https://docs.google.com/spreadsheets/d/1XOzf0LwksHnVeAcgQ7qMAmQAhlHV2iEf4ICvUwOaOfo/edit?gid=0#gid=0).
For updates from each interlock, occuring at every meeting, please see [the meeting notes](https://docs.google.com/document/d/1YNP-XJ9jpTjM6ekKOBgHH8-avAws2DVKeCpn858siiQ/edit?tab=t.0).
