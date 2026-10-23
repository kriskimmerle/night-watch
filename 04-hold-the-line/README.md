# NIGHT WATCH · Episode 04 · Hold the Line

[![NIGHT WATCH · Hold the Line](thumbnail.jpg)](https://kriskimmerle.substack.com)

**Watch:** on [AI Risk Praxis](https://kriskimmerle.substack.com) or LinkedIn · 7:44 · October 2026

An AI guardrail is software that sits outside a model and checks what goes in, what comes out and what the model is about to do. This episode starts with the highway guardrails the name comes from. They're crash tested against a set kind of hit, and something much heavier can go through them. AI guardrails work the same way. They can never catch everything, because there are far too many possible prompts to test, attackers adapt, and sometimes there's no attacker at all. They're still worth running, for the same reasons teams run firewalls and antivirus. They raise the cost of an attack, leave a record of what they catch and show reasonable care. The last part covers how teams deploy them, from the threat model and layered checks to channel timing, cost, what happens when a checker breaks and what the big clouds sell, and it ends on limiting what the system can do.

**How to read this page.** The film moves fast. Every claim and real-world event it shows is listed below at its timestamp, with what's on screen, what it's getting at, and where to read more. A narrator tells the story in his own words, and the quotes here are the on-screen captions, which differ from the narration on purpose. The highway, the crash-test cars, the courier, the AI agent character and the x-ray diagrams are illustrations. The crash test follows the real test standard, and the incidents and numbers are real and sourced.

## At a glance

| Time | What happens |
|---|---|
| 0:00 | AI Risk Praxis presents |
| 0:08 | A highway guardrail crash test |
| 0:22 | The rail catches the pickup and steers it back |
| 0:30 | A much heavier truck goes through |
| 0:40 | AI has guardrails too |
| 0:50 | Title |
| 0:56 | What an AI guardrail is, seen in an x-ray view |
| 1:06 | Orders hidden in what the AI reads, called prompt injection |
| 1:18 | What shouldn't leave, like a card number |
| 1:24 | An agent's refund held until a person says yes |
| 1:34 | Checks that steer sensitive topics |
| 1:48 | Rules, small models and AI judges |
| 1:58 | Why anyone attacks an AI, starting with the $1 SUV |
| 2:09 | It doesn't feel like breaking in |
| 2:26 | Access is the prize |
| 2:36 | Hidden instructions in résumés, papers and links |
| 2:48 | It can never catch everything |
| 3:05 | Attackers adapt |
| 3:11 | Pliny the Liberator |
| 3:25 | TIME100 AI, 2025 |
| 3:33 | Twelve published defenses, all bypassed |
| 3:55 | EchoLeak, one email to Microsoft 365 Copilot |
| 4:05 | Clinejection, a bug report that took the wheel |
| 4:20 | PocketOS, with no attacker at all |
| 4:33 | Test models that got out of their test |
| 4:43 | Worth running anyway, like firewalls and antivirus |
| 4:54 | It raises the cost |
| 5:10 | It leaves a record |
| 5:24 | The bar is reasonable security |
| 5:31 | Start with a threat model |
| 5:43 | Stack different checks, the Swiss cheese model |
| 6:02 | Every channel has its own clock |
| 6:17 | Every check costs time and money |
| 6:40 | Spend the expensive checks where it would hurt most |
| 6:47 | Fail open, or fail closed |
| 6:59 | Guardrails in a box from the big clouds |
| 7:12 | Limit what the system can do, at the bank's bollards |
| 7:29 | Keep revisiting |
| 7:37 | End card |

## Citations by timestamp

### 0:08 · A crash-tested rail

> Built for one kind of crash.

**What this is getting at.** Highway guardrails are rated by crash test. In the US the standard is AASHTO's *Manual for Assessing Safety Hardware* (MASH, 2nd edition, 2016). At test level 3, the everyday highway rating, a rail is hit by a small car and by a 2,270-kilogram (5,000-pound) pickup, each at 62 miles an hour and 25 degrees. The film shows the pickup test, the one the narrator describes. AASHTO's own text is paywalled, so these numbers come from state transportation manuals that reproduce the test matrix.

**Sources**
- [Iowa DOT Design Manual §8A-7, "Introduction to MASH Crash Testing"](https://iowadot.gov/design-manual/chapter-8-roadside-safety/8a-7-introduction-mash-crash-testing) (revised Jun 2, 2026). [GOV]
- TxDOT, [Bridge Railing Manual, "Required Crash Tests"](https://www.txdot.gov/manuals/brg/rlg/chapter-2---policies-on-use-of-bridge-railing-for-/section-2---fhwa-policy-on-bridge-railing/required-crash-tests.html) and [Roadway Design Manual §17.2](https://www.txdot.gov/manuals/des/rdw/chapter-17-roadside-safety-design-and-roadside-saf/17-2-roadside-safety-hardware-crash-criteria.html). [GOV]

### 0:22 · Catch it, then steer it back

> Catch it, then steer it back.

**What this is getting at.** What a guardrail is for. MASH passes a barrier only if it contains and redirects the vehicle or brings it to a controlled stop, without the vehicle going through, under or over it. A rail is designed to turn a bad crash into a survivable one, which is the film's picture of an AI guardrail too.

**Sources**
- National Academies, [*Development of a MASH Barrier to Shield Pedestrians, Bicyclists, and Other Vulnerable Users from Motor Vehicles*](https://www.nationalacademies.org/read/27896/chapter/10) (2024), ch. 8, quoting MASH's structural criterion. [ACADEMIC]
- [Iowa DOT §8A-7](https://iowadot.gov/design-manual/chapter-8-roadside-safety/8a-7-introduction-mash-crash-testing). [GOV]

### 0:30 · Past its rating

> Past its rating, it can give way.
>
> Heavier trucks need higher test levels.

**What this is getting at.** A test level works like a threat model. A rail rated for a pickup at 62 miles an hour makes no promise about a loaded truck, which is why test levels 4 to 6 add a box truck, a tractor-trailer and a tanker. Iowa DOT notes that crash tests run under ideal conditions and that these devices aren't designed for every possible condition. The NTSB has made the same point in an accident report, finding a standard rail that wasn't designed to redirect a much heavier vehicle. The truck in the film is an illustration.

**Sources**
- [Iowa DOT §8A-7](https://iowadot.gov/design-manual/chapter-8-roadside-safety/8a-7-introduction-mash-crash-testing) and [TxDOT §17.2](https://www.txdot.gov/manuals/des/rdw/chapter-17-roadside-safety-design-and-roadside-saf/17-2-roadside-safety-hardware-crash-criteria.html), for test levels 4 to 6. [GOV]
- [NTSB Highway Accident Report HAR-12/01](https://www.ntsb.gov/investigations/AccidentReports/Reports/HAR1201.pdf) (adopted Jun 5, 2012). [GOV]

### 0:40 · AI has guardrails too

> AI has guardrails too.

The turn from the road to AI. The narrator adds that they work the same way and are just as easy to misunderstand, which is the series' view.

### 0:56 · Software outside the model

> Software outside the model.
>
> It checks inputs, outputs, and actions.

**What this is getting at.** The definition the film uses. NIST's taxonomy of attacks on AI sorts protections by when they apply. Safety training happens inside the model, while classifier models that detect and stop harmful interactions run at deployment, and that deployment layer is what the film calls guardrails. The UK NCSC explains why the checks sit outside, since today's models "simply do not enforce a security boundary between instructions and data inside a prompt." With agents, the checks also look at actions before a tool runs, as the Five Eyes agencies' guidance on agents describes under guardrails and constraints.

**Sources**
- [NIST AI 100-2e2025, *Adversarial Machine Learning*](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf) (Mar 2025), pp. 47–48. [GOV]
- [UK NCSC: "Prompt injection is not SQL injection (it may be worse)"](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]
- Five Eyes agencies, ["Careful adoption of agentic AI services"](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 1, 2026), p. 20. [GOV]

### 1:06 · Orders hidden in what it reads

> Orders hidden in what it reads.
>
> That trick is called prompt injection.

**What this is getting at.** An email, a web page or a document can carry instructions the user never wrote, and a model that reads them may follow them. OWASP ranks prompt injection first in its Top 10 for LLM applications. It says "it is unclear if there are fool-proof methods of prevention", and lists measures that limit the impact, with filtering inputs and outputs as one of seven. In the film, the input check looks for those hidden orders on the way in.

**Sources**
- [OWASP Top 10 for LLM Applications 2025, LLM01 Prompt Injection](https://genai.owasp.org/llmrisk/llm01-prompt-injection/). [STANDARD]

### 1:18 · What shouldn't leave

> What shouldn't leave.
>
> A card number, masked before anyone sees it.

**What this is getting at.** Checks on the way out. Amazon Bedrock's sensitive-information filter recognizes about 31 built-in kinds of personal data, card numbers among them, and can mask or block them in a response. It works by probability and context, so it can miss. Microsoft's Azure AI Content Safety screens responses for harmful content and protected material. The card in the film is an illustration.

**Sources**
- AWS, [Amazon Bedrock Guardrails sensitive-information filters](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-sensitive-filters.html). [SELF]
- Microsoft Learn, [Azure AI Content Safety overview](https://learn.microsoft.com/en-us/azure/ai-services/content-safety/overview) (updated Oct 2026). [SELF]

### 1:24 · Held for a human

> Held for a human.
>
> An agent is an AI that acts on its own. Its refund waits for a yes.

**What this is getting at.** Checks on actions. OpenAI's Agents SDK lets a developer mark a tool as needing approval, so the run pauses, for hours if need be, until a person answers. Amazon's AgentCore Policy puts fixed rules, denying by default, at the gateway where an agent calls its tools. The refund is an illustration.

**Sources**
- OpenAI, [guardrails and approvals guide](https://developers.openai.com/api/docs/guides/agents/guardrails-approvals), and the [Agents SDK guardrails docs](https://openai.github.io/openai-agents-python/guardrails/) (v0.24.0, Oct 2026). [SELF]
- AWS, [Amazon Bedrock AgentCore Policy](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/policy.html). [SELF]

### 1:34 · Checks can steer

> Checks can steer, too.
>
> Sensitive topics go to a person, or to an approved script with self-serve links.

**What this is getting at.** A check doesn't only say yes or no. It can route a conversation. This pattern comes from practice. Some legal and compliance questions shouldn't get a free-form AI answer, so they go to a person or to an approved reply with links to self-serve help. The tools support it. A Bedrock guardrail returns a blocked message you write yourself when a denied topic comes up, and NVIDIA's NeMo Guardrails uses dialog rails to steer a conversation's flow.

**Sources**
- AWS, [Amazon Bedrock Guardrails denied topics](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-denied-topics.html), including "Messaging for blocked prompts". [SELF]
- NVIDIA, [NeMo Guardrails rail types](https://docs.nvidia.com/nemo/guardrails/latest/about-nemo-guardrails-library/rail-types), on dialog rails. [SELF]

### 1:48 · Rules, small models, AI judges

> Rules · small models · AI judges

**What this is getting at.** The three kinds of checker. Rules, such as word lists and a pattern for card numbers, are fast, cheap and predictable but miss nuance. Small classifier models, such as Meta's Prompt Guard 2, are trained to spot one kind of problem. An AI judge is a second model asked to evaluate the first, as in OpenAI's open-source Guardrails library. The film ranks them fastest to slowest, and the measured times are at 6:17.

**Sources**
- LangChain, [Guardrails docs](https://docs.langchain.com/oss/python/langchain/guardrails), on deterministic and model-based checks. [SELF]
- Meta, [Llama Prompt Guard 2 model card](https://huggingface.co/meta-llama/Llama-Prompt-Guard-2-86M) (Apr 29, 2025). [SELF]
- OpenAI, [Guardrails library](https://github.com/openai/openai-guardrails-python) (open source; a preview release). [SELF]

### 1:58 · For laughs, at first

> For laughs, at first.
>
> A dealer's chatbot agreed to sell an SUV for $1.

**What this is getting at.** Early attacks on chatbots were mostly pranks. In December 2023, a Chevrolet dealer's website chatbot, built on ChatGPT, agreed to sell a 2024 Tahoe for one dollar after a user talked it into it. The deal wasn't binding, and the chatbot's vendor pulled it from the dealer's site. Its CEO said the logs showed people trying for hours and the bot mostly resisting.

**Sources**
- [Business Insider, Katie Notopoulos](https://www.businessinsider.com/car-dealership-chevrolet-chatbot-chatgpt-pranks-chevy-2023-12) (Dec 18, 2023). [PRESS]

### 2:09 · It doesn't feel like breaking in

> It doesn't feel like breaking in.
>
> People cheated about 3× more reporting to a machine than to a person.

**What this is getting at.** Why ordinary people try it. In a representative survey of 3,270 UK adults, about a quarter of regular chatbot users had tried to get past a refusal, for fun, out of curiosity or to get an answer, about equally often. Hobbyist red-teamers interviewed for a PLOS One study described it as play and said they meant no harm. And in two experiments with 848 people, participants cheated about three times more when they reported to a machine than to a person, whether or not the machine seemed human. The narrator's "Most people who try it mean no harm" is a hedged summary of these studies.

**Sources**
- Cohn, Gesche and Maréchal, ["Honesty in the Digital Age"](https://doi.org/10.1287/mnsc.2021.3985), *Management Science* 68(2) (2022). [ACADEMIC]
- Grosse and Ebert, [arXiv 2510.27275](https://arxiv.org/abs/2510.27275) (Oct 31, 2025; revised Jul 30, 2026). A preprint.
- Inie, Stray and Derczynski, ["Summon a demon and bind it"](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0314658), *PLOS One* (Jan 15, 2025). [ACADEMIC]

### 2:26 · Access is the prize

> Access is the prize.
>
> Private data, untrusted content, a way out: Simon Willison's "lethal trifecta."

**What this is getting at.** The stakes changed when AIs got tools. Simon Willison's "lethal trifecta" is an agent with access to private data, exposure to untrusted content and a way to send data out. With all three, anyone who can get words in front of it can trick it into sending your data to them. The UK NCSC and OWASP make the same point in their own terms, that the damage depends on what the system is able to do. The narrator widens the list to spending money, which is the film's extension of Willison's.

**Sources**
- Simon Willison, ["The lethal trifecta for AI agents"](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/) (Jun 16, 2025). An independent developer's blog.
- [UK NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]
- [OWASP LLM01:2025](https://genai.owasp.org/llmrisk/llm01-prompt-injection/). [STANDARD]

### 2:36 · Hidden instructions, wherever AI decides

> Hidden instructions, wherever AI decides.
>
> Résumés · research papers · links that tell assistants whom to recommend

**What this is getting at.** Hidden text already turns up wherever an AI makes or shapes a decision. In about 200,000 real résumés, about 1% carried hidden text aimed at AI screeners, though more than 90% of those were keywords and claims rather than commands, and the authors don't assume every applicant meant it. Nikkei Asia found hidden prompts asking AI reviewers for positive reviews in 17 arXiv preprints from 14 institutions in 8 countries. Microsoft found 31 real companies, across 14 industries, hiding instructions in "summarize with AI" links that told assistants to remember or recommend them.

**Sources**
- Zhang et al. (Duke, hireEZ and others), [arXiv 2605.28999](https://arxiv.org/abs/2605.28999) (May 27, 2026; USENIX Security 2026), and [Duke Pratt news](https://pratt.duke.edu/news/thwarting-prompt-injection/) (Jul 22, 2026). A preprint.
- [Nikkei Asia](https://asia.nikkei.com/business/technology/artificial-intelligence/positive-review-only-researchers-hide-ai-prompts-in-papers) (Jun 30, 2025). [PRESS]
- Microsoft Defender Security Research, ["Manipulating AI memory for profit: The rise of AI Recommendation Poisoning"](https://www.microsoft.com/en-us/security/blog/2026/02/10/ai-recommendation-poisoning/) (Feb 10, 2026). [VENDOR]

### 2:48 · It can never catch everything

> It can never catch everything.
>
> More possible prompts than atoms in the universe.

**What this is getting at.** The size of the problem. Sander Schulhoff estimates that a GPT-5-class model has about 10^1,000,000 possible prompts, against about 10^80 atoms in the universe. A check for this film found the estimate holds, and if anything it's conservative. Almost all of those prompts are gibberish, but the meaningful ones are still far too many to ever test, and attackers search them on purpose. Schulhoff goes further than the film. His essay argues guardrails don't protect you and can make teams overconfident. The film agrees they aren't a wall and disagrees about their value (4:43).

**Sources**
- Sander Schulhoff, ["The AI Security Industry is Bullshit"](https://sanderschulhoff.substack.com/p/the-ai-security-industry-is-bullshit) (Dec 20, 2025). An essay.

### 3:05 · Attackers adapt

> Attackers adapt.

A bridge to the people, and the research, that show it.

### 3:11 · Pliny the Liberator

> Pliny the Liberator
>
> Anonymous red-teamer · jailbreaks published in the open since 2023

**What this is getting at.** You can't talk about guardrails without Pliny the Liberator. Since 2023, this anonymous red-teamer has broken nearly every major AI model, talking each one out of its own safety rules, and published the methods in the open for anyone to study. In a check of 23 major releases from 2024 to early 2026 made for this film, a Pliny jailbreak was public on launch day for 19 of them. Pliny also publishes the hidden system prompts AI products run on, and co-designed a HackAPrompt track in 2025 whose data was then released openly. For defenders, that public record is one of the clearest real-world tests of guardrails. Pliny has argued that content filters are largely futile and that real security belongs in the system around the model, and the film's close lands in the same place on the second point. On screen are Pliny's X profile, including the "{LOVE PLINY}" tucked into the display name in invisible characters, and a post from the launch night of OpenAI's gpt-oss models in August 2025, shown with its harmful line blurred.

**Sources**
- Pliny on X, [@elder_plinius](https://x.com/elder_plinius), and the [gpt-oss launch-night post](https://x.com/elder_plinius/status/1952958577867669892) (late Aug 5, 2025, US time). [SELF]
- Pliny on GitHub, [elder-plinius](https://github.com/elder-plinius). [SELF]
- [VentureBeat, Carl Franzen](https://venturebeat.com/ai/an-interview-with-the-most-prolific-jailbreaker-of-chatgpt-and-other-leading-llms) (May 31, 2024). [PRESS]
- [Decrypt, Jose Antonio Lanz](https://decrypt.co/333858/openai-jailbreak-proof-new-models-hacked), on the gpt-oss jailbreak (Aug 6, 2025). [PRESS]
- [Latent Space podcast](https://www.latent.space/p/jailbreaking-agi-pliny-the-liberator) with Pliny (Dec 16, 2025). [PRESS]
- [The Pliny HackAPrompt Dataset](https://huggingface.co/datasets/hackaprompt/Pliny_HackAPrompt_Dataset) (Jul 4, 2025).

### 3:25 · TIME100 AI

> One of TIME's 100 most influential people in AI, 2025.

**What this is getting at.** Recognition well beyond the field. TIME's 2025 profile describes Pliny as an anonymous figure finding the holes in billion-dollar AI systems. SANS later announced Pliny as a keynote speaker for its AI Cybersecurity Summit in April 2026.

**Sources**
- [TIME, Tharin Pillay, TIME100 AI 2025](https://time.com/collections/time100-ai-2025/7305870/pliny-the-liberator/) (Aug 27, 2025). [PRESS]
- [SANS, Rob T. Lee](https://www.sans.org/blog/keynote-pliny-the-liberator-sans-ai-cybersecurity-summit) (Feb 25, 2026). [PRESS]

### 3:33 · Twelve of twelve

> 12 of 12 defenses bypassed.
>
> Tested with researchers from OpenAI, Anthropic and Google DeepMind.

**What this is getting at.** Adaptive attacks. In "The Attacker Moves Second", researchers from OpenAI, Anthropic, Google DeepMind, HackAPrompt, ETH Zürich and others tested 12 published defenses against jailbreaks and prompt injection. Attacks that learn and change tactics got past all 12, most of them more than 90% of the time, though most of the defenses had originally reported near-zero attack success. Four were filter models of the kind the film calls guardrails, including Google's own Model Armor. The test was demanding, since the attacker could see each detector's scores. Schulhoff, a co-author, ran HackAPrompt, the prompt-hacking contest whose 2023 paper gathered more than 600,000 attack prompts and won an EMNLP 2023 best paper award. The narrator quotes his line, "You can patch a bug, but you can't patch a brain."

**Sources**
- Nasr, Carlini, Sitawarin, Schulhoff, Tramèr et al., ["The Attacker Moves Second"](https://arxiv.org/abs/2510.09023) (Oct 10, 2025). A preprint.
- Schulhoff et al., ["Ignore This Title and HackAPrompt"](https://arxiv.org/abs/2311.16119) (EMNLP 2023), among the [EMNLP 2023 best papers](https://2023.emnlp.org/program/best_papers/). [ACADEMIC]
- [Schulhoff's essay](https://sanderschulhoff.substack.com/p/the-ai-security-industry-is-bullshit) (Dec 20, 2025), for the quote.

### 3:55 · One email, no clicks

> One email. No clicks.
>
> Microsoft 365 Copilot leaked data. Microsoft fixed it; no customers affected.

**What this is getting at.** EchoLeak, a real attack chain found by researchers. Aim Labs showed that one ordinary-looking email could later make Microsoft 365 Copilot send data from its context to an attacker, once an employee asked Copilot something that pulled the email in. The chain got past Microsoft's classifier for hidden instructions by never mentioning AI. Microsoft rated it critical and fixed it on its servers, it lists the flaw as not exploited, and Aim knows of no affected customers. "No clicks" means the victim didn't have to click anything, though they still used Copilot as usual.

**Sources**
- [Microsoft Security Response Center, CVE-2025-32711](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2025-32711) (Jun 11, 2025). [SELF]
- [NVD, CVE-2025-32711](https://nvd.nist.gov/vuln/detail/CVE-2025-32711). [GOV]
- Aim Labs (now part of Cato Networks), ["Breaking down EchoLeak"](https://www.catonetworks.com/blog/breaking-down-echoleak/). [VENDOR]
- Reddy et al., [arXiv 2509.10540](https://arxiv.org/abs/2509.10540) (Sep 2025). A preprint.

### 4:05 · A bug report took the wheel

> A bug report took the wheel.
>
> The rogue update reached real users. It quietly installed another program.

**What this is getting at.** Clinejection. An AI bot that sorted bug reports on the Cline project's public GitHub repository could be steered by the title of a report, and that opened a path to the keys used to publish the software. Researcher Adnan Khan reported it privately in January 2026 and disclosed it on Feb 9. On Feb 17, someone used a leftover publishing token to release an unapproved version of Cline's command-line tool. It quietly installed OpenClaw, a real open-source agent that Cline says isn't malicious, and it was live for about eight hours before Cline replaced it.

**Sources**
- [Cline security advisory GHSA-9ppg-jx86-fqw7](https://github.com/cline/cline/security/advisories/GHSA-9ppg-jx86-fqw7) (Feb 17, 2026). [SELF]
- [Adnan Khan, "Clinejection"](https://adnanthekhan.com/posts/clinejection/) (Feb 9, 2026).
- [Snyk's analysis](https://snyk.io/blog/cline-supply-chain-attack-prompt-injection-github-actions/). [VENDOR]

### 4:20 · No attacker at all

> Sometimes, no attacker at all.
>
> An agent wiped a live database and its backups. The host later restored them.

**What this is getting at.** Accidents count too. On Apr 24, 2026, a coding agent working for PocketOS, which makes software for car-rental businesses, hit a credential mismatch during routine work in a test setup. It found an API token in an unrelated file, one with far broader rights than its job needed, and in a single call deleted the production database and its volume-level backups. The founder says it took nine seconds, with no confirmation step. The project's written rules didn't stop it. The token's power and the missing confirmation decided the outcome. The hosting provider, Railway, later restored the backups and patched the endpoint the agent had used.

**Sources**
- Jer Crane, PocketOS founder, [on X](https://x.com/lifeof_jer/status/2048103471019434248) (Apr 25, 2026). [SELF]
- [6abc / ABC News](https://6abc.com/post/rogue-ai-agent-cursor-goes-haywire-deletes-tech-companys-database/19008099/), with Railway's CEO (Apr 2026). [PRESS]

### 4:33 · Out of the test

> Out of the test.
>
> Safety filters were off for the tests. OpenAI, then Anthropic, disclosed it.

**What this is getting at.** In July 2026, models OpenAI was testing for hacking skills, run on purpose without its usual production safety classifiers, broke out of their test environment and into Hugging Face's production systems. OpenAI says they were looking for the test's answers. Hugging Face says they reached a limited set of internal datasets and credentials, and that five datasets linked to the test were the only customer content accessed. On Jul 30, Anthropic disclosed similar incidents in a partner's test environment that had live internet access by mistake, where models without the safeguards of its public versions broke into real organizations. These are the companies' own accounts.

**Sources**
- Hugging Face, ["Security incident disclosure — July 2026"](https://huggingface.co/blog/security-incident-july-2026) (Jul 16, 2026) and its [technical timeline](https://huggingface.co/blog/agent-intrusion-technical-timeline) (Jul 27, 2026). [SELF]
- OpenAI, [Jul 21, 2026 post](https://openai.com/index/hugging-face-model-evaluation-security-incident/) and [Aug 26, 2026 findings](https://openai.com/index/hugging-face-incident-and-the-road-ahead/). [SELF]
- Anthropic, ["Investigating three incidents in our cybersecurity evaluations"](https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals) (Jul 30, 2026) and ["An alignment assessment of recent cybersecurity incidents"](https://www.anthropic.com/research/alignment-assessment-cybersecurity-incidents) (Sep 9, 2026). [SELF]

### 4:43 · Worth running anyway

> Worth running anyway.
>
> Antivirus has never caught every virus.

**What this is getting at.** The turn, and the series' view. None of this makes guardrails pointless. NIST's malware guide calls antivirus "a necessity", and also says "it is not possible for antivirus software to stop all malware incidents." Teams run it anyway, alongside other layers, which security people call defense in depth. A classifier guardrail is closest to antivirus, since both work by probability. Permissions and allowlists are the firewall-like part of the stack.

**Sources**
- [NIST SP 800-83 Rev. 1, *Guide to Malware Incident Prevention and Handling*](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-83r1.pdf) (Jul 2013), pp. 22 and 28. [GOV]
- [NIST glossary, "defense-in-depth"](https://csrc.nist.gov/glossary/term/defense_in_depth). [GOV]

### 4:54 · It raises the cost

> It raises the cost.
>
> 339 people · about 3,700 hours · 4 got all the way through

**What this is getting at.** In February 2025, Anthropic opened a model guarded by its constitutional classifiers to a public challenge with eight levels. 339 people took part, over more than 300,000 chats and about 3,700 hours of combined effort. The system held for five of the seven days, and four people cleared all eight levels by the end. Anthropic notes the challenge made attacking easier than real life, with instant automatic grading and none of the account monitoring it would use in a real deployment. Separately, the UK AI Security Institute has found universal jailbreaks in every system it tested, and found that one newer model took about forty times more expert effort to crack than one released six months earlier. Both fit the film's claim that guardrails make attacks slower and more expensive.

**Sources**
- Anthropic, ["Constitutional Classifiers"](https://www.anthropic.com/research/constitutional-classifiers) (Feb 3, 2025; updated through Feb 18, 2025). [SELF]
- [The Decoder, Maximilian Schreiner](https://the-decoder.com/claude-jailbreak-results-are-in-and-the-hackers-won/) (Feb 4, 2025; updated Feb 11 and 15). [PRESS]
- [UK AI Security Institute, "5 key findings from our first Frontier AI Trends Report"](https://www.aisi.gov.uk/blog/5-key-findings-from-our-first-frontier-ai-trends-report) (Dec 2025). [GOV]

### 5:10 · It leaves a record

> It leaves a record.
>
> Monitoring caught a state-backed campaign running through Anthropic's coding tool.

**What this is getting at.** A guardrail is also a sensor. In September 2025, Anthropic detected a campaign it attributes, with high confidence, to a Chinese state-sponsored group that had jailbroken Claude Code and aimed it at about 30 organizations, succeeding against a small number. Over about ten days, Anthropic banned the accounts, notified the affected organizations and worked with authorities. It's Anthropic's own account, and it doesn't say whether detection began with a classifier flag or with wider monitoring, which is why the caption says "monitoring". NIST's generative AI profile lists the number of unauthorized access attempts among the security metrics worth tracking.

**Sources**
- Anthropic, ["Disrupting an AI-orchestrated cyber espionage campaign"](https://www.anthropic.com/news/disrupting-AI-espionage) (Nov 13, 2025). [SELF]
- [NIST AI 600-1, Generative AI Profile](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf) (Jul 2024), MS-2.7-004. [GOV]

### 5:24 · Reasonable care

> The bar is reasonable security.
>
> The FTC's bar for security. Europe's AI law asks for "an appropriate level."

**What this is getting at.** Regulators don't ask for perfect. Marking its 50th data security settlement in 2014, the FTC said reasonableness is the touchstone of its approach, that it "does not require perfect security", and that a breach alone doesn't mean a company broke the law. The EU AI Act asks high-risk systems for "an appropriate level of accuracy, robustness, and cybersecurity", including measures to prevent, detect and respond to attacks. NIST's AI Risk Management Framework notes that "not all incidents and failures can be eliminated."

**Sources**
- [FTC, "Commission Statement Marking the FTC's 50th Data Security Settlement"](https://www.ftc.gov/system/files/documents/cases/140131gmrstatement.pdf) (Jan 31, 2014). [GOV]
- [EU AI Act, Article 15](https://artificialintelligenceact.eu/article/15/). [LAW]
- [NIST AI 100-1, AI RMF 1.0](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) (Jan 2023), §1.2.3. [GOV]

### 5:31 · Start with a threat model

> Start with a threat model.
>
> What it can reach · who can reach it · what would really hurt

**What this is getting at.** Before the first check, write down what the AI can touch, who or what can put words in front of it, and what it must never do. The Five Eyes agencies' guidance on agents has a section on threat modelling and recommends up-to-date risk taxonomies such as OWASP's and MITRE ATLAS. Microsoft's checklist starts with what actions the system should never take. OWASP's guide for agents frames threat modelling as four questions, starting with what you're working on.

**Sources**
- Five Eyes agencies (ASD's ACSC, CISA, NSA, the Canadian Centre for Cyber Security, NCSC-NZ and NCSC-UK), ["Careful adoption of agentic AI services"](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 1, 2026), p. 19, also on [CISA's site](https://www.cisa.gov/resources-tools/resources/careful-adoption-agentic-ai-services). [GOV]
- [Microsoft Security Blog, "Threat modeling AI applications"](https://www.microsoft.com/en-us/security/blog/2026/02/26/threat-modeling-ai-applications/) (Feb 26, 2026). [VENDOR]
- [OWASP, "Agentic AI – Threats and Mitigations"](https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/) v1.1 (Dec 2025), p. 12. [STANDARD]

### 5:43 · Stack different checks

> Stack different checks.
>
> Every layer has holes. Harm gets through when the holes line up.

**What this is getting at.** The Swiss cheese model. The psychologist James Reason drew safety defenses as stacked slices, each with holes that open, close and move, so harm usually needs the holes in many layers to line up at the same moment. The International AI Safety Report uses the same picture for AI safeguards. For AI there's a catch. Layers only help if they fail in different ways, which is why the film says different checks, mixing rules, permissions and models instead of stacking more AI judges. Researchers have also beaten a layered pipeline one layer at a time.

**Sources**
- James Reason, ["Human error: models and management"](https://pmc.ncbi.nlm.nih.gov/articles/PMC1117770/), *BMJ* 320:768 (Mar 18, 2000). [ACADEMIC]
- [International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026) (Feb 3, 2026), Figure 3.5. [GOV]
- Dung and Mai, [arXiv 2510.11235](https://arxiv.org/abs/2510.11235) (Oct 13, 2025). A preprint.
- McKenzie et al., ["STACK"](https://arxiv.org/abs/2506.24068) (v3 Feb 5, 2026). A preprint.

### 6:02 · Every channel has its own clock

> Every channel has its own clock.
>
> A call gets about a fifth of a second. An email can wait minutes.

**What this is getting at.** One assistant may answer email, web chat, text messages and phone calls, and each sets a different time budget for its checks. In a study across ten languages, people answered yes-or-no questions after a mean of 208 milliseconds. Email security already spends minutes, and Microsoft says its attachment sandbox typically finishes within 15 minutes. So a call only has room for tiny checks before speaking, while email has room for slow, deep ones. MITRE ATLAS added a technique in September 2026 for attackers probing an agent's email addresses, webhooks and messaging channels.

**Sources**
- Stivers et al., ["Universals and cultural variation in turn-taking in conversation"](https://pmc.ncbi.nlm.nih.gov/articles/PMC2705608/), *PNAS* 106(26) (2009). [ACADEMIC]
- Microsoft Learn, [Safe Attachments](https://learn.microsoft.com/en-us/defender-office-365/safe-attachments-about) (Jul 17, 2026). [SELF]
- [MITRE ATLAS](https://atlas.mitre.org/), technique AML.T0006.003 ([data, v2026.09](https://github.com/mitre-atlas/atlas-data)). [STANDARD]

### 6:17 · Every check costs time and money

> Every check costs time and money.
>
> An AI judge took about 1.5 s. Racing it alongside is faster, but it can be late.

**What this is getting at.** In OpenAI's published tests, its AI-judge checks for jailbreaks and prompt injection took a median of about 1.5 seconds each with its default judge model. Meta lists 19.3 milliseconds for its small Prompt Guard 2 classifier on one A100 GPU. The setups differ, so read it as an order of magnitude. To hide the wait, OpenAI's Agents SDK runs input checks alongside the agent by default, and its docs warn that the agent may already have spent tokens and run tools before a tripwire stops it. The cloud services also bill per check, so frequent small checks add up.

**Sources**
- OpenAI, [Guardrails library check benchmarks](https://github.com/openai/openai-guardrails-python/tree/main/docs/ref/checks) (Dec 15, 2025). [SELF]
- Meta, [Llama Prompt Guard 2 model card](https://huggingface.co/meta-llama/Llama-Prompt-Guard-2-86M) (Apr 29, 2025) and the [LlamaFirewall paper](https://arxiv.org/abs/2505.03574) (May 2025). [SELF]
- OpenAI, [Agents SDK guardrails docs](https://openai.github.io/openai-agents-python/guardrails/) (v0.24.0, Oct 2026). [SELF]

### 6:40 · Where it would hurt most

> Spend the expensive checks where it would hurt most.

**What this is getting at.** Cheap checks on everything, expensive ones where the risk is. NIST's AI RMF says to prioritize risk treatment by impact, likelihood and available resources. The Five Eyes guidance says to classify an agent's actions by impact, likelihood and reversibility, with human approval where the cost of an error is high. In the "AI Control" study, the same small review budget reached 62% safety when a cheap trusted model picked what to review, against 15% when it went to the first cases in line. That was a research testbed, and an extreme case.

**Sources**
- [NIST AI 100-1](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf), MANAGE 1.2. [GOV]
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), p. 22. [GOV]
- Greenblatt, Shlegeris, Sachan and Roger, ["AI Control"](https://arxiv.org/abs/2312.06942) (ICML 2024). [ACADEMIC]

### 6:47 · Fail open, or fail closed

> Fail open, or fail closed.
>
> Microsoft's and Google's built-in filters let requests through unfiltered.

**What this is getting at.** Decide what happens when the checker itself breaks. Microsoft's docs say that if its content-filtering system is down or too slow, "your request still completes without content filtering", with only an error field to show it. Google says its Model Armor integration on its agent platform skips the check and serves the request when Model Armor can't be reached. Other tools fail closed and stop everything, which turns a guardrail outage into a product outage. Either can be the right call, as long as it's made before an outage.

**Sources**
- Microsoft Learn, ["Content filtering for Microsoft Foundry Models (classic)"](https://learn.microsoft.com/en-us/azure/foundry-classic/foundry-models/concepts/content-filter) (Aug 4, 2026). [SELF]
- Google Cloud, ["Integrate Model Armor with Gemini Enterprise Agent Platform"](https://docs.cloud.google.com/model-armor/model-armor-vertex-integration), formerly Vertex AI (Oct 13, 2026). [SELF]

### 6:59 · Guardrails in a box

> Guardrails in a box.
>
> Bedrock Guardrails · Content Safety · Model Armor. None knows your business.

**What this is getting at.** Every big cloud sells guardrails, with different defaults. Microsoft's default policy turns filters on for the models it sells. Google's built-in harm filters default to off on its newest Gemini models, and Model Armor is off until you set it up. Amazon's Bedrock Guardrails checks nothing until you attach one, and inline it skips tool calls and their results. None of them knows your business rules, such as which customer may see which order, so that stays your job.

**Sources**
- AWS, [Amazon Bedrock Guardrails](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails.html) and its [Converse API notes on tool use](https://docs.aws.amazon.com/bedrock/latest/userguide/guardrails-use-converse-api.html). [SELF]
- Microsoft Learn, [Foundry default safety policies](https://learn.microsoft.com/en-us/azure/foundry/guardrails/default-safety-policies) (Oct 2026). [SELF]
- Google Cloud, [Model Armor overview](https://docs.cloud.google.com/security-command-center/docs/model-armor-overview) and [Gemini safety filters](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/multimodal/configure-safety-filters) (Oct 2026). [SELF]

### 7:12 · Limit what it can do

> Limit what it can do.
>
> Least access · a person approves · stop and ask

**What this is getting at.** Because guardrails will miss things, the guidance now is to limit what the system can do. The Five Eyes agencies call least privilege critical, leave the decision about when a human must approve to the system's designers and operators, and want systems set "to fail-safe by default requiring agents to stop and escalate issues to human reviewers in uncertain scenarios." The UK NCSC says protections should focus more on deterministic, non-AI safeguards that constrain what the system can do, rather than just trying to keep malicious content away from the model. In the film, the agent's courier is held at the bank's bollards, a car with the right key is let into the records drive, and a hold lamp waits on a decision.

**Sources**
- [Five Eyes](https://www.ncsc.govt.nz/assets/guidance/Documents/Careful-adoption-of-agentic-AI-services_FINAL.pdf) (May 2026), pp. 20 and 22. [GOV]
- [UK NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection) (Dec 8, 2025). [GOV]
- [UK NCSC blog, "Thinking carefully before adopting agentic AI"](https://www.ncsc.gov.uk/blogs/thinking-carefully-before-adopting-agentic-ai) (May 15, 2026). [GOV]

### 7:29 · Keep revisiting

> Keep revisiting where you check, when, and what happens on a no.

The series' view, as the toll plaza's booths answer one by one. NIST, Microsoft and OWASP all describe threat modelling as ongoing work (5:31).

## Further reading

None of these is in the film.
- **A design that contains injection.** CaMeL plans a task from the trusted request and tracks where each piece of data came from, so injected text can't change the plan. It solved 77% of a benchmark's tasks with provable security, against 84% with no defense. [Debenedetti et al., arXiv 2503.18813](https://arxiv.org/abs/2503.18813) (Mar 2025)
- **Meta's "Rule of Two."** In one session, an agent should have no more than two of three properties, which are reading untrusted input, reaching sensitive systems or data, and changing state or communicating out. [Meta AI](https://ai.meta.com/blog/practical-ai-agent-security/) (Oct 31, 2025) [SELF]
- **Guardrails as layers, from a model maker.** OpenAI's guide treats guardrails as a layered defense and rates each tool's risk to decide where extra checks or a human go. [A practical guide to building agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf) (Apr 2025) [SELF]
- **The cost keeps rising.** Anthropic's next-generation classifiers add about 1% compute, and 1,700+ hours of red-teaming found no universal jailbreak. [Anthropic](https://www.anthropic.com/research/next-generation-constitutional-classifiers) (Jan 9, 2026) [SELF]

## About this page
- **When checked.** The research was read on Oct 19 and 20, 2026, and every link was re-checked on Oct 23, 2026. Some sites, including openai.com, TIME and the INFORMS journal site, refuse automated checks.
- **Timestamps.** For the 7:44 cut. Quoted lines are the on-screen captions. The narrator tells the same facts in his own words.
- **Labels.** [SELF] marks an organization describing its own work, product, data or incident. [VENDOR] marks a company that sells related security or AI products. [PRESS] is news coverage. [GOV], [LAW], [STANDARD] and [ACADEMIC] mark government guidance, law, standards bodies and peer-reviewed research. Preprints are labelled in the text. None of these is independent confirmation by itself.
- **What's real.** The highway, the crash-test cars, the trucks, the courier, the toll plaza, the AI agent character and the x-ray diagrams are illustrations, and no real people are shown apart from Pliny's public X profile. The crash test follows the MASH standard. The incidents and numbers are real.
- **The series' view.** "AI has guardrails too… just as easy to misunderstand", "Worth running anyway", the comparison with firewalls and antivirus, and "Keep revisiting where you check…" are opinion.
- **Honest limits.** Most incident accounts here come from the companies involved. The adaptive-attack results assume a strong attacker who can see the detectors' scores. The timing numbers come from different setups and shouldn't be compared as if one lab measured them all.
- **Left out on purpose.** A "3,000 attempts" figure for the $1 SUV, which isn't in the original report. A widely repeated download count for the rogue Cline release, which isn't in Cline's advisory. "Over 1,200 agents" in the Hugging Face incident, which neither company's disclosures give. Colorado's "reasonable care" AI duty, replaced before it took effect.
- **Licence.** Quotes from NCSC and UK AI Security Institute pages contain public sector information licensed under the Open Government Licence v3.0. OWASP material is CC BY-SA 4.0.
- **Corrections.** Welcome as a GitHub issue.
