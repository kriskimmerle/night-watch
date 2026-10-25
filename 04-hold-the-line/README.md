# NIGHT WATCH · Episode 04 · Hold the Line

[![NIGHT WATCH · Hold the Line](thumbnail.jpg)](https://kriskimmerle.substack.com)

**Watch:** on [AI Risk Praxis](https://kriskimmerle.substack.com) or LinkedIn · 11:22 · October 2026

An AI guardrail is software that sits outside a model and checks what goes in, what comes out and what the model is about to do. This episode starts with the highway guardrails the name comes from. They're crash tested against a set kind of hit, and something much heavier can go through them. AI guardrails work the same way. The film explains the three kinds of check, why people attack AI, and why the problem keeps growing as AI connects to more systems. It meets the people who attack AI on purpose, and the robots that are turning a software risk into a physical one. Guardrails lower that risk, but they can never catch everything, because there are far too many possible prompts to test and attacks adapt. They're still worth running, for the same reasons teams run firewalls and antivirus. They raise the cost of an attack, leave a record of what they catch and show reasonable care, and different kinds of checks together catch what one alone would miss. The last part covers how teams deploy them, from the threat model and stacked checks to what each check costs in time, money and mistakes, what happens when a checker breaks and what the big clouds sell, and it ends on limiting what the system can do.

**How to read this page.** The film moves fast. Every claim and real-world event it shows is listed below at its timestamp, with what's on screen, what it's getting at, and where to read more. A narrator tells the story in his own words, and the quotes here are the on-screen captions, which differ from the narration on purpose. The highway, the crash-test cars, the courier, Microduck, the robot arm, the AI agent character and the x-ray diagrams are illustrations. The crash test follows the real test standard, and the incidents and numbers are real and sourced.

## At a glance

| Time | What happens |
|---|---|
| 0:00 | AI Risk Praxis presents |
| 0:08 | A highway guardrail crash test |
| 0:22 | The rail catches the pickup and steers it back |
| 0:30 | A much heavier truck goes through |
| 0:40 | AI has guardrails too |
| 0:50 | Title |
| 0:56 | An aside on the series' changing look and sound, and the little red dot that points to what matters |
| 1:28 | What an AI guardrail is, seen in an x-ray view |
| 1:39 | Orders hidden in what the AI reads, called prompt injection |
| 1:51 | What shouldn't leave, like a card number |
| 1:57 | An agent's refund held until a person says yes |
| 2:07 | Checks that steer sensitive topics |
| 2:21 | The three kinds of check |
| 2:24 | Rules, instant and free, and the rewording that slips past |
| 2:47 | Small models, each with one job |
| 3:01 | A second AI acting as a judge |
| 3:12 | Why anyone attacks an AI, starting with the $1 SUV |
| 3:24 | It doesn't feel like breaking in |
| 3:40 | Words that take an agent's power and turn it on you |
| 3:51 | Hidden instructions in résumés, papers and links |
| 4:02 | Known prompt-injection flaws, 2 in 2023 and 98 this year |
| 4:16 | Every new connection is a new place to land |
| 4:25 | Attackers adapt |
| 4:35 | Prompt injection again, then jailbreaking and red teaming |
| 4:50 | Pliny the Liberator |
| 5:07 | TIME100 AI, 2025 |
| 5:14 | A robot dog hijacked at Black Hat |
| 5:29 | Microduck, a $399 robot duck |
| 5:46 | Robots talked into unsafe actions |
| 6:00 | A software risk today, a physical one soon |
| 6:12 | Guardrails lower that risk, but can never catch everything |
| 6:30 | Sander Schulhoff and HackAPrompt |
| 6:51 | Twelve published defenses, all bypassed |
| 7:04 | Why you can't patch a brain |
| 7:26 | Why have guardrails at all, like firewalls and antivirus |
| 7:36 | Defense in depth |
| 7:45 | The Swiss cheese model, and why the checks should differ |
| 8:01 | Slower, more expensive, less likely to work |
| 8:19 | It's also an alarm |
| 8:33 | The bar is reasonable care |
| 8:40 | Start before the first check, with a threat model |
| 8:52 | Stack several different checks |
| 9:02 | Why not keep adding checks |
| 9:12 | Every channel has its own clock |
| 9:28 | The checks' own clocks |
| 9:37 | Money, and mistakes |
| 9:51 | Every check is a trade-off, and the tripwire |
| 10:06 | Cheap checks on everything, expensive ones where it would hurt most |
| 10:16 | Fail open, or fail closed |
| 10:31 | Guardrails in a box from the big clouds |
| 10:48 | Limit what the system can do, at the bank's bollards |
| 11:07 | Keep revisiting |
| 11:14 | End card |

## Citations by timestamp

### 0:08 · A crash-tested rail

> Highway guardrails are crash tested.

**What this is getting at.** Highway guardrails are rated by crash test. In the US the standard is AASHTO's *Manual for Assessing Safety Hardware* (MASH, 2nd edition, 2016). At test level 3, the everyday highway rating, a rail is hit by a small car and by a 2,270-kilogram (5,000-pound) pickup, each at 62 miles an hour and 25 degrees. The film shows the pickup test, the one the narrator describes. AASHTO's own text is paywalled, so these numbers come from state transportation manuals that reproduce the test matrix.

**Sources**
- [Iowa DOT Design Manual §8A-7, "Introduction to MASH Crash Testing"](https://iowadot.gov/design-manual/chapter-8-roadside-safety/8a-7-introduction-mash-crash-testing) (revised Jun 2, 2026). [GOV]
- TxDOT, [Bridge Railing Manual, "Required Crash Tests"](https://www.txdot.gov/manuals/brg/rlg/chapter-2---policies-on-use-of-bridge-railing-for-/section-2---fhwa-policy-on-bridge-railing/required-crash-tests.html) and [Roadway Design Manual §17.2](https://www.txdot.gov/manuals/des/rdw/chapter-17-roadside-safety-design-and-roadside-saf/17-2-roadside-safety-hardware-crash-criteria.html). [GOV]

### 0:22 · Catch the truck, steer it back

> Built to catch the truck and steer it back.

**What this is getting at.** What a guardrail is for. MASH passes a barrier only if it contains and redirects the vehicle or brings it to a controlled stop, without the vehicle going through, under or over it. A rail is designed to turn a bad crash into a survivable one, which is the film's picture of an AI guardrail too.

**Sources**
- National Academies, [*Development of a MASH Barrier to Shield Pedestrians, Bicyclists, and Other Vulnerable Users from Motor Vehicles*](https://www.nationalacademies.org/read/27896/chapter/10) (2024), ch. 8, quoting MASH's structural criterion. [ACADEMIC]
- [Iowa DOT §8A-7](https://iowadot.gov/design-manual/chapter-8-roadside-safety/8a-7-introduction-mash-crash-testing). [GOV]

### 0:30 · Much heavier than tested

> Much heavier than tested, it can give way.

**What this is getting at.** A test level works like a threat model. A rail rated for a pickup at 62 miles an hour makes no promise about a loaded truck, which is why test levels 4 to 6 add a box truck, a tractor-trailer and a tanker. Iowa DOT notes that crash tests run under ideal conditions and that these devices aren't designed for every possible condition. The NTSB has made the same point in an accident report, finding a standard rail that wasn't designed to redirect a much heavier vehicle. The truck in the film is an illustration.

**Sources**
- [Iowa DOT §8A-7](https://iowadot.gov/design-manual/chapter-8-roadside-safety/8a-7-introduction-mash-crash-testing) and [TxDOT §17.2](https://www.txdot.gov/manuals/des/rdw/chapter-17-roadside-safety-design-and-roadside-saf/17-2-roadside-safety-hardware-crash-criteria.html), for test levels 4 to 6. [GOV]
- [NTSB Highway Accident Report HAR-12/01](https://www.ntsb.gov/investigations/AccidentReports/Reports/HAR1201.pdf) (adopted Jun 5, 2012). [GOV]

### 0:40 · AI has guardrails too

> AI has guardrails too.
>
> They work the same way, and they're just as easy to misunderstand.

The turn from the road to AI. That they're just as easy to misunderstand is the series' view.

### 1:28 · Software outside the model

> Software that sits outside the model.
>
> It checks what goes in, what comes out, and what the model is about to do.

**What this is getting at.** The definition the film uses. NIST's taxonomy of attacks on AI sorts protections by when they apply. Safety training happens inside the model, while classifier models that detect and stop harmful interactions run at deployment, and that deployment layer is what the film calls guardrails. The UK NCSC explains why the checks sit outside, since today's models "simply do not enforce a security boundary between instructions and data inside a prompt." With agents, the checks also look at actions before a tool runs, as the Five Eyes agencies' guidance on agents describes under guardrails and constraints.

**Sources**
- [NIST AI 100-2e2025, *Adversarial Machine Learning*](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf) (Mar 2025), pp. 47–48. [GOV]
- [UK NCSC: "Prompt injection is not SQL injection (it may be worse)"](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]
- Five Eyes agencies, ["Careful adoption of agentic AI services"](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 1, 2026), p. 20. [GOV]

### 1:39 · Orders hidden in what it reads

> Orders hidden in what the AI reads.
>
> An email or a webpage can carry instructions the user never wrote. That's prompt injection.

**What this is getting at.** An email, a web page or a document can carry instructions the user never wrote, and a model that reads them may follow them. OWASP ranks prompt injection first in its Top 10 for LLM applications. It says "it is unclear if there are fool-proof methods of prevention", and lists measures that limit the impact, with filtering inputs and outputs as one of seven. In the film, the input check looks for those hidden orders on the way in.

**Sources**
- [OWASP Top 10 for LLM Applications 2025, LLM01 Prompt Injection](https://genai.owasp.org/llmrisk/llm01-prompt-injection/). [STANDARD]

### 1:51 · What shouldn't leave

> On the way out, what shouldn't leave.
>
> Like a customer's card number.

**What this is getting at.** Checks on the way out. Amazon Bedrock's sensitive-information filter recognizes about 31 built-in kinds of personal data, card numbers among them, and can mask or block them in a response. It works by probability and context, so it can miss. Microsoft's Azure AI Content Safety screens responses for harmful content and protected material. The card in the film is an illustration.

**Sources**
- AWS, [Amazon Bedrock Guardrails sensitive-information filters](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-sensitive-filters.html). [SELF]
- Microsoft Learn, [Azure AI Content Safety overview](https://learn.microsoft.com/en-us/azure/ai-services/content-safety/overview) (updated Oct 2026). [SELF]

### 1:57 · Held for a person

> An action, held for a person.
>
> An agent is an AI that acts on its own. A check holds its refund until a person says yes.

**What this is getting at.** Checks on actions. OpenAI's Agents SDK lets a developer mark a tool as needing approval, so the run pauses, for hours if need be, until a person answers. Amazon's AgentCore Policy puts fixed rules, denying by default, at the gateway where an agent calls its tools. The refund is an illustration.

**Sources**
- OpenAI, [guardrails and approvals guide](https://developers.openai.com/api/docs/guides/agents/guardrails-approvals), and the [Agents SDK guardrails docs](https://openai.github.io/openai-agents-python/guardrails/) (v0.24.0, Oct 2026). [SELF]
- AWS, [Amazon Bedrock AgentCore Policy](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/policy.html). [SELF]

### 2:07 · Checks can steer

> Checks can steer, too.
>
> A sensitive question can go to a person, or get an approved script and links to self-serve help.

**What this is getting at.** A check doesn't only say yes or no. It can route a conversation. This pattern comes from practice. Some legal and compliance questions shouldn't get a free-form AI answer, so they go to a person or to an approved reply with links to self-serve help. The tools support it. A Bedrock guardrail returns a blocked message you write yourself when a denied topic comes up, and NVIDIA's NeMo Guardrails uses dialog rails to steer a conversation's flow.

**Sources**
- AWS, [Amazon Bedrock Guardrails denied topics](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-denied-topics.html), including "Messaging for blocked prompts". [SELF]
- NVIDIA, [NeMo Guardrails rail types](https://docs.nvidia.com/nemo/guardrails/latest/about-nemo-guardrails-library/rail-types), on dialog rails. [SELF]

### 2:21 · Three kinds of check

> The checks come in three kinds.

**What this is getting at.** The three kinds of checker, which the film ranks fastest to slowest. Rules match fixed text. Small classifier models are trained to spot one kind of problem. An AI judge is a second model asked to evaluate the first. LangChain's docs draw the same split, between deterministic checks, which are fast, cheap and predictable but miss nuance, and model-based checks, which catch subtler problems but are slower and cost more. The next three entries take the kinds one at a time, and the measured times are at 9:28.

**Sources**
- LangChain, [Guardrails docs](https://docs.langchain.com/oss/python/langchain/guardrails), on deterministic and model-based checks. [SELF]
- Meta, [Llama Prompt Guard 2 model card](https://huggingface.co/meta-llama/Llama-Prompt-Guard-2-86M) (Apr 29, 2025). [SELF]
- OpenAI, [Guardrails library](https://github.com/openai/openai-guardrails-python) (open source; a preview release). [SELF]

### 2:24 · The simplest is a rule

> The simplest is a rule.
>
> A list of banned words, or a regular expression, regex for short, that matches a card number.
>
> Instant, and free on Amazon's cloud.
>
> But a rule only matches what someone wrote down. Say it differently, and it slips right past.

**What this is getting at.** A rule is written in advance and matches fixed text. Amazon Bedrock Guardrails has word filters, a managed profanity list plus up to 10,000 custom words or phrases, and it takes your own regex patterns in its sensitive-information filter. AWS lists both as free. Rules work well where the bad thing has a fixed shape, such as a card number written the usual way, and they miss anything reworded. AWS's own example is that a custom filter for "competitor" doesn't match "competitors". The UK NCSC says of blocking known attack phrases that "there are infinite ways to rephrase an attack that would avoid such a filter." No vendor publishes a time for these checks, so "instant" is the film's word for very fast. The card number in the film is an illustration.

**Sources**
- AWS, [Bedrock Guardrails word filters](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-word-filters.html), [sensitive-information filters](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-sensitive-filters.html) and [Bedrock pricing](https://aws.amazon.com/bedrock/pricing/) (Oct 2026). [SELF]
- [UK NCSC: "Prompt injection is not SQL injection (it may be worse)"](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]

### 2:47 · Small models, each with one job

> Small models, each with one job.
>
> They're fast, and they judge what the words mean, so they catch rewordings a rule would miss.

**What this is getting at.** A small classifier is a model trained for one narrow task. Meta's Prompt Guard 2, for example, labels text as benign or malicious, looking for jailbreaks and prompt injection, and it answers in tens of milliseconds (9:28). Because a classifier works from meaning rather than exact text, it can catch rewordings that a rule misses. It can still be fooled. OWASP's 2026 list warns that semantic filters "are evadable by rephrasing or encoding", and adaptive attacks got past Prompt Guard 94% of the time in the study at 6:51.

**Sources**
- Meta, [Llama Prompt Guard 2 model card](https://huggingface.co/meta-llama/Llama-Prompt-Guard-2-86M) (Apr 29, 2025). [SELF]
- OWASP, [Top 10 for LLM Applications 2026](https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/) (Aug 3, 2026), LLM01:2026 Prompt Injection. [STANDARD]

### 3:01 · A second AI as a judge

> A second AI, acting as a judge.
>
> You describe your rules in plain language. It reads each request or answer and decides.

**What this is getting at.** The slowest kind. An AI judge is a second model, given rules written in plain language, that reads each request or answer and decides whether it breaks them. OpenAI's guide to building agents describes guardrails built as agents that enforce policies such as jailbreak prevention and relevance, layered with rules such as regex. OpenAI's open-source Guardrails library uses a model as the judge in checks such as its jailbreak and prompt-injection detectors, and in OpenAI's tests those took about 1.5 seconds each (9:28). The rules and the refund in the film are illustrations.

**Sources**
- OpenAI, ["A practical guide to building agents"](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) (Apr 2025), pp. 25 and 31. [SELF]
- OpenAI, [Guardrails library check docs](https://github.com/openai/openai-guardrails-python/tree/main/docs/ref/checks) (Dec 15, 2025). [SELF]

### 3:12 · For laughs, at first

> Why would anyone attack an AI?
>
> For a while, mostly for laughs.
>
> A car dealer's chatbot once agreed to sell an SUV for $1.

**What this is getting at.** Early attacks on chatbots were mostly pranks. In December 2023, a Chevrolet dealer's website chatbot, built on ChatGPT, agreed to sell a 2024 Tahoe for one dollar after a user talked it into it. The deal wasn't binding, and the chatbot's vendor pulled it from the dealer's site. Its CEO said the logs showed people trying for hours and the bot mostly resisting. The dealer's lot in the film is an illustration.

**Sources**
- [Business Insider, Katie Notopoulos](https://www.businessinsider.com/car-dealership-chevrolet-chatbot-chatgpt-pranks-chevy-2023-12) (Dec 18, 2023). [PRESS]

### 3:24 · It doesn't feel like breaking in

> Most mean no harm. It doesn't feel like breaking in.
>
> In experiments, people cheated about 3× more reporting to a machine than to a person.

**What this is getting at.** Why ordinary people try it. In a representative survey of 3,270 UK adults, about a quarter of regular chatbot users had tried to get past a refusal, for fun, out of curiosity or to get an answer, about equally often. Hobbyist red-teamers interviewed for a PLOS One study described it as play and said they meant no harm. And in two experiments with 848 people, participants cheated about three times more when they reported to a machine than to a person, whether or not the machine seemed human. "Most mean no harm" is a hedged summary of these studies.

**Sources**
- Cohn, Gesche and Maréchal, ["Honesty in the Digital Age"](https://doi.org/10.1287/mnsc.2021.3985), *Management Science* 68(2) (2022). [ACADEMIC]
- Grosse and Ebert, [arXiv 2510.27275](https://arxiv.org/abs/2510.27275) (Oct 31, 2025; revised Jul 30, 2026). A preprint.
- Inie, Stray and Derczynski, ["Summon a demon and bind it"](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0314658), *PLOS One* (Jan 15, 2025). [ACADEMIC]

### 3:40 · Words can take that power

> Words can take that power and turn it against you.

**What this is getting at.** The stakes changed when AIs got tools. The narrator's examples are an AI that can read your email, open your files and spend your money. Simon Willison's "lethal trifecta" is an agent with access to private data, exposure to untrusted content and a way to send data out. With all three, anyone who can get words in front of it can trick it into sending your data to them. The UK NCSC and OWASP make the same point in their own terms, that the damage depends on what the system is able to do. Spending money is the film's extension of Willison's list.

**Sources**
- Simon Willison, ["The lethal trifecta for AI agents"](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/) (Jun 16, 2025). An independent developer's blog.
- [UK NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]
- [OWASP LLM01:2025](https://genai.owasp.org/llmrisk/llm01-prompt-injection/). [STANDARD]

### 3:51 · Hidden instructions already turn up

> Hidden instructions already turn up.
>
> In résumés, in research papers aimed at AI reviewers, in links that ask assistants to recommend a company.

**What this is getting at.** Hidden text already turns up wherever an AI makes or shapes a decision. In about 200,000 real résumés, about 1% carried hidden text aimed at AI screeners, though more than 90% of those were keywords and claims rather than commands, and the authors don't assume every applicant meant it. Nikkei Asia found hidden prompts asking AI reviewers for positive reviews in 17 arXiv preprints from 14 institutions in 8 countries. Microsoft found 31 real companies, across 14 industries, hiding instructions in "summarize with AI" links that told assistants to remember or recommend them.

**Sources**
- Zhang et al. (Duke, hireEZ and others), [arXiv 2605.28999](https://arxiv.org/abs/2605.28999) (May 27, 2026; USENIX Security 2026), and [Duke Pratt news](https://pratt.duke.edu/news/thwarting-prompt-injection/) (Jul 22, 2026). A preprint.
- [Nikkei Asia](https://asia.nikkei.com/business/technology/artificial-intelligence/positive-review-only-researchers-hide-ai-prompts-in-papers) (Jun 30, 2025). [PRESS]
- Microsoft Defender Security Research, ["Manipulating AI memory for profit: The rise of AI Recommendation Poisoning"](https://www.microsoft.com/en-us/security/blog/2026/02/10/ai-recommendation-poisoning/) (Feb 10, 2026). [VENDOR]

### 4:02 · Known flaws, growing fast

> Prompt injection flaws are growing fast.
>
> In America's vulnerability database, 2 in 2023 and 98 this year.

**What this is getting at.** A count made for this film. In NIST's National Vulnerability Database, the US record of disclosed software flaws, CVE records whose description contains the exact phrase "prompt injection" went from 2 in 2023 to 18 in 2024, 34 in 2025 and 98 in 2026 through Oct 23. The film labels only the first and the last. The first, CVE-2023-29374, is a LangChain flaw published in April 2023. NVD published far more records of every kind in 2026, so a fairer trend is the share, and that rose every year too, from 0.7 to 11.4 per 10,000 records. Two caveats. The count is a floor, because many flaws never get a CVE and some are described in other words, as Microsoft's EchoLeak flaw is, filed in the [NVD](https://nvd.nist.gov/vuln/detail/CVE-2025-32711) as "AI command injection". And a CVE records a disclosed flaw, which says nothing about whether anyone attacked it.

**Sources**
- NIST, [National Vulnerability Database API, exact-phrase search](https://services.nvd.nist.gov/rest/json/cves/2.0?keywordSearch=prompt%20injection&keywordExactMatch), our count by publication date on Oct 23, 2026. The all-time total that day was 152. [DATA]

### 4:16 · Every new connection

> Every new connection is a new place for a hidden instruction to land.

**What this is getting at.** Why the count keeps rising. Stanford's 2026 AI Index reports that organizational adoption of AI reached 88%. Agents now open files, send messages and run tools, often through the Model Context Protocol (MCP), which connects AI tools to outside servers. The official MCP Registry listed 49,041 servers on Oct 23, 2026, up from 1,204 at the end of 2025, by our count. Those are registrations, which don't show how much each server is used. The Five Eyes agencies' guidance on agents says every component of an agentic system "widens the attack surface", and 23 of 2026's 98 prompt-injection CVEs so far mention MCP.

**Sources**
- Stanford HAI, [2026 AI Index](https://hai.stanford.edu/ai-index/2026-ai-index-report) (Apr 2026). [ACADEMIC]
- [MCP Registry API](https://registry.modelcontextprotocol.io/v0/servers), our full count on Oct 23, 2026. [DATA]
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), p. 6. [GOV]

### 4:25 · Attackers adapt

> Attackers adapt.
>
> They want to trick an AI into working for them, or to break it free of its own rules.

A bridge to the people, and the research, that show it. The two goals are the film's way into the two attack types defined next.

### 4:35 · Three terms

> The first, prompt injection, we've already seen.
>
> Talking it out of its rules is jailbreaking.
>
> Attacking on purpose, to find the holes first, is red teaming.

**What this is getting at.** The terms, one at a time. NIST defines prompt injection as an attack that exploits the joining of untrusted input to a prompt written by a more trusted party, such as the app's designer. Simon Willison, who coined the term in 2022, uses the same test. In NIST's glossary a jailbreak is a direct prompting attack "intended to circumvent restrictions placed on model outputs", such as getting past a model's refusals, and red teaming is "a structured testing effort, often adopting adversarial methods, to find flaws and vulnerabilities". The sources disagree on one point. OWASP treats jailbreaking as a kind of prompt injection, while NIST and Willison keep the two apart, and the film follows NIST and Willison.

**Sources**
- [NIST AI 100-2e2025, *Adversarial Machine Learning*](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf) (Mar 2025), glossary, PDF pp. 123–125. [GOV]
- Simon Willison, ["Prompt injection and jailbreaking are not the same thing"](https://simonwillison.net/2024/Mar/5/prompt-injection-jailbreaking/) (Mar 5, 2024). An independent developer's blog.
- [OWASP LLM01:2025](https://genai.owasp.org/llmrisk/llm01-prompt-injection/). [STANDARD]

### 4:50 · Pliny the Liberator

> Pliny the Liberator
>
> An anonymous red teamer who has jailbroken nearly every major AI model since 2023, often on launch day.

**What this is getting at.** The best-known red teamer. Since 2023, this anonymous red teamer has broken nearly every major AI model, talking each one out of its own safety rules, and published the methods in the open for anyone to study. In a check of 23 major releases from 2024 to early 2026 made for this film, a Pliny jailbreak was public on launch day for 19 of them. Pliny also publishes the hidden system prompts AI products run on, and co-designed a HackAPrompt track in 2025 whose data was then released openly. For defenders, that public record is one of the clearest real-world tests of guardrails. Pliny has argued that content filters are largely futile and that real security belongs in the system around the model, and the film's close lands in the same place on the second point. On screen are Pliny's X profile, including the "{LOVE PLINY}" tucked into the display name in invisible characters, and a post from the launch night of OpenAI's gpt-oss models in August 2025, shown with its harmful line blurred.

**Sources**
- Pliny on X, [@elder_plinius](https://x.com/elder_plinius), and the [gpt-oss launch-night post](https://x.com/elder_plinius/status/1952958577867669892) (late Aug 5, 2025, US time). [SELF]
- Pliny on GitHub, [elder-plinius](https://github.com/elder-plinius). [SELF]
- [VentureBeat, Carl Franzen](https://venturebeat.com/ai/an-interview-with-the-most-prolific-jailbreaker-of-chatgpt-and-other-leading-llms) (May 31, 2024). [PRESS]
- [Decrypt, Jose Antonio Lanz](https://decrypt.co/333858/openai-jailbreak-proof-new-models-hacked), on the gpt-oss jailbreak (Aug 6, 2025). [PRESS]
- [Latent Space podcast](https://www.latent.space/p/jailbreaking-agi-pliny-the-liberator) with Pliny (Dec 16, 2025). [PRESS]
- [The Pliny HackAPrompt Dataset](https://huggingface.co/datasets/hackaprompt/Pliny_HackAPrompt_Dataset) (Jul 4, 2025).

### 5:07 · TIME100 AI

> One of TIME's 100 most influential people in AI, 2025.

**What this is getting at.** Recognition well beyond the field. TIME's 2025 profile describes Pliny as an anonymous figure finding the holes in billion-dollar AI systems. SANS later announced Pliny as a keynote speaker for its AI Cybersecurity Summit in April 2026, and its summary of the summit lists the talk on the second day, Apr 21.

**Sources**
- [TIME, Tharin Pillay, TIME100 AI 2025](https://time.com/collections/time100-ai-2025/7305870/pliny-the-liberator/) (Aug 27, 2025). [PRESS]
- [SANS, Rob T. Lee](https://www.sans.org/blog/keynote-pliny-the-liberator-sans-ai-cybersecurity-summit) (Feb 25, 2026), and SANS's [summit summary](https://www.sans.org/blog/visual-summary-sans-ai-cybersecurity-summit-2026) (Apr 20, 2026). [PRESS]

### 5:14 · A robot dog at Black Hat

> At Black Hat, a robot dog, hijacked.
>
> Pliny's team, BT6, took it over through its own camera and microphone.

**What this is getting at.** At Black Hat USA in Las Vegas this August, six people from BT6, a white-hat red-team collective, gave a Briefings talk called "Kinetic Prompt Injection: Agent Compromise With a Physical Blast Radius", and Pliny is among the listed speakers. Black Hat's summary describes a live jailbreak of a stock Unitree Go2 robot dog running Google's Gemini Robotics-ER 1.6 model, reached through the robot's own camera and microphone and driven to move with no human in the loop. Black Hat posted the recording on Aug 7. The talk's date, Aug 6, comes from a third-party schedule write-up, because Black Hat's own schedule pages refuse automated checks. It was a single talk by one team, and no source says whether Pliny was there in person or remotely.

The footage in the film is from that recording (8:41 to 8:55): the robot dog trots in and stands by the stage's floor camera. It is cropped so no presenter's face is in frame, and none of the talk's slides or prompts appear.

**Sources**
- Black Hat, ["Black Hat USA 2026 | Kinetic Prompt Injection: Agent Compromise With a Physical Blast Radius"](https://www.youtube.com/watch?v=LZkdihOzfe4), the talk's recording, with its speaker list and summary (posted Aug 7, 2026). [SELF]
- Alicia Dahling, [schedule write-up](https://unapologeticallydahling.com/blog/black-hat-2026-the-most-terrifying-morning-in-vegas) (Jul 30, 2026), for the date. A blog.

### 5:29 · AI is starting to move things

> AI is starting to move things.
>
> Microduck, from Pollen Robotics. $399. More than 10,000 sold in its first five days.

**What this is getting at.** An example of AI that moves things, at a consumer price. Microduck is a robot duck about 25 centimetres (ten inches) tall from Pollen Robotics, a French robot maker that Hugging Face bought in 2025. It opened for pre-orders on Aug 27, 2026, at an introductory $399 before tax and shipping, and Hugging Face told CNBC it had sold more than 10,000 in about five days. Owners train its moves themselves with reinforcement learning. Its software is open source under Apache 2.0, and Pollen asks that it not be called open-source hardware, because its design files aren't open. Microduck is the film's one example of robots getting cheap and popular, and this film's research found no attack on it. The Microduck in the film is an illustration built in code.

**Sources**
- Pollen Robotics, [Microduck](https://pollen-robotics.com/microduck/), its [launch post](https://pollen-robotics.com/microduck/blog/introducing-microduck/) (Aug 27, 2026) and [press kit](https://pollen-robotics.com/microduck/press-kit/). [SELF]
- [CNBC, Evelyn Cheng](https://www.cnbc.com/2026/09/01/hugging-faces-new-duck-robot-is-selling-fast-a-chinese-chip-powers-it.html) (Sep 1, 2026), citing Hugging Face. [PRESS]
- Hugging Face, ["Hugging Face to sell open-source robots thanks to Pollen Robotics acquisition"](https://huggingface.co/blog/hugging-face-pollen-robotics-acquisition) (Apr 14, 2025). [SELF]

### 5:46 · More than saying something wrong

> A bad instruction can do more than say something wrong.
>
> Researchers have already talked AI-driven robots into unsafe actions.

**What this is getting at.** When a language model steers a robot, a planted instruction can turn into movement. In 2024, Penn researchers' RoboPAIR jailbroke three systems run by language models, among them a Unitree Go2 robot dog, with attack success rates that often reached 100% in their own tests, and they shared the findings with AI companies and the robot makers before release. BadRobot (ICLR 2025) got embodied AI agents to break safety and ethical rules through ordinary voice interaction. A 2026 preprint found that text on a sheet of paper in a robot's camera view could work as a prompt injection on its planner, and that simple defenses worked well in that setup. America's cyber agency, CISA, and its partners warn that AI such as language models "almost certainly should not be used to make safety decisions for OT environments", meaning operational technology, the systems that run physical processes. Pliny's team showed another case on stage at Black Hat (5:14). The robot arm in the film is an illustration.

**Sources**
- Robey et al., ["Jailbreaking LLM-Controlled Robots"](https://arxiv.org/abs/2410.13691) (RoboPAIR, Oct 2024). A preprint; its authors list it at ICRA 2025.
- Zhang et al., ["BadRobot"](https://arxiv.org/abs/2407.20242) (ICLR 2025). [ACADEMIC]
- Samarakoon et al., ["Hijacking Robots with a Piece of Paper"](https://arxiv.org/abs/2608.05715) (Aug 6, 2026). A preprint.
- CISA, ASD's ACSC and partners, ["Principles for the Secure Integration of Artificial Intelligence in Operational Technology"](https://www.cisa.gov/sites/default/files/2026-01/joint-guidance-principles-for-the-secure-integration-of-artificial-intelligence-in-operational-technology-508cV2.pdf) (Dec 3, 2025), p. 9. [GOV]

### 6:00 · A software risk today, a physical one soon

> Today, a software risk. Soon, a physical one.

**What this is getting at.** The film's own judgment, drawn from the two sections before it. So far, prompt injection mostly does its harm in software: data leaked, messages sent, tools run that nobody asked for. Robots that run on AI models are getting cheap enough to sell by the thousand (5:29), and researchers have already talked them into unsafe actions (5:46). As more of them ship, the same hidden instruction can move something in the physical world.

### 6:12 · Guardrails lower that risk, but can never catch everything

> Guardrails lower that risk.
>
> It can never catch everything.
>
> More possible prompts than atoms in the universe, and always another way to say the same thing.

**What this is getting at.** The size of the problem. Sander Schulhoff (6:30) estimates that a GPT-5-class model has about 10^1,000,000 possible prompts, against about 10^80 atoms in the universe. A check for this film found the estimate holds, and if anything it's conservative. Almost all of those prompts are gibberish, but the meaningful ones are still far too many to ever test, and attackers search them on purpose. For every prompt a check learns to stop, there's another way to say the same thing (2:24). Schulhoff goes further than the film. His essay argues guardrails don't protect you and can make teams overconfident. The film agrees they aren't a wall and disagrees about their value (7:26).

**Sources**
- Sander Schulhoff, ["The AI Security Industry is Bullshit"](https://sanderschulhoff.substack.com/p/the-ai-security-industry-is-bullshit) (Dec 20, 2025). An essay.

### 6:30 · Sander Schulhoff

> Sander Schulhoff
>
> Runs HackAPrompt and Learn Prompting. His 2023 contest drew about 2,800 people and 600,000+ attacks.

**What this is getting at.** Who he is. Learn Prompting's site lists Schulhoff as its founder and CEO, and as CEO of HackAPrompt, which runs prompt-hacking contests. The 2023 contest's paper reports more than 2,800 participants from more than 50 countries, who wrote more than 600,000 attack prompts against three models. It appeared at EMNLP 2023 and won one of its best paper awards. HackAPrompt is one of the biggest contests of its kind. Several events call themselves the largest on different measures, so the film gives the 2023 figures instead. His photo is shown with an on-screen credit.

**Sources**
- Schulhoff et al., ["Ignore This Title and HackAPrompt"](https://arxiv.org/abs/2311.16119) (EMNLP 2023), among the [EMNLP 2023 best papers](https://2023.emnlp.org/program/best_papers/). [ACADEMIC]
- Learn Prompting, [About](https://learnprompting.org/about). [SELF]

### 6:51 · Twelve of twelve

> 12 of 12 defenses bypassed.
>
> Attacks that adapt got past all twelve, most more than 9 times in 10.

**What this is getting at.** Adaptive attacks. In "The Attacker Moves Second", Schulhoff and researchers from OpenAI, Anthropic, Google DeepMind, ETH Zürich and others tested 12 published defenses against jailbreaks and prompt injection. Attacks that learn and change tactics got past all 12, most of them more than 90% of the time, though most of the defenses had originally reported near-zero attack success. Four were filter models of the kind the film calls guardrails, including Google's own Model Armor. The test was demanding, since the attacker could see each detector's scores. The narrator then quotes Schulhoff's line, "You can patch a bug, but you can't patch a brain."

**Sources**
- Nasr, Carlini, Sitawarin, Schulhoff, Tramèr et al., ["The Attacker Moves Second"](https://arxiv.org/abs/2510.09023) (Oct 10, 2025). A preprint.
- [Schulhoff's essay](https://sanderschulhoff.substack.com/p/the-ai-security-industry-is-bullshit) (Dec 20, 2025), for the quote.

### 7:04 · You can't patch a brain

> A bug is a mistake in a line of code.
>
> You find it, fix it, and that hole is closed.
>
> A model has no line to fix.
>
> A fix makes the same attack less likely, but it can't prove the hole is gone.

**What this is getting at.** Schulhoff's line, in plain words. His essay puts it as odds. Fix a bug in code and you can be 99.99% sure it's fixed, but try to fix a flaw in an AI model and you can be 99.99% sure it isn't. The film's plain-words version follows. A software bug sits in a specific line that can be changed and tested. A model's behavior comes from training, so fixing the model itself means more training. That makes the same attack less likely to work, but it can't prove the hole is gone. His essay's advice is classic security around the model, such as sandboxing and tight data permissions, and the film's close lands nearby (10:48). The code in the film is an illustration.

**Sources**
- [Schulhoff's essay](https://sanderschulhoff.substack.com/p/the-ai-security-industry-is-bullshit) (Dec 20, 2025), "Final takeaways". An essay.

### 7:26 · Why have guardrails at all

> Why have guardrails at all?
>
> For the same reason we still run firewalls and antivirus.

**What this is getting at.** The turn, and the series' view. None of this makes guardrails pointless. NIST's malware guide calls antivirus "a necessity", and also says "it is not possible for antivirus software to stop all malware incidents." Teams run it anyway. A classifier guardrail is closest to antivirus, since both work by probability. Permissions and allowlists are the firewall-like part of the stack.

**Sources**
- [NIST SP 800-83 Rev. 1, *Guide to Malware Incident Prevention and Handling*](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-83r1.pdf) (Jul 2013), pp. 22 and 28. [GOV]

### 7:36 · Defense in depth

> Defense in depth.
>
> Different kinds of checks, so what one misses, another catches.

**What this is getting at.** Why teams run imperfect checks together. One of NIST's glossary definitions, from the standard ISA/IEC 62443, describes "layering heterogeneous security technologies in the common attack vectors to ensure that attacks missed by one technology are caught by another." Heterogeneous means different kinds. The Five Eyes agencies' guidance on agents says to "avoid reliance on a single security mechanism", and to layer guardrails "ranging from anomaly detection and rule-based filtering to specialised machine learning algorithms". In the film the layers are a rule, a classifier, an AI judge, a person and the logs.

**Sources**
- [NIST glossary, "defense-in-depth"](https://csrc.nist.gov/glossary/term/defense_in_depth), citing NISTIR 8183. [GOV]
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), pp. 15 and 20. [GOV]

### 7:45 · The Swiss cheese model

> The same idea, as Swiss cheese.
>
> Every slice has holes. Harm usually gets through only when the holes line up.
>
> So the checks should be different.
>
> If they all miss the same things, the holes always line up.

**What this is getting at.** Defense in depth, drawn as a picture. The psychologist James Reason drew safety defenses as stacked slices, each with holes that open, close and move, so harm usually needs the holes in many layers to line up at the same moment. The International AI Safety Report uses the same picture for AI safeguards. For AI there's a catch. Layers only help if they fail in different ways. Dung and Mai note that if every safety technique failed the same way, defense in depth "would provide no additional protection at all". That's why the film says the checks should be different, mixing kinds such as rules, models and people instead of stacking more AI judges. Researchers have also beaten a layered pipeline one layer at a time. In the film the slices carry the names of the checks at 7:45.

**Sources**
- James Reason, ["Human error: models and management"](https://pmc.ncbi.nlm.nih.gov/articles/PMC1117770/), *BMJ* 320:768 (Mar 18, 2000). [ACADEMIC]
- [International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026) (Feb 3, 2026), Figure 3.5. [GOV]
- Dung and Mai, [arXiv 2510.11235](https://arxiv.org/abs/2510.11235) (Oct 13, 2025). A preprint.
- McKenzie et al., ["STACK"](https://arxiv.org/abs/2506.24068) (v3 Feb 5, 2026). A preprint.

### 8:01 · Slower, more expensive, less likely to work

> Slower, more expensive, less likely to work.
>
> 339 people tried. 4 got all the way through, after about 3,700 hours.

**What this is getting at.** In February 2025, Anthropic opened a model guarded by its constitutional classifiers to a public challenge with eight levels. 339 people took part, over more than 300,000 chats and about 3,700 hours of combined effort. The system held for five of the seven days, and four people cleared all eight levels by the end. In Anthropic's automated test of 10,000 synthetic jailbreak prompts, the share that worked fell from 86% without the classifiers to 4.4% with them. Anthropic notes the challenge made attacking easier than real life, with instant automatic grading and none of the account monitoring it would use in a real deployment. Separately, the UK AI Security Institute has found universal jailbreaks in every system it tested, and found that one newer model took about forty times more expert effort to crack than one released six months earlier. Both fit the film's claim that guardrails make attacks slower, more expensive and less likely to work.

**Sources**
- Anthropic, ["Constitutional Classifiers"](https://www.anthropic.com/research/constitutional-classifiers) (Feb 3, 2025; updated through Feb 18, 2025). [SELF]
- [The Decoder, Maximilian Schreiner](https://the-decoder.com/claude-jailbreak-results-are-in-and-the-hackers-won/) (Feb 4, 2025; updated Feb 11 and 15). [PRESS]
- [UK AI Security Institute, "5 key findings from our first Frontier AI Trends Report"](https://www.aisi.gov.uk/blog/5-key-findings-from-our-first-frontier-ai-trends-report) (Dec 2025). [GOV]

### 8:19 · It's also an alarm

> It's also an alarm.
>
> Monitoring caught a state-backed campaign running through Anthropic's coding tool.

**What this is getting at.** A guardrail is also a sensor, since every blocked attempt leaves a record. In September 2025, Anthropic detected a campaign it attributes, with high confidence, to a Chinese state-sponsored group that had jailbroken Claude Code and aimed it at about 30 organizations, succeeding against a small number. Over about ten days, Anthropic banned the accounts, notified the affected organizations and worked with authorities. It's Anthropic's own account, and it doesn't say whether detection began with a classifier flag or with wider monitoring, which is why the caption says "monitoring". NIST's generative AI profile lists the number of unauthorized access attempts among the security metrics worth tracking.

**Sources**
- Anthropic, ["Disrupting an AI-orchestrated cyber espionage campaign"](https://www.anthropic.com/news/disrupting-AI-espionage) (Nov 13, 2025). [SELF]
- [NIST AI 600-1, Generative AI Profile](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf) (Jul 2024), MS-2.7-004. [GOV]

### 8:33 · Reasonable care

> It shows you took reasonable care.
>
> That is the standard regulators hold companies to.

**What this is getting at.** Regulators don't ask for perfect. Marking its 50th data security settlement in 2014, the FTC said reasonableness is the touchstone of its approach, that it "does not require perfect security", and that a breach alone doesn't mean a company broke the law. That statement covers data security in general rather than AI. The EU AI Act asks high-risk systems for "an appropriate level of accuracy, robustness, and cybersecurity", including measures to prevent, detect and respond to attacks. NIST's AI Risk Management Framework notes that "not all incidents and failures can be eliminated."

**Sources**
- [FTC, "Commission Statement Marking the FTC's 50th Data Security Settlement"](https://www.ftc.gov/system/files/documents/cases/140131gmrstatement.pdf) (Jan 31, 2014). [GOV]
- [EU AI Act, Article 15](https://artificialintelligenceact.eu/article/15/). [LAW]
- [NIST AI 100-1, AI RMF 1.0](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) (Jan 2023), §1.2.3. [GOV]

### 8:40 · Start before the first check

> Start before the first check.
>
> What your AI can reach, who can send it words, and what would really hurt.

**What this is getting at.** Before the first check, write down what the AI can touch, who or what can put words in front of it, and what it must never do. The Five Eyes agencies' guidance on agents has a section on threat modelling and recommends up-to-date risk taxonomies such as OWASP's and MITRE ATLAS. Microsoft's checklist starts with what actions the system should never take. OWASP's guide for agents frames threat modelling as four questions, starting with what you're working on. The film comes back to this list at 10:06.

**Sources**
- Five Eyes agencies (ASD's ACSC, CISA, NSA, the Canadian Centre for Cyber Security, NCSC-NZ and NCSC-UK), ["Careful adoption of agentic AI services"](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 1, 2026), p. 19, also on [CISA's site](https://www.cisa.gov/resources-tools/resources/careful-adoption-agentic-ai-services). [GOV]
- [Microsoft Security Blog, "Threat modeling AI applications"](https://www.microsoft.com/en-us/security/blog/2026/02/26/threat-modeling-ai-applications/) (Feb 26, 2026). [VENDOR]
- [OWASP, "Agentic AI – Threats and Mitigations"](https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/) v1.1 (Dec 2025), p. 12. [STANDARD]

### 8:52 · Stack several different checks

> Stack several different checks.
>
> On what comes in, on the tools it can use, on what goes out, and on the logs.

**What this is getting at.** Defense in depth (7:36), placed on a real system. The Five Eyes guidance says to apply security controls "at all points where information enters or exits the system, including user inputs, tool calls, data pre-processing and model inference", and to prioritise review of incidents where guardrails are triggered. OpenAI's guide to building agents layers rules, model checks and a moderation check on what comes in, and rates each tool's risk to decide where extra checks or a person go. MITRE ATLAS's mitigation for guardrails says their decisions should be logged.

**Sources**
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), pp. 15 and 20. [GOV]
- OpenAI, ["A practical guide to building agents"](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) (Apr 2025), pp. 25–26. [SELF]
- [MITRE ATLAS](https://atlas.mitre.org/), mitigation AML.M0020, "Generative AI Guardrails" ([data, v2026.09](https://github.com/mitre-atlas/atlas-data)). [STANDARD]

### 9:02 · Why not keep adding checks

> So why not keep adding checks?
>
> Every check has a cost. It takes time, costs money and makes mistakes.

**What this is getting at.** The catch with stacking. Every check adds delay, adds to the bill, and blocks some good requests or misses some bad ones. Microsoft's guidance on threat modeling AI lists "Performance and latency impacts from additional controls" among the trade-offs, and a 2025 preprint by researchers at Enkrypt AI, an AI security company, is titled "No Free Lunch with Guardrails". The next three entries take time, money and mistakes in turn. The price tags in the film are illustrations.

**Sources**
- Microsoft Learn, ["Complete AI threat modeling"](https://learn.microsoft.com/en-us/security/zero-trust/sfi/threat-modeling-ai) (updated Mar 26, 2026). [SELF]
- Kumar et al. (Enkrypt AI), ["No Free Lunch with Guardrails"](https://arxiv.org/abs/2504.00441) (Apr 2025). A preprint. [VENDOR]

### 9:12 · Every channel has its own clock

> Start with time. Each channel has its own clock.
>
> On a call, about a fifth of a second. An email can wait minutes.

**What this is getting at.** Time, the first cost. One assistant may answer email, web chat, text messages and phone calls, and each sets a different time budget for its checks. In a study across ten languages, people answered yes-or-no questions after a mean of 208 milliseconds. Email security already spends minutes, and Microsoft says its attachment sandbox typically finishes within 15 minutes. So a call only has room for tiny checks before speaking, while email has room for slow, deep ones. MITRE ATLAS added a technique in September 2026 for attackers probing an agent's email addresses, webhooks and messaging channels.

**Sources**
- Stivers et al., ["Universals and cultural variation in turn-taking in conversation"](https://pmc.ncbi.nlm.nih.gov/articles/PMC2705608/), *PNAS* 106(26) (2009). [ACADEMIC]
- Microsoft Learn, [Safe Attachments](https://learn.microsoft.com/en-us/defender-office-365/safe-attachments-about) (Jul 17, 2026). [SELF]
- [MITRE ATLAS](https://atlas.mitre.org/), technique AML.T0006.003 ([data, v2026.09](https://github.com/mitre-atlas/atlas-data)). [STANDARD]

### 9:28 · The checks' own clocks

> The checks have clocks of their own.
>
> A small classifier, about 20 ms. An AI judge, about 1.5 s.

**What this is getting at.** In OpenAI's published tests, its AI-judge checks for jailbreaks and prompt injection took a median of about 1.5 seconds each with its default judge model. Meta lists 19.3 milliseconds for its small Prompt Guard 2 classifier on one A100 GPU. The setups differ, so read it as an order of magnitude. Set against the channels, a judge that slow fits inside an email's wait but not a call's fifth of a second.

**Sources**
- OpenAI, [Guardrails library check benchmarks](https://github.com/openai/openai-guardrails-python/tree/main/docs/ref/checks) (Dec 15, 2025). [SELF]
- Meta, [Llama Prompt Guard 2 model card](https://huggingface.co/meta-llama/Llama-Prompt-Guard-2-86M) (Apr 29, 2025) and the [LlamaFirewall paper](https://arxiv.org/abs/2505.03574) (May 2025). [SELF]

### 9:37 · Money, and mistakes

> Then money. One filter, about 15¢ per 1,000 short messages.
>
> And mistakes. Every filter blocks some good requests and lets some bad ones through.

**What this is getting at.** Money first. Amazon Bedrock Guardrails lists its content filter at $0.15 per 1,000 text units, and a text unit holds up to 1,000 characters, so one short message through that one filter costs about $0.00015, or 15 cents per 1,000 messages. That's our math from the list price. Longer messages and frequent checks multiply it. Then mistakes. On Meta's in-house English test, its Llama Guard 4 model caught 69% of unsafe outputs and wrongly flagged 11% of safe ones. NVIDIA's length-per-perplexity heuristic, one of the jailbreak checks in NeMo Guardrails, caught 31.19% of jailbreaks in NVIDIA's own data, with 7.44% false positives. Each vendor graded its own tool on its own test set, and NVIDIA's docs note that moving the threshold trades one kind of mistake for the other. The coins in the film are illustrations. The voice prices only the filter, and the AI judge's taller stack isn't a measured figure.

**Sources**
- AWS, [Amazon Bedrock pricing](https://aws.amazon.com/bedrock/pricing/) (Oct 2026). [SELF]
- Meta, [Llama Guard 4 model card](https://github.com/meta-llama/PurpleLlama/blob/main/Llama-Guard4/12B/MODEL_CARD.md). [SELF]
- NVIDIA, [NeMo Guardrails jailbreak protection](https://docs.nvidia.com/nemo/guardrails/latest/configure-guardrails/guardrail-catalog/jailbreak-protection.md). [SELF]

### 9:51 · Every check is a trade-off

> Every check is a trade-off.
>
> Teams handle it in two common ways.
>
> Run alongside, with a tripwire.
>
> That's faster, but if it fires late, the agent may already have acted.

**What this is getting at.** The first common way. OpenAI's Agents SDK runs input checks alongside the agent by default, which its docs call the best latency, and stops the run when a check's tripwire fires. The same docs warn that by then the agent may already have spent tokens and run tools. In blocking mode the check finishes first, which avoids that at the cost of the wait. Amazon's AgentCore Policy has the same timing on the way out, where a check on a tool's result runs after the tool has run, so it can withhold the result but can't undo the action. The film's two ways are two of several patterns the docs describe, alongside checks on streamed text and monitoring after the fact.

**Sources**
- OpenAI, [Agents SDK guardrails docs](https://openai.github.io/openai-agents-python/guardrails/) (v0.24.0, Oct 2026), and its [guardrails and approvals guide](https://developers.openai.com/api/docs/guides/agents/guardrails-approvals). [SELF]
- AWS, [AgentCore Policy, "Guardrails in policies"](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/policy-guardrails-in-policies.html). [SELF]

### 10:06 · Cheap checks on everything

> Or run cheap checks on everything.
>
> Save the slow, expensive ones for where it would hurt most, the list from the start.

**What this is getting at.** The second common way. Cheap checks on everything, expensive ones where the risk is, and "the list from the start" is the threat model at 8:40. NIST's AI RMF says to prioritize risk treatment by impact, likelihood and available resources. The Five Eyes guidance says to classify an agent's actions by impact, likelihood and reversibility, with human approval where the cost of an error is high. In the "AI Control" study, the same small review budget reached 62% safety when a cheap trusted model picked what to review, against 15% when it went to the first cases in line. That was a research testbed, and an extreme case.

**Sources**
- [NIST AI 100-1](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf), MANAGE 1.2. [GOV]
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), p. 22. [GOV]
- Greenblatt, Shlegeris, Sachan and Roger, ["AI Control"](https://arxiv.org/abs/2312.06942) (ICML 2024). [ACADEMIC]

### 10:16 · Fail open, or fail closed

> Checks are software, and software breaks.
>
> Some let requests through unfiltered. Others stop everything. Decide before an outage does.

**What this is getting at.** Decide what happens when the checker itself breaks. Microsoft's docs say that if its content-filtering system is down or too slow, "your request still completes without content filtering", with only an error field to show it. Google says its Model Armor integration on its agent platform skips the check and serves the request when Model Armor can't be reached. Others fail closed and stop everything. LiteLLM's gateway, for one, blocks a request by default whenever a guardrail errors, and its docs say that's "precisely because a guardrail is usually a security control." Failing closed turns a guardrail outage into a product outage. Either can be the right call, as long as it's made before an outage.

**Sources**
- Microsoft Learn, ["Content filtering for Microsoft Foundry Models (classic)"](https://learn.microsoft.com/en-us/azure/foundry-classic/foundry-models/concepts/content-filter) (Aug 4, 2026). [SELF]
- Google Cloud, ["Integrate Model Armor with Gemini Enterprise Agent Platform"](https://docs.cloud.google.com/model-armor/model-armor-vertex-integration), formerly Vertex AI (Oct 13, 2026). [SELF]
- LiteLLM, [Generic Guardrail API docs](https://docs.litellm.ai/docs/adding_provider/generic_guardrail_api). [SELF]

### 10:31 · Guardrails in a box

> Guardrails in a box.
>
> None of them knows your business, like which customer may see which order.
>
> That part is still yours to build.

**What this is getting at.** Every big cloud sells guardrails, with different defaults. Microsoft's default policy turns filters on for the models it sells. Google's built-in harm filters default to off on its newest Gemini models, and Model Armor is off until you set it up. Amazon's Bedrock Guardrails checks nothing until you attach one, and inline it skips tool calls and their results. None of them knows your business rules, such as which customer may see which order, so that stays your job.

**Sources**
- AWS, [Amazon Bedrock Guardrails](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails.html) and its [Converse API notes on tool use](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-use-converse-api.html). [SELF]
- Microsoft Learn, [Foundry default safety policies](https://learn.microsoft.com/en-us/azure/foundry/guardrails/default-safety-policies) (Oct 2026). [SELF]
- Google Cloud, [Model Armor overview](https://docs.cloud.google.com/security-command-center/docs/model-armor-overview) and [Gemini safety filters](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/multimodal/configure-safety-filters) (Oct 2026). [SELF]

### 10:48 · Limit what it can do

> Limit what the system can do.
>
> Least access. A person approves what can't be undone. When a check can't decide, stop and ask.

**What this is getting at.** Because guardrails will miss things, the guidance now is to limit what the system can do. The Five Eyes agencies call least privilege critical, leave the decision about when a human must approve to the system's designers and operators, and want systems set "to fail-safe by default requiring agents to stop and escalate issues to human reviewers in uncertain scenarios." The UK NCSC says protections should focus more on deterministic, non-AI safeguards that constrain what the system can do, rather than just trying to keep malicious content away from the model. In the film, the agent's courier is held at the bank's bollards, a car with the right key is let into the records drive, and a hold lamp waits on a decision.

**Sources**
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), pp. 20 and 22. [GOV]
- [UK NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]
- [UK NCSC blog, "Thinking carefully before adopting agentic AI"](https://www.ncsc.gov.uk/blogs/thinking-carefully-before-adopting-agentic-ai) (May 15, 2026). [GOV]

### 11:07 · Keep revisiting

> Keep revisiting where you check, when, and what happens on a no.

The series' view, as the toll plaza's booths answer one by one. NIST, Microsoft and OWASP all describe threat modelling as ongoing work (8:40).

## Further reading

None of these is in the film.
- **A design that contains injection.** CaMeL plans a task from the trusted request and tracks where each piece of data came from, so injected text can't change the plan. It solved 77% of a benchmark's tasks with provable security, against 84% with no defense. [Debenedetti et al., arXiv 2503.18813](https://arxiv.org/abs/2503.18813) (Mar 2025)
- **Meta's "Rule of Two."** In one session, an agent should have no more than two of three properties, which are reading untrusted input, reaching sensitive systems or data, and changing state or communicating out. [Meta AI](https://ai.meta.com/blog/practical-ai-agent-security/) (Oct 31, 2025) [SELF]
- **The cost keeps rising.** Anthropic's next-generation classifiers add about 1% compute, and 1,700+ hours of red-teaming found no universal jailbreak. [Anthropic](https://www.anthropic.com/research/next-generation-constitutional-classifiers) (Jan 9, 2026) [SELF]

## About this page
- **When checked.** The research was read on Oct 19 and 20, 2026, and the research for this cut on Oct 23, 2026. Every link from the earlier cut was re-checked on Oct 23, 2026, and the links new to this cut were checked on Oct 24, 2026. Some sites, including openai.com, TIME, CNBC and the INFORMS journal site, refuse automated checks. YouTube showed the Black Hat recording's title but not its description.
- **Timestamps.** For the 11:22 cut (Oct 24, evening). Quoted lines are the on-screen captions. The narrator tells the same facts in his own words.
- **Labels.** [SELF] marks an organization describing its own work, product, data or incident. [VENDOR] marks a company that sells related security or AI products. [PRESS] is news coverage. [GOV], [LAW], [STANDARD] and [ACADEMIC] mark government guidance, law, standards bodies and peer-reviewed research. [DATA] marks a count made for this film from public data, with the method in the text. Preprints are labelled in the text. None of these is independent confirmation by itself.
- **What's real.** The highway, the crash-test cars, the trucks, the courier, the toll plaza, the car dealer's lot, Microduck, the robot arm, the AI agent character and the x-ray diagrams are illustrations. The robot dog is footage from Black Hat's recording of BT6's talk, credited on screen, and cropped so no presenter's face is in frame. No real people are shown apart from Pliny's public X profile and a photo of Sander Schulhoff, credited on screen. The crash test follows the MASH standard. The incidents and numbers are real.
- **The series' view.** "AI has guardrails too… just as easy to misunderstand", the comparison with firewalls and antivirus, and "Keep revisiting where you check…" are opinion.
- **Honest limits.** Most incident accounts here come from the companies involved. The adaptive-attack results assume a strong attacker who can see the detectors' scores. The timing numbers come from different setups and shouldn't be compared as if one lab measured them all. The miss and false-alarm rates are vendors grading their own tools on their own tests. The vulnerability and registry counts are our own, from public data, and they measure disclosed flaws and registrations rather than attacks or use. Microduck's sales figure is Hugging Face's own, reported by CNBC. Three lines are the film's own simplifications rather than sourced findings. The film says attackers mostly want one of two things (4:25), but no source counts their goals. It calls rules "instant" (2:24), but no vendor publishes a time for them. And it calls the two ways at 9:56 and 10:06 common, but the docs describe several patterns and no source counts which ones teams use.
- **Left out on purpose.** A "3,000 attempts" figure for the $1 SUV, which isn't in the original report. Colorado's "reasonable care" AI duty, replaced before it took effect. "The largest" contest for HackAPrompt, since several contests claim that on different numbers. "Virtually" and "panel" for Pliny at Black Hat, since it was one team's talk and no source says Pliny took part remotely. Any claim that Microduck descends from the Open Duck Mini project, which no official source makes, or that its hardware is open source.
- **Licence.** Quotes from NCSC and UK AI Security Institute pages contain public sector information licensed under the Open Government Licence v3.0. OWASP material is CC BY-SA 4.0.
- **Corrections.** Welcome as a GitHub issue.
