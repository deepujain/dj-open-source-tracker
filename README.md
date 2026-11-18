# Warp Speed

Warp Speed is a team of AI agents that carries open-source work from an open
issue to a merged pull request. No single agent does everything. Each agent
owns one stage, the way people on an engineering team do, and hands its work to
the next agent.

Every contribution starts with the **Triage agent**. It reads a project's open
issues, sets aside the ones someone else has claimed or that fall outside the
project's contribution rules, and picks the ones worth solving.

The **Research agent** then studies each issue the way a new teammate would:
the code paths involved, the project's contributing guide, and what reviewers
asked for on earlier pull requests. It hands the Build agent a plan, not a
guess.

The **Build agent** writes the change and its tests in an isolated checkout, so
many issues move forward side by side without stepping on each other. Before
anything leaves the machine, the **Review agent** checks the commit against the
same gates the project runs in CI. A change that fails goes back to the Build
agent, not to the project's reviewers.

Once the pull request is open, the **Repair agent** owns it. When a hosted check
fails, the Repair agent reads the log, reproduces the failure and pushes one
focused fix. The **Testing agent** runs the project's end-to-end suites on that
exact commit and keeps the evidence.

The **Nudge agent** watches over all of them. It reads every open pull request
on a schedule, and when one stalls, it wakes the agent that owns the next step.
The **Learn agent** closes the loop: every review outcome, merged or not,
becomes a rule the other agents follow on their next run, so each project gets
easier to contribute to over time.

Together these agents work dozens of pull requests across many projects at
once, each one racing to ready for review with every check green.

![Warp Speed dashboard: pull requests landed, opened and ready for review](assets/warp-speed-dashboard-hd.png)

## Warp Speed-Assisted Contributions

These contributions were assisted by Warp Speed.

| Project | Contributions | Open | Merged | Merged % |
|--------------|---------------|------|--------|----------|
| <a href="https://github.com/apache/airflow"><img src="https://apache.org/logos/res/airflow/default.png" alt="Apache Airflow logo" height="18"></a> <a href="https://github.com/apache/airflow">Apache Airflow</a> | [37](https://github.com/apache/airflow/pulls/deepujain) | 1 | 14 | 37.8% |
| <a href="https://github.com/apache/hadoop"><img src="https://apache.org/logos/res/hadoop/hadoop.png" alt="Apache Hadoop logo" height="18"></a> <a href="https://github.com/apache/hadoop">Apache Hadoop</a> | [15](https://github.com/apache/hadoop/pulls/deepujain) | 3 | 5 | 33.3% |
| <a href="https://github.com/apache/spark"><img src="https://apache.org/logos/res/spark/spark.png" alt="Apache Spark logo" height="18"></a> <a href="https://github.com/apache/spark">Apache Spark</a> | [7](https://github.com/apache/spark/pulls/deepujain) | 0 | 4 | 57.1% |
| <a href="https://github.com/apache/superset"><img src="https://apache.org/logos/res/superset/default.png" alt="Apache Superset logo" height="18"></a> <a href="https://github.com/apache/superset">Apache Superset</a> | [12](https://github.com/apache/superset/pulls/deepujain) | 2 | 10 | 83.3% |
| <a href="https://github.com/brevdev/brev-cli"><img src="https://avatars.githubusercontent.com/u/70683657?v=4" alt="Brev logo" height="18"></a> <a href="https://github.com/brevdev/brev-cli">Brev CLI</a> | [2](https://github.com/brevdev/brev-cli/pulls/deepujain) | 0 | 2 | 100.0% |
| <a href="https://github.com/openclaw/clawhub"><img src="https://raw.githubusercontent.com/openclaw/clawhub/main/public/logo192.png" alt="ClawHub logo" height="18"></a> <a href="https://github.com/openclaw/clawhub">ClawHub</a> | [26](https://github.com/openclaw/clawhub/pulls/deepujain) | 1 | 12 | 46.2% |
| <a href="https://github.com/kubernetes-sigs/gateway-api"><img src="https://avatars.githubusercontent.com/u/36015203?v=4" alt="Kubernetes SIGs logo" height="18"></a> <a href="https://github.com/kubernetes-sigs/gateway-api">Gateway API</a> | [2](https://github.com/kubernetes-sigs/gateway-api/pulls/deepujain) | 1 | 1 | 50.0% |
| <a href="https://github.com/NousResearch/hermes-agent"><img src="https://raw.githubusercontent.com/NousResearch/hermes-agent/main/website/static/img/logo.png" alt="Hermes Agent logo" height="18"></a> <a href="https://github.com/NousResearch/hermes-agent">Hermes Agent</a> | [16](https://github.com/NousResearch/hermes-agent/pulls/deepujain) | 5 | 1 | 6.2% |
| <a href="https://github.com/UKGovernmentBEIS/inspect_ai"><img src="https://raw.githubusercontent.com/UKGovernmentBEIS/inspect_ai/main/docs/images/aisi-logo.svg" alt="AISI logo" height="18"></a> <a href="https://github.com/UKGovernmentBEIS/inspect_ai">Inspect AI</a> | [39](https://github.com/UKGovernmentBEIS/inspect_ai/pulls/deepujain) | 3 | 20 | 51.3% |
| <a href="https://github.com/meridianlabs-ai/inspect_petri"><img src="https://raw.githubusercontent.com/meridianlabs-ai/inspect_petri/main/docs/images/petri.svg" alt="Inspect Petri logo" height="18"></a> <a href="https://github.com/meridianlabs-ai/inspect_petri">Inspect Petri</a> | [7](https://github.com/meridianlabs-ai/inspect_petri/pulls/deepujain) | 1 | 2 | 28.6% |
| <a href="https://github.com/Leaflet/Leaflet"><img src="https://avatars.githubusercontent.com/u/2854298?v=4" alt="Leaflet logo" height="18"></a> <a href="https://github.com/Leaflet/Leaflet">Leaflet</a> | [6](https://github.com/Leaflet/Leaflet/pulls/deepujain) | 0 | 1 | 16.7% |
| <a href="https://github.com/NVIDIA/NemoClaw"><img src="https://raw.githubusercontent.com/NVIDIA/NemoClaw/main/fern/assets/NVIDIA_symbol.svg" alt="NemoClaw logo" height="18"></a> <a href="https://github.com/NVIDIA/NemoClaw">NemoClaw</a> | [227](https://github.com/NVIDIA/NemoClaw/pulls/deepujain) | 10 | 155 | 68.3% |
| <a href="https://github.com/NVIDIA/NeMo-Agent-Toolkit"><img src="https://avatars.githubusercontent.com/u/1728152?v=4" alt="NVIDIA logo" height="18"></a> <a href="https://github.com/NVIDIA/NeMo-Agent-Toolkit">NVIDIA NeMo Agent Toolkit</a> | [3](https://github.com/NVIDIA/NeMo-Agent-Toolkit/pulls/deepujain) | 0 | 2 | 66.7% |
| <a href="https://github.com/openclaw/openclaw"><img src="https://raw.githubusercontent.com/openclaw/openclaw/main/ui/public/favicon.svg" alt="OpenClaw logo" height="18"></a> <a href="https://github.com/openclaw/openclaw">OpenClaw</a> | [36](https://github.com/openclaw/openclaw/pulls/deepujain) | 4 | 6 | 16.7% |
| <a href="https://github.com/pytorch/pytorch"><img src="https://raw.githubusercontent.com/pytorch/pytorch/main/docs/source/_static/img/pytorch-logo-flame.svg" alt="PyTorch logo" height="18"></a> <a href="https://github.com/pytorch/pytorch">PyTorch</a> | [42](https://github.com/pytorch/pytorch/pulls/deepujain) | 19 | 6 | 14.3% |
| <a href="https://github.com/NVIDIA/SkillEvaluator"><img src="https://avatars.githubusercontent.com/u/1728152?v=4" alt="NVIDIA logo" height="18"></a> <a href="https://github.com/NVIDIA/SkillEvaluator">SkillEvaluator</a> | [5](https://github.com/NVIDIA/SkillEvaluator/pulls/deepujain) | 0 | 5 | 100.0% |
| <a href="https://github.com/NVIDIA/SkillSpector"><img src="https://avatars.githubusercontent.com/u/1728152?v=4" alt="NVIDIA logo" height="18"></a> <a href="https://github.com/NVIDIA/SkillSpector">SkillSpector</a> | [31](https://github.com/NVIDIA/SkillSpector/pulls/deepujain) | 0 | 29 | 93.5% |
| <a href="https://github.com/NVIDIA-NeMo/Switchyard"><img src="https://avatars.githubusercontent.com/u/1728152?v=4" alt="NVIDIA logo" height="18"></a> <a href="https://github.com/NVIDIA-NeMo/Switchyard">Switchyard</a> | [10](https://github.com/NVIDIA-NeMo/Switchyard/pulls/deepujain) | 0 | 5 | 50.0% |
| <a href="https://github.com/meridianlabs-ai/ts-mono"><img src="https://avatars.githubusercontent.com/u/196480008?v=4" alt="Meridian Labs logo" height="18"></a> <a href="https://github.com/meridianlabs-ai/ts-mono">ts-mono</a> | [20](https://github.com/meridianlabs-ai/ts-mono/pulls/deepujain) | 0 | 16 | 80.0% |
| **Total Contributions** | **543** | **50** | **296** | **54.5%** |

**Total Contributions:** 543

**Success Rate:** 54.5% merged (296 of 543)

## Bootstrapping Projects

These projects are in their initial contribution phase and do not yet have a
merged contribution.

| Project | Contributions | Open | Merged |
| --- | ---: | ---: | ---: |
| <a href="https://github.com/NVIDIA-AI-Blueprints/deep-researcher-agent"><img src="https://avatars.githubusercontent.com/u/1728152?v=4" alt="NVIDIA logo" height="18"></a> <a href="https://github.com/NVIDIA-AI-Blueprints/deep-researcher-agent">Deep Researcher Agent (AIQ)</a> | [3](https://github.com/NVIDIA-AI-Blueprints/deep-researcher-agent/pulls/deepujain) | 1 | 0 |
| <a href="https://github.com/kubernetes/kubernetes"><img src="https://raw.githubusercontent.com/kubernetes/kubernetes/master/logo/logo.png" alt="Kubernetes logo" height="18"></a> <a href="https://github.com/kubernetes/kubernetes">Kubernetes</a> | [2](https://github.com/kubernetes/kubernetes/pulls/deepujain) | 2 | 0 |
| <a href="https://github.com/NVIDIA/Megatron-LM"><img src="https://avatars.githubusercontent.com/u/1728152?v=4" alt="NVIDIA logo" height="18"></a> <a href="https://github.com/NVIDIA/Megatron-LM">Megatron-LM</a> | [7](https://github.com/NVIDIA/Megatron-LM/pulls/deepujain) | 4 | 0 |
| <a href="https://github.com/NVIDIA/OpenShell"><img src="https://raw.githubusercontent.com/NVIDIA/OpenShell/main/docs/brand/assets/favicon.svg" alt="OpenShell logo" height="18"></a> <a href="https://github.com/NVIDIA/OpenShell">OpenShell</a> | [1](https://github.com/NVIDIA/OpenShell/pulls/deepujain) | 0 | 0 |
| <a href="https://rea.tools"><img src="https://avatars.githubusercontent.com/u/76467478?v=4" alt="REA logo" height="18"></a> <a href="https://github.com/morluto/rea">REA</a> | [3](https://github.com/morluto/rea/pulls/deepujain) | 3 | 0 |
| <a href="https://www.schedmd.com/"><img src="https://raw.githubusercontent.com/SchedMD/slurm/master/doc/html/slurm_logo.png" alt="Slurm logo" height="18"></a> <a href="https://www.schedmd.com/">Slurm</a> | [3](https://support.schedmd.com/buglist.cgi?email3=deepujain%40gmail.com&emaillongdesc3=1&emailtype3=substring&list_id=418332&product=Slurm&query_format=advanced&resolution=---) | 3 | 0 |

## Non-Warp Speed Contributions

These contributions were not assisted by Warp Speed.

| Project | Contributions | Open | Merged | Merged % |
|--------------|---------------|------|--------|----------|
| <a href="https://github.com/apache/avro"><img src="https://apache.org/logos/res/avro/default.png" alt="Apache Avro logo" height="18"></a> <a href="https://github.com/apache/avro">Apache Avro</a> | [1](https://issues.apache.org/jira/browse/AVRO-1419) | 1 | 0 | 0.0% |
| <a href="https://github.com/apache/druid"><img src="https://apache.org/logos/res/druid/default.png" alt="Apache Druid logo" height="18"></a> <a href="https://github.com/apache/druid">Apache Druid</a> | [1](https://github.com/apache/druid/pulls/deepujain) | 0 | 1 | 100.0% |
| <a href="https://github.com/elastic/beats"><img src="https://avatars.githubusercontent.com/u/6764390?v=4" alt="Elastic logo" height="18"></a> <a href="https://github.com/elastic/beats">Elastic Beats</a> | [2](https://github.com/elastic/beats/pulls/deepujain) | 0 | 2 | 100.0% |
| <a href="https://github.com/eBay/oink"><img src="https://avatars.githubusercontent.com/u/3639281?v=4" alt="eBay Open Source logo" height="18"></a> <a href="https://github.com/eBay/oink">eBay Oink</a> | [1](https://github.com/eBay/oink/pulls/deepujain) | 0 | 1 | 100.0% |
| <a href="https://github.com/eBay/nvidiagpubeat"><img src="https://avatars.githubusercontent.com/u/3639281?v=4" alt="eBay Open Source logo" height="18"></a> <a href="https://github.com/eBay/nvidiagpubeat">nvidiagpubeat</a> | Creator and maintainer | — | — | — |
| <a href="https://github.com/apache/pig"><img src="https://apache.org/logos/res/pig/default.png" alt="Apache Pig logo" height="18"></a> <a href="https://github.com/apache/pig">Apache Pig</a> | [2](https://issues.apache.org/jira/issues/?jql=key%20in%20(PIG-1885%2C%20PIG-671)) | 0 | 2 | 100.0% |
| <a href="https://github.com/apache/zeppelin"><img src="https://zeppelin.apache.org/assets/themes/zeppelin/img/zepLogo.png" alt="Apache Zeppelin logo" height="18"></a> <a href="https://github.com/apache/zeppelin">Apache Zeppelin</a> | [6](https://github.com/apache/zeppelin/pulls/deepujain) | 0 | 0 | 0.0% |
| <a href="https://github.com/NICTA/scoobi"><img src="https://avatars.githubusercontent.com/u/1151968?v=4" alt="Scoobi logo" height="18"></a> <a href="https://github.com/NICTA/scoobi">Scoobi</a> | [2](https://github.com/NICTA/scoobi/pulls/deepujain) | 0 | 0 | 0.0% |
| **Total Contributions** | **15** | **1** | **6** | **40.0%** |

## Reusable Skill

This repo also includes a reusable
[OSS Contribution README skill](skills/oss-contribution-readme/SKILL.md) for
creating README files like this one.

Use it to build a polished OSS contribution showcase with verified GitHub PR
counts, tracker patch submissions, official project logos, linked totals,
featured contribution tables, and screenshot-friendly formatting.
