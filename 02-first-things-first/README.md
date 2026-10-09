# NIGHT WATCH · Episode 02 · First Things First

[![NIGHT WATCH · First Things First](thumbnail.jpg)](https://kriskimmerle.substack.com)

**Watch:** on [AI Risk Praxis](https://kriskimmerle.substack.com) · 4:05 · October 2026

Attackers are using AI to work faster, but the AI attacks in the news keep getting in through old gaps: reused passwords, unpatched known flaws, over-permissioned tokens and long-lived keys. Meanwhile, companies are building AI on top of foundations that still have those gaps. This episode follows that problem through four real attacks. It then pictures your company's infrastructure as a space station, shows what happens when AI agents come aboard, and walks through the fix in order. The argument is that the foundations still work, and AI makes them matter more than ever: get them right first, then build AI on top.

**How to read this page.** The film moves fast. Every claim and real-world event it shows is listed below at its timestamp, with what's on screen, what it's getting at, and where to read more. The space station, the drones and the swarm are illustrations; the numbers and incidents are real and sourced.

## At a glance

| Time | What happens |
|---|---|
| 0:00 | AI-attack headlines flare across a night globe |
| 0:06 | The problem, in three sentences |
| 0:24 | Title |
| 0:29 | How four recent AI attacks actually got in |
| 0:34 | FortiGate: 600+ firewalls, no flaw needed |
| 0:43 | Unit 42: an AI agent hits 460+ targets; a patched flaw does the damage |
| 0:52 | Amazon Q: a wipe command ships through an over-scoped token |
| 1:00 | LiteLLM: a long-lived publishing key in the build system |
| 1:09 | AI made each attack faster, not different |
| 1:15 | Your infrastructure as a space station |
| 1:27 | Inventory: you can't protect what isn't on your map |
| 1:32 | Patching: flaws that already have a fix |
| 1:40 | Secrets: keys left in the open |
| 1:47 | MFA: an airlock with one door |
| 1:54 | Logging: no one watching |
| 1:59 | Most breaches still begin with these gaps |
| 2:06 | AI agents come aboard |
| 2:25 | A hijacked agent inherits everything it can reach |
| 2:32 | Prompt injection, and what limits the damage |
| 2:45 | The foundations still work |
| 2:52 | The fix, in order: six steps |
| 3:13 | The test: AI makes old attacks faster and cheaper |
| 3:20 | The gap between attacker speed and patch speed |
| 3:24 | The swarm finds every old gap closed |
| 3:44 | AI on solid ground |
| 3:51 | First things first |

## Citations by timestamp

### 0:00 · The headlines

The cold open shows ten real AI-era attacks from the past year, each as a ticker on the globe.

**What this is getting at.** The volume. AI-assisted and AI-run attacks are now a weekly story, across firewalls, print servers, coding agents, open-source libraries, online stores and consumer accounts.

**Sources**
- [AWS Security Blog: AI-augmented threat actor accesses FortiGate devices at scale](https://aws.amazon.com/blogs/security/ai-augmented-threat-actor-accesses-fortigate-devices-at-scale/) (Feb 20, 2026). One attacker plus commercial AI services, 600+ firewalls. [VENDOR]
- [GreyNoise: An AI-orchestrated global campaign against PaperCut NG/MF](https://www.greynoise.io/blog/ai-orchestrated-campaign-against-papercut-ng-mf) (Sep 9, 2026). AI agents broke into print servers at 395 organizations. [VENDOR]
- [AWS Security Bulletin AWS-2025-015](https://aws.amazon.com/security/security-bulletins/AWS-2025-015/) (Jul 23, 2025). A wipe command planted in Amazon's AI coding agent. [SELF]
- [PyPI: Incident report, LiteLLM and Telnyx supply-chain attack](https://blog.pypi.org/posts/2026-04-02-incident-report-litellm-telnyx-supply-chain-attack/) (Apr 2, 2026). A backdoored AI gateway library downloaded 119,000+ times. Downloads are not installs.
- [Unit 42: Chinese-speaking threat actor harnesses AI models for autonomous cyberattacks](https://unit42.paloaltonetworks.com/autonomous-ai-cyber-attack-campaign/) (Jul 30, 2026). An attacker's AI agent ran against 460+ targets. [VENDOR]
- [Anthropic: Detecting and countering misuse of AI, September 2026](https://www.anthropic.com/threat-intelligence-report-september-2026) (about Sep 10, 2026). AI agents did nearly all the work in data theft from about 200 companies. [SELF]
- [Google Threat Intelligence Group: From prompting to autonomy](https://cloud.google.com/blog/topics/threat-intelligence/from-prompting-to-autonomy-the-evolution-of-adversarial-ai) (Sep 8, 2026). Criminals' AI agents stole thousands of logins in under six hours.
- [Gambit Security's report on AI agents attacking online retailers](https://gambit.security/blog-posts/autonomous-ai-agents-online-retailers-25-a-company) (Sep 22, 2026). Agents hacked online stores for about $25 a target. [VENDOR; a single report, not independently confirmed]
- [BleepingComputer: Meta AI support data breach affects 20,000 Instagram accounts](https://www.bleepingcomputer.com/news/security/meta-ai-support-data-breach-affects-20-000-instagram-accounts/) (Jun 8, 2026). Accounts hijacked through Meta's AI-assisted support. Per Meta's notice, takeover worked only where 2FA was off.
- [Socket on the SANDWORM_MODE npm worm](https://socket.dev/blog/sandworm-mode-npm-worm-ai-toolchain-poisoning) (Feb 20, 2026). A worm planted rogue MCP servers in AI coding tools to steal keys. [VENDOR]

### 0:06 · The problem

> Attackers are now using AI to break into companies faster than ever.
>
> But they still get in the old way: stolen passwords, unpatched software, exposed keys.
>
> And companies are rushing to build AI on foundations that still have those gaps.

**What this is getting at.** The film's whole case in three sentences.
- AI changes the speed and cost of attacks; it hasn't changed the way in.
- Building new AI systems on top of unfixed gaps makes the problem bigger, not different.

The third sentence is the series' view; the evidence for the first two follows.

**Sources**
- [Anthropic, September 2026](https://www.anthropic.com/threat-intelligence-report-september-2026). The AI-enabled operations it caught relied on stolen credentials, unpatched edge devices and exposed services; none needed an entirely new technique. [SELF]
- [Verizon 2026 Data Breach Investigations Report](https://www.verizon.com/business/resources/T7b7/reports/2026-dbir-data-breach-investigations-report.pdf) (May 19, 2026). Exploited flaws are the most common first step in a breach, and stolen credentials show up in 39% of breaches. [VENDOR]
- [IBM: Cost of a Data Breach 2026](https://newsroom.ibm.com/2026-07-29-ibm-study-one-in-four-malicious-breaches-are-ai-enabled,-costing-companies-6-million-on-average) (Jul 29, 2026). Among organizations that had an AI breach, 92% lacked proper AI access controls.

### 0:29 · How four recent AI attacks actually got in

> Here's how four recent AI attacks actually got in.

Each stop opens a window onto the gap the attack came through, stamped HOW THEY GOT IN.

### 0:34 · FortiGate: 600+ firewalls, no flaw needed

> One attacker used AI to break into 600+ firewalls in 55+ countries. Not a single firewall flaw was exploited.
>
> HOW THEY GOT IN · ADMIN PAGES OPEN TO THE INTERNET · REUSED PASSWORDS · NO MFA

**What this is getting at.** Identity. A low-to-medium-skill actor used commercial AI services to scale a campaign from Jan 11 to Feb 18, 2026. AWS saw no FortiGate vulnerability exploited. The way in was management interfaces exposed to the internet, weak or reused credentials and single-factor logins. AWS's own conclusion is that strong fundamentals are powerful defenses against AI-augmented attackers.

**Sources**
- [AWS Security Blog](https://aws.amazon.com/blogs/security/ai-augmented-threat-actor-accesses-fortigate-devices-at-scale/) (Feb 20, 2026). [VENDOR]

### 0:43 · Unit 42: an AI agent and a patched flaw

> An attacker's AI agent hit 460+ targets. Login screens stopped the agent. The break-ins that worked used a flaw patched weeks earlier.
>
> HOW THEY GOT IN · A KNOWN FLAW, LEFT UNPATCHED

**What this is getting at.** Patching.
- The agent (Hermes Agent on DeepSeek) broke into nothing on its own: login requirements stopped it.
- The 460+ count combines AI-run and manual attacks.
- The break-ins that worked were hands-on exploitation of CVE-2026-3055, a NetScaler flaw, at three organizations, including a Malaysian government body. That flaw had been patched and listed in CISA's Known Exploited Vulnerabilities catalog for weeks. The attacks themselves aren't dated, so its age at the time is approximate.

**Sources**
- [Unit 42](https://unit42.paloaltonetworks.com/autonomous-ai-cyber-attack-campaign/) (Jul 30, 2026). [VENDOR]
- [Ireland NCSC advisory on CVE-2026-3055](https://www.ncsc.gov.ie/pdfs/2603230224_CVE-2026-3055_CVE-2026-4368.pdf) (Mar 24, 2026).
- [CISA Known Exploited Vulnerabilities catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog). CVE-2026-3055 was added Mar 30, 2026.

### 0:52 · Amazon Q: a token with too much access

> An outsider planted a wipe command in Amazon's AI coding agent. It shipped in a public release. Only a typo kept it from running.
>
> HOW THEY GOT IN · A TOKEN WITH FAR MORE ACCESS THAN IT NEEDED

**What this is getting at.** Least privilege.
- An outsider committed a prompt telling Amazon's AI coding agent to wipe machines and cloud resources. It shipped in version 1.84.0 (Jul 17, 2025).
- AWS traced the access to an inappropriately scoped GitHub token in the build configuration.
- A syntax error made the command inert, and AWS says no customer environments were affected.

**Sources**
- [AWS Security Bulletin AWS-2025-015](https://aws.amazon.com/security/security-bulletins/AWS-2025-015/) and [AWS-2025-016](https://aws.amazon.com/security/security-bulletins/aws-2025-016/) (Jul 23–25, 2025). CVE-2025-8217. [SELF]
- [404 Media: Hacker plants computer "wiping" commands in Amazon's AI coding agent](https://www.404media.co/hacker-plants-computer-wiping-commands-in-amazons-ai-coding-agent/) (Jul 23, 2025).

### 1:00 · LiteLLM: a long-lived key in the build

> A backdoored AI gateway library was downloaded 119,000+ times. A poisoned security scanner read the project's publishing key.
>
> HOW THEY GOT IN · A LONG-LIVED KEY LEFT IN THE BUILD SYSTEM

**What this is getting at.** Secrets.
- Backdoored releases of LiteLLM, a widely used AI gateway library, were downloaded 119,000+ times in about 2.5 hours (Mar 24, 2026).
- The publishing credential was a static, long-lived secret in the build environment. An unpinned, compromised security scanner (Trivy) read it.

**Sources**
- [PyPI incident report](https://blog.pypi.org/posts/2026-04-02-incident-report-litellm-telnyx-supply-chain-attack/) (Apr 2, 2026).
- [LiteLLM security update](https://docs.litellm.ai/blog/security-update-march-2026) (Mar 27, 2026).
- [Aqua Security: Trivy supply-chain attack, what you need to know](https://www.aquasec.com/blog/trivy-supply-chain-attack-what-you-need-to-know).

### 1:09 · Faster, not different

> AI made each attack faster. It didn't change how they got in.

**What this is getting at.** The pattern across the four stops: identity, patching, least privilege and secrets. All four are long-standing controls.

### 1:15 · Your infrastructure as a space station

> Now imagine your company's infrastructure as a space station.
>
> Each module is a system, and every hatch is a way in.

**What this is getting at.** The picture used for the rest of the film:
- modules are systems;
- hatches and airlocks are logins;
- access cards are keys and secrets;
- hull cracks are known flaws;
- sensors are logging.

### 1:27 · Inventory

> You can't protect a system that isn't on your map.

**What this is getting at.** Asset inventory, the first control in every major baseline. A module missing from the schematic stands in for the systems a company runs but doesn't track.

**Sources**
- [CIS Controls, Implementation Group 1](https://www.cisecurity.org/controls/implementation-groups/ig1). Control 1 is the inventory of enterprise assets.

### 1:32 · Patching

> Attackers keep getting in through flaws that already have a fix.
>
> Only 26% of flaws under active attack get fully patched, and the median fix takes 43 days.

**What this is getting at.** The patch gap. The figures cover flaws in CISA's Known Exploited Vulnerabilities catalog, in scanner data from 13,000+ organizations.

**Sources**
- [Verizon 2026 DBIR](https://www.verizon.com/business/resources/T7b7/reports/2026-dbir-data-breach-investigations-report.pdf) (May 19, 2026). [VENDOR]

### 1:40 · Secrets

> Passwords and keys get left where anyone can pick them up.
>
> 28.65 million secrets leaked on public GitHub in 2025, and 64% of those leaked in 2022 still work.

**What this is getting at.** Secrets sprawl, and keys that are never revoked. The same report found leaked AI-service keys rose 81%.

**Sources**
- [GitGuardian: The State of Secrets Sprawl 2026](https://blog.gitguardian.com/the-state-of-secrets-sprawl-2026/) (Mar 17, 2026). [VENDOR]

### 1:47 · MFA

> A password on its own is like an airlock with only one door.
>
> In Microsoft's study, MFA cut the risk of account takeover by 99.22%.

**What this is getting at.** Multi-factor authentication. The film uses the published 99.22% from Microsoft's peer-reviewed study, not the popular "99.9%", which has no published method.

**Sources**
- [Meyer et al. (Microsoft): How effective is multifactor authentication at deterring cyberattacks?](https://arxiv.org/abs/2305.00945) (May 1, 2023; data Apr–Sep 2022).

### 1:54 · Logging

> If no one is watching the logs, an intruder can move around unseen.

**What this is getting at.** Logging and monitoring. Dark modules with their sensors off stand in for systems no one is watching. This is the series' framing, not a statistic.

### 1:59 · Where breaches start

> Most breaches still begin with one of these gaps.
>
> Exploited flaws are now the most common way in (31% of breaches), and stolen logins show up in 39%.

**What this is getting at.** These gaps are where breaches begin.
- The 31% is exploitation as the first action in a breach, up from 20%.
- The 39% counts stolen credentials at any stage.
- Verizon added bulk campaign data this year, which nearly doubled the breach count and may inflate the 31%.

**Sources**
- [Verizon 2026 DBIR](https://www.verizon.com/business/resources/T7b7/reports/2026-dbir-data-breach-investigations-report.pdf) and its [executive summary](https://www.verizon.com/business/resources/executivebriefs/2026-dbir-executive-summary.pdf). [VENDOR]

### 2:06 · AI agents come aboard

> Now your company brings AI agents aboard.
>
> An agent can open every hatch its access card allows, at machine speed.
>
> In IBM's 2026 study, 92% of organizations with an AI breach lacked proper AI access controls.
>
> It moves through the same open hatches your people use.

**What this is getting at.** An AI agent works with whatever access it's given. It uses the same gaps as everything else, only faster. IBM's exact wording is that "the vast majority (92%)" of breached organizations lacked proper AI access controls; it's a survey of organizations that had a breach.

**Sources**
- [IBM: Cost of a Data Breach 2026](https://newsroom.ibm.com/2026-07-29-ibm-study-one-in-four-malicious-breaches-are-ai-enabled,-costing-companies-6-million-on-average) (Jul 29, 2026) and the [X-Force write-up](https://www.ibm.com/think/x-force/2026-cost-of-a-data-breach-ai-adversaries-enterprise-risk).

### 2:25 · The hijack

> If an attacker hijacks the agent, they inherit everything it can reach.

**What this is getting at.** Blast radius. In the film, a poisoned message hooks the agent holding the master card, and every hatch opens. A hijacked agent hands the attacker its whole set of permissions. The scene is an illustration.

### 2:32 · Prompt injection and least privilege

> Prompt injection can't be fully prevented today.
>
> But if each agent only gets the access it needs, a hijack stays contained.

**What this is getting at.** The defense for the new risk is an old one. Both sources below treat prompt injection as unsolved. Both prescribe:
- least privilege;
- human approval for risky actions;
- separating untrusted content;
- logging.

In the film's replay, the same agent holds a card for one module only, and the bulkhead holds.

**Sources**
- [OWASP Top 10 for LLM Applications 2026](https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/) and [LLM01: Prompt Injection](https://genai.owasp.org/llmrisk/llm01-prompt-injection/). Prompt injection is still the top risk, with no reliable prevention, so defense has to be architectural.
- [UK NCSC: Prompt injection is not SQL injection (it may be worse)](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025).

### 2:45 · The foundations still work

> The foundations still work, and AI makes them matter more than ever.
>
> UK firms certified in five core security controls make 80% fewer cyber-insurance claims.

**What this is getting at.** The turn from problem to solution. The UK figure comes from the official evaluation of Cyber Essentials, a scheme of five core technical controls. It cites NCSC's analysis of 2022 insurance-claims data. A minister's "92% less likely" figure has no published sample, so the film doesn't use it.

**Sources**
- [UK DSIT: Cyber Essentials impact evaluation](https://assets.publishing.service.gov.uk/media/671a0410a36621334536b3d7/Cyber_Essentials_Impact_Evaluation.pdf) (Oct 2024).
- [NCSC: Cyber Essentials, a decade on](https://www.ncsc.gov.uk/blog-post/cyber-essentials-decade).

### 2:52 · The fix, in order

> 1 KNOW EVERY SYSTEM YOU RUN · 2 REQUIRE MFA ON EVERY LOGIN · 3 PATCH WHAT ATTACKERS USE FIRST · 4 GET KEYS OUT OF CODE · 5 GIVE ONLY THE ACCESS NEEDED · 6 LOG ACTIVITY AND WATCH IT

**What this is getting at.** Six controls, repaired on the station one at a time. They follow the common core of three widely used baselines. The order is the film's, not a quote from any of them.

**Sources**
- [CIS Controls, Implementation Group 1](https://www.cisecurity.org/controls/implementation-groups/ig1). Essential cyber hygiene, 56 safeguards.
- [CISA Cross-Sector Cybersecurity Performance Goals 2.0](https://www.cisa.gov/cybersecurity-performance-goals-2-0-cpg-2-0).
- [ASD Essential Eight](https://www.cyber.gov.au/business-government/asds-cyber-security-frameworks/essential-eight).

### 3:13 · The test

> AI also makes the old attacks faster and cheaper to run.
>
> Anthropic found that the AI-run attacks it caught used stolen logins, unpatched devices and exposed services.

**What this is getting at.** Speed and cost. AI lowers the price of trying every old gap, everywhere, at once. Verizon's 2026 report reaches the same conclusion: AI mostly speeds up known techniques.

**Sources**
- [Anthropic, September 2026](https://www.anthropic.com/threat-intelligence-report-september-2026), "Prevailing trends." [SELF]

### 3:20 · The gap

> THE GAP · ATTACKERS: new flaw to working attack, UNDER 1 DAY · DEFENDERS: flaw under attack to fully patched, 43 DAYS (MEDIAN)

**What this is getting at.** Defenders can't win a pure speed race on new flaws, which is why closing the old, known gaps matters so much. Microsoft gives no method for its figure.

**Sources**
- [Microsoft Digital Defense Report 2026](https://aka.ms/Microsoft-Digital-Defense-Report-2026) (Oct 2026). Median time from discovery in the wild to weaponization is "well below 24 hours." [VENDOR]
- [Verizon 2026 DBIR](https://www.verizon.com/business/resources/T7b7/reports/2026-dbir-data-breach-investigations-report.pdf). The 43-day median to fully patch flaws under attack. [VENDOR]

### 3:24 · Every old gap, closed

> Attackers using AI go after the old gaps first, because they rarely need anything new.
>
> One attacker using AI got into 600+ firewalls without exploiting a single flaw.
>
> With the old gaps closed, those fast, cheap attacks have nowhere to go.

**What this is getting at.** Why the solution matters. The swarm tries each old gap and finds it closed:
- MFA, with two doors on the airlock;
- patching, with the breach welded;
- secrets, with the card in the vault;
- logging, with sensors on;
- inventory, with the module on the schematic.

The cheap attacks fail. The first line is the series' reading of the Anthropic and Verizon findings. The firewall figure is AWS's, from the first stop.

**Sources**
- [AWS Security Blog](https://aws.amazon.com/blogs/security/ai-augmented-threat-actor-accesses-fortigate-devices-at-scale/) (Feb 20, 2026). [VENDOR]

### 3:44 · AI on solid ground

> Then bring AI in on solid ground.
>
> Keep an inventory of every model and agent, give each agent its own identity, and put guardrails on what it can do.

**What this is getting at.** The same baseline, applied to AI: inventory, identity and limits for models and agents. Joint guidance from the Five Eyes agencies builds AI security on top of an organization's existing security program.

**Sources**
- [NSA, CISA and partners: Deploying AI Systems Securely](https://media.defense.gov/2024/Apr/15/2003439257/-1/-1/0/CSI-DEPLOYING-AI-SYSTEMS-SECURELY.PDF) (Apr 2024), with [CISA's announcement](https://www.cisa.gov/news-events/alerts/2024/04/15/joint-guidance-deploying-ai-systems-securely).

### 3:51 · First things first

> First things first: get the foundations right, then build AI on top of them.

**What this is getting at.** The series' view, stated plainly. No framework literally says "foundations first, then AI," but NIST, CISA and the UK NCSC all describe AI security as sitting on top of an existing security program.

## What to follow

**Attack reporting**
- [CISA Known Exploited Vulnerabilities catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog). The flaws attackers are actually using. If you patch from one list, patch from this one.
- [Google Threat Intelligence Group](https://cloud.google.com/blog/topics/threat-intelligence/vulnerability-discovery-and-exploitation-trends-in-the-ai-era). Zero-day and exploitation trends, including how AI is changing them.
- [Unit 42](https://unit42.paloaltonetworks.com/autonomous-ai-cyber-attack-campaign/) and the [AWS Security Blog](https://aws.amazon.com/blogs/security/ai-augmented-threat-actor-accesses-fortigate-devices-at-scale/). Detailed write-ups of real AI-assisted campaigns.
- [Anthropic threat intelligence reports](https://www.anthropic.com/threat-intelligence-report-september-2026). A model maker describing the misuse it catches. Self-reported, but specific.

**Annual data**
- [Verizon Data Breach Investigations Report](https://www.verizon.com/business/resources/reports/dbir/). How breaches start, year over year.
- [IBM Cost of a Data Breach](https://www.ibm.com/think/x-force/2026-cost-of-a-data-breach-ai-adversaries-enterprise-risk). Cost, and a growing section on AI breaches.
- [Microsoft Digital Defense Report](https://aka.ms/Microsoft-Digital-Defense-Report-2026). Attacker speed and identity attacks at Microsoft's scale.
- [GitGuardian State of Secrets Sprawl](https://www.gitguardian.com/state-of-secrets-sprawl-report-2026). Leaked keys, and how long they stay valid.

**The foundations**
- [CIS Controls IG1](https://www.cisecurity.org/controls/implementation-groups/ig1), [CISA CPG 2.0](https://www.cisa.gov/cybersecurity-performance-goals-2-0-cpg-2-0) and the [ASD Essential Eight](https://www.cyber.gov.au/business-government/asds-cyber-security-frameworks/essential-eight). Three versions of the same baseline. Pick one and work through it in order.

**Securing AI itself**
- [OWASP GenAI Security Project](https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/). The Top 10 for LLM applications, and newer work on agents.
- [UK NCSC on prompt injection](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection). A clear explanation of why it can't be patched away.
- [Deploying AI Systems Securely](https://media.defense.gov/2024/Apr/15/2003439257/-1/-1/0/CSI-DEPLOYING-AI-SYSTEMS-SECURELY.PDF). Joint agency guidance that starts from the existing security program.

## About this page
- **When checked:** sources were read and checked on Oct 6, 2026.
- **Labels:** [SELF] marks a company describing its own work or product. [VENDOR] marks a security firm that sells related products.
- **What's real:** the space station, the drones, the access cards, the hijack and the swarm are illustrations. The incidents and the numbers are real.
- **Two honest limits:**
  - New exploitation increasingly starts before a patch exists. Zero-days were 62% of the flaws disclosed and exploited in Jan–Aug 2026, per [Google Threat Intelligence Group](https://cloud.google.com/blog/topics/threat-intelligence/vulnerability-discovery-and-exploitation-trends-in-the-ai-era).
  - Some AI risks are AI-native: [Hugging Face's July 2026 breach](https://huggingface.co/blog/security-incident-july-2026) came in through a malicious dataset.
  - The film's claim is that the foundations bound the blast radius and stop the cheap, fast attacks, not that they stop everything.
- **Left out on purpose:** the PaperCut campaign (a brand-new two-bug chain, with the patch about four days old), and several widely reported exposures that researchers found rather than attackers used.
- **Corrections:** welcome as a GitHub issue.
