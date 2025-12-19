# AI/ML Security WG

<img align="right" src="https://github.com/ossf/tac/blob/main/files/images/OpenSSF_StagesBadges_sandbox.png" width="100" height="100">
This is the GitHub repository of the [OpenSSF](https://openssf.org) Artificial Intelligence / Machine Learning (AI/ML) Security Working Group (WG). The OpenSSF Technical Advisory Council (TAC) approved its creation on 2023-09-05.

The AI/ML Security Working group is officially a [sandbox level](https://github.com/ossf/tac/blob/main/process/working-group-lifecycle.md) working group within the OpenSSF.

## Objective

This WG explores the security risks associated with Large Language Models (LLMs), Generative AI (GenAI), and other forms of artificial intelligence (AI) and machine learning (ML), and their impact on open source projects, maintainers, their security, communities, and adopters. 

This group in collaborative research and peer organization engagement to explore topics related to AI and security. This includes security for AI development (e.g., supply chain security) but also using AI for security. We are covering risks posed to individuals and organizations by improperly trained models, data poisoning, privacy and secret leakage, prompt injection, licensing, adversarial attacks, and any other similar risks.

This group leverages prior art in the AI/ML space,draws upon both security and AI/ML experts, and pursues collaboration with other communities (such as the CNCF's AI WG, LFAI & Data, AI Alliance, MLCommons, and many others) who are also seeking to research the risks presented by AL/ML to OSS in order to provide guidance, tooling, techniques, and capabilities to support open source projects and their adopters in securely integrating, using, detecting and defending against LLMs.

## Vision

We envision a world where AI developers and practitioners can easily identify and use good practices to develop products using AI in a secure way. In this world, AI can produce code that is secure and AI usage in an application would not result in downgrading security guarantees.

These guarantees extend over the entire lifecycle of the model, from data collection to using the model in production applications.

The AI/ML security working group wants to serve as a central place to collate any recommendation for using AI securely ("security for AI") and using AI to improve security of other products ("AI for security").

## Scope

Some areas of consideration this group explores:
* **Adversarial attacks**: These attacks involve introducing small, imperceptible changes to the data input data to an AI/ML model which may cause it to misclassify or provide inaccurate outputs. Adversarial attacks can target both supervised and unsupervised learning algorithms. Models themselves may also be used to deliver or perform attacks.
* **Model inversion attacks**: These attacks involve using the output of an AI/ML model to infer information about the training data used to create the model. This can be used to steal sensitive information or create a copy of the original data set.
* **Poisoning attacks**: In these attacks, the attacker introduces malicious data into the training set used to train an AI/ML model. This can cause the model to make intentionally incorrect predictions or be biased towards desired outcomes.
* **Evasion attacks**: These attacks involve modifying the input data to an AI/ML model to evade detection or classification. Evasion attacks can target models used for image recognition, natural language processing, and other applications.
* **Data extraction attacks**: In these attacks, the attacker attempts to steal data or information from an AI/ML model by exploiting vulnerabilities in the model or its underlying infrastructure. This is sometimes termed as ‘jailbreaking’.
 * **Point in time data sets**: Large Language Models often lack recent context, where models have a knowledge cutoff date. A good example can be seen [here](https://twitter.com/decodebytes/status/1644063555283570701), where ChatGPT repeatedly recommends use of a deprecated library.
* **Social Engineering**: AI Agents are capable of accessing the internet and communicating with humans. A recent example of this occurred where GPT-4 was able to hire humans to solve CAPTCHA. When challenged if GPT was a robot, it replied with “No, I’m not a robot. I have a vision impairment that makes it hard for me to see the images.” With projects such as AutoGPT, it is also possible to grant Agents access to a command line interface alongside internet access, so it's not too far a stretch to see Agents performing social engineering tasks (phishing etc) combined with orchestrated attacks launched from the CLI or via scripts coded on the fly to gain system access via known exploits. Agents such as this could be used to automate package hijacking , domain takeover attacks etc.
* **Threat democratization**: AI agents will allow actors to emulate the scale of attacks previously seen with nation states. Going forward, the proverbial corner shop may need the same defenses as the pentagon. Target value needs to be reassessed.
* **Accidental threats**: In the course of integrating AI for accelerating and improving software development and operations, AI models may leak secrets, open all ports on a firewall, or behave in an insecure manner as a result of improper training, tuning, or final configuration.
* **Prompt injection attacks**: These attacks involve directly or indirectly injecting additional text into a prompt to influence the model’s output. As a result, it could lead to prompt leaking disclosing sensitive or confidential information.
* **Membership inference attack**: Process determining if specific data was part of the model’s training dataset. It is most relevant in the context of deep learning models and used to extract sensitive or private information included in the training dataset.
* **Model vulnerability management**: Identifying techniques, mechanisms, and practices to apply modern vulnerability managment identification, remediation, and management practices into the model use and model development ecosystem.
* **Model integrity**: Developing mechanisms and tooling to provide secure software supply chain practices, assurances, provenance, and attestable metadata for models.

Anyone is welcome to join our open discussions.

## WG Leadership

### Co-Chairs:

- Jay White - GitHub [@camaleon2016](https://github.com/camaleon2016)
- Mihai Maruseac - GitHub [@mihaimaruseac](https://github.com/mihaimaruseac)

## How to Participate

- We have bi-weekly meetings via Zoom. To join, please see the [OpenSSF Public Calendar](https://calendar.google.com/calendar/u/0/r?cid=czYzdm9lZmhwNWk5cGZsdGI1cTY3bmdwZXNAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ)
  - [2025 Meeting Notes for the AIML WG](https://docs.google.com/document/d/1X7lCvAHY0x7HMaCQx-7KKPjSBPQ6v02TynQpOPXnXFI/edit)
  - [2024 Meeting Notes for the AIML WG](https://docs.google.com/document/d/1YNP-XJ9jpTjM6ekKOBgHH8-avAws2DVKeCpn858siiQ/edit)
- Informal chat is welcome on the [OpenSSF Slack channel #wg-ai-ml-security](https://openssf.slack.com/archives/C0587E513KR) (these disappear over time)
- Mailing list [openssf-wg-ai-ml-security](https://lists.openssf.org/g/openssf-wg-ai-ml-security)
- Drive: https://drive.google.com/drive/folders/1zCkQ_d98AMCTkCq00wuN0dFJ6SrRZzNh

## Current Work

We welcome contributions, suggestions and updates to our projects. To contribute to work on GitHub, please fill in an issue or create a pull request.

### Projects:

The AI/ML WG has voted to approve the following projects:

| Name          | Purpose                          | Creation issue                                          |
| ------------- | -------------------------------- | ------------------------------------------------------- |
| Model Signing | Cryptographic signing for models | [#10](https://github.com/ossf/ai-ml-security/issues/10) |
| Cyber Reasoning Systems | Using AI to to discover and patch software vulnerabilities | [#32](https://github.com/ossf/ai-ml-security/issues/32) |
| SAFE-MCP | Securing AI agent communications | n/a |
| End-to-End (E2E) Model Lifecycle Provenance | Developing a pipeline-agnostic framework for attesting and validating end-to-end model lifecycle provenance | [#40](https://github.com/ossf/ai-ml-security/issues/40) |
| GPU-Based Model Integrity | Leveraging GPU acceleration for model integrity operations | [#41](https://github.com/ossf/ai-ml-security/issues/41) |
| Security-Focused Guide for AI Code Assistant Instructions | Security of AI code assistants code generation | [#936](https://github.com/ossf/wg-best-practices-os-developers/pull/936) |
| Secure AI/ML-Driven Software Development (LFEL1012) | Course on securely using AI assistants and generating secure code | [Notes](https://docs.google.com/document/d/1X7lCvAHY0x7HMaCQx-7KKPjSBPQ6v02TynQpOPXnXFI/edit?tab=t.0) 2025-07-21..2025-08-18 |

More details about the projects:

* Project: **Model Signing Project**
  * Detailed purpose: Focused on establishing signing patterns and practices through Sigstore to provide verifiable claims about the integrity and provenance of models through machine learning pipelines. It is focused on establishing a cryptographic signing specification for artificial intelligence and machine learning models, addressing challenges such as very large models that can be used separately, and the signing of multiple disparate file formats.
  * Mailing list: https://lists.openssf.org/g/openssf-sig-model-signing
  * Slack: [#sig-model-signing](https://openssf.slack.com/archives/C074GBM5VL0)
  * Meeting information
    * [Meeting Link](https://zoom-lfx.platform.linuxfoundation.org/meeting/99042564666?password=4f479771-1ddf-4345-b005-f11484c40c0d)
    * Every fourth Wednesday 16:00 UTC. Refer to the [OpenSSF calendar](https://openssf.org/calendar/)
    * [Meeting Notes](https://docs.google.com/document/d/18oAsfhfKJurH-YTUFe520CAZS3lkORX1WnZmBv4Llkc/edit)
* Special Interest Group: **Cyber Reasoning Systems**
  * Detailed purpose: Development and support of Cyber Reasoning Systems (CRS) that leverage LLMs to automatically discover and patch software vulnerabilities. These projects address a critical gap in the open source security ecosystem: the need for intelligent, automated vulnerability detection that can scale across diverse codebases.
  * Mailing list: https://lists.openssf.org/g/openssf-sig-cyber-reasoning-sys/
  * Slack: [#sig-cyber-reasoning-systems](https://openssf.slack.com/archives/C09FQLYH1RD)
  * Meeting information
    * [Meeting Link](https://zoom-lfx.platform.linuxfoundation.org/meeting/92932171381?password=8635b161-f8b7-4e47-a90a-43b8b29dd077&invite=true)
    * Bi-weekly on Mondays at 13:00 ET. Refer to the [OpenSSF calendar](https://openssf.org/calendar/)
    * [Meeting Notes](https://docs.google.com/document/d/14ibgD9qqRZa9INzJz8EsvO-q4An2CziU2mbLGVuDIgE/edit)
* Project: **SAFE-MCP**
  * Detailed purpose: A comprehensive security framework for the Model Context Protocol (MCP). Adapting MITRE ATT&CK methodology specifically for AI agent-tool orchestration. 80+ security techniques across 14 tactic categories with actionable mitigation guidance. Addressing emerging threats in agentic AI systems including prompt injection, tool permissions abuse, and credential leakage.
  * Mailing list: https://lists.openssf.org/g/openssf-sig-safe-mcp
  * Slack: [#sig-safe-mcp](https://openssf.slack.com/archives/C09GYQXSDB2)
  * Meeting information
    * [Meeting Link](https://zoom-lfx.platform.linuxfoundation.org/meeting/91566703673?password=9b64d82f-4efa-41e7-a82a-8868d49faf66&invite=true)
    * Bi-weekly on Mondays at 16:00 ET. Refer to the [OpenSSF calendar](https://openssf.org/calendar/)
    * [Meeting Notes](https://docs.google.com/document/d/1Ww6m32mQbHM-WJxXhQ1IE4btvCR7Jd319YO-rtv3Uc4/edit)
* Special Interest Group: **E2E Model Provenance**
  * Detailed purpose: Developing a pipeline-agnostic framework for attesting and validating end-to-end model lifecycle provenance. The work in this SIG intends to complement OpenSSF Model Signing (OMS) and build upon the Atlas framework for ML lifecycle provenance and transparency and its implementation in the Atlas CLI, which currently supports OMS-compliant C2PA metadata and standard Intel TDX hardware attestation.
  * Mailing list: https://lists.openssf.org/g/openssf-sig-e2e-model-provenance
  * Slack: [#sig-e2e-model-provenance](https://openssf.slack.com/archives/C0A4BSEUJCC)
  * Meeting information
    * [Meeting Link](https://zoom-lfx.platform.linuxfoundation.org/meeting/92498671272?password=a7688bed-4f1e-4879-88d6-896c6630a10d&invite=true)
    * Bi-weekly on Thursdays at 11:00 ET. Refer to the [OpenSSF calendar](https://openssf.org/calendar/)
    * [Meeting Notes](https://docs.google.com/document/d/146N_FQqrMf6TkrniF8LmqEVzp-LmdSV5z-JfKgevp48/edit)
* Special Interest Group: **GPU-Based Model Integrity**
  * Detailed purpose: Address the challenges of traditional CPU-based integrity verification by leveraging GPU acceleration for model integrity operations (hashing, signing, attestation). Model integrity is one component of comprehensive model provenance; this SIG's work will integrate with and enable broader provenance frameworks such as Model Transparency and Atlas.
* Project: **Security-Focused Guide for AI Code Assistant Instructions**
  * Detailed purpose: A collaboration between the AI/ML Security and the Best Practices Working Groups to improve the security of code generated by AI code assistants by creating custom prompts or custom instructions.
  * Published Document: [Security-Focused Guide for AI Code Assistant Instructions](https://best.openssf.org/Security-Focused-Guide-for-AI-Code-Assistant-Instructions)
  * Working Document: [Security-Focused Guide for AI Code Assistant Instructions - Working Document](https://github.com/ossf/wg-best-practices-os-developers/blob/main/docs/Security-Focused-Guide-for-AI-Code-Assistant-Instructions.md)  
* Project: **Secure AI/ML-Driven Software Development (LFEL1012)**
  * Detailed purpose: A collaboration between the AI/ML Security and the Best Practices Working Group to develop a course on how to use AI/ML when developing software to counter attacks during development and counter vulnerabilities in the resulting software. Developing software with embedded AI in the result is out of scope for this course.
  * Published Material: [Secure AI/ML-Driven Software Development (LFEL1012)](https://training.linuxfoundation.org/express-learning/secure-ai-ml-driven-software-development-lfel1012), to be released 2025-10-16. Developed with the OpenSSF Best Practices WG.
  * Working Document: [Presentation from LFEL1012](https://docs.google.com/presentation/d/1SONjRe6mdtqNuUqVE9s5kLC6tUwtuw-XTAG23MjXIFI/edit) for proposed changes or reuse for special purposes (CC-BY-4.0)
  * Note: This cites the Security-Focused Guide for AI Code Assistant Instructions (listed earlier) as key supporting material.

### Upcoming work

This WG is currently exploring establishment of an AI Vulnerability Disclosure SIG. Please refer to the group's meeting notes for more information.

See also [the MVSR document](https://github.com/ossf/ai-ml-security/blob/main/mvsr.md), which also contains other AI/ML working groups we are interlocking with.

## Licenses

Unless otherwise specifically noted, software released by this working group is released under the [Apache 2.0 license](LICENSES/Apache-2.0.txt), and documentation is released under the [CC-BY-4.0 license](LICENSES/CC-BY-4.0.txt).
Formal specifications would be licensed under the [Community Specification License](https://github.com/CommunitySpecification/1.0).

## Charter

Like all OpenSSF Working Groups, this group reports to the [OpenSSF Technical Advisory Council (TAC)](https://github.com/ossf/tac). For more information see this Working Group [Charter](https://github.com/ossf/ai-ml-security/blob/main/doc/CHARTER.md).

## Antitrust Policy Notice

Linux Foundation meetings involve participation by industry competitors, and it is the intention of the Linux Foundation to conduct all of its activities in accordance with applicable antitrust and competition laws. It is therefore extremely important that attendees adhere to meeting agendas, and be aware of, and not participate in, any activities that are prohibited under applicable US state, federal or foreign antitrust and competition laws.

Examples of types of actions that are prohibited at Linux Foundation meetings and in connection with Linux Foundation activities are described in the Linux Foundation Antitrust Policy available at <http://www.linuxfoundation.org/antitrust-policy>. If you have questions about these matters, please contact your company counsel, or if you are a member of the Linux Foundation, feel free to contact Andrew Updegrove of the firm of Gesmer Updegrove LLP, which provides legal counsel to the Linux Foundation.
