# Policytide

[User guide](USER_GUIDE.md)

## What it is

Policytide is an independent UK politics web app that brings policy developments, 2024 election promises and a personal finance illustration into one place. Its goal is to make complex policy information easier to explore, understand and relate to your own circumstances, without telling you which party to support.

This public repository contains the **project overview and user guide only**. The application source and editorial research workflows are kept in a separate private repository. Policytide is currently a curated prototype, not a live or exhaustive political information service.

## Key features

- **Personalised overview:** relevant policy updates and manifesto promises appear nearer the top based on the topics and circumstances you choose.
- **What's changing:** selected policy developments with dates, stages, applicable UK nations and linked sources.
- **Party promises:** 32 selected Labour 2024 commitments with evidence, timelines and dated progress judgements, alongside historical manifesto material from six other parties.
- **Explore and compare:** search or filter commitments and compare two parties' 2024 proposals by policy topic.
- **Your finances:** illustrate how employment income tax, employee National Insurance, supported student loans and optional salary sacrifice might affect annual and average monthly take-home pay in 2026/27 and 2027/28.
- **No account needed:** your interests and circumstances are saved in your browser and can be changed or cleared.

The Labour assessments are dated editorial judgements, **not live or independently audited fact-checks**. The 26 assessments published on 21 November 2026 used AI-assisted source research and were not separately independently fact-checked. Opposition comparisons describe **2024 manifesto positions**, which may not reflect current party positions. The app does not calculate a political compatibility score.

## Tech stack

| Area | Technology |
| --- | --- |
| Interface | HTML, CSS and vanilla JavaScript |
| Design | Editorial layouts, responsive CSS, Archivo and IBM Plex typography |
| Data | Curated JavaScript policy and manifesto records with dated source links |
| Personalisation | Explainable rule-based matching and browser localStorage |
| Finance illustration | Client-side tax, National Insurance and loan calculations |
| Monitoring | Node.js, selected official UK data sources and GitHub Actions for editorial research |
| Hosting | Static app deployment on Vercel |
| Quality checks | Automated JavaScript and browser regression tests |

There is no account system, application database or frontend framework. The monitors help researchers find potential changes, but they cannot publish new political judgements automatically.

## Technical decisions and trade-offs

| Decision | Reason | Trade-off |
| --- | --- | --- |
| Keep policy records curated and sourced | Readers can inspect dates and evidence behind a claim. | The service covers selected topics and needs editorial updates. |
| Use transparent relevance rules | People can see why a policy was brought to their attention. | Relevance cannot capture the full impact of a policy on someone's life. |
| Treat opposition manifestos as historical | Avoids suggesting that parties outside government failed to implement pledges. | The 2024 comparison is not a guide to each party's current position. |
| Store profiles locally | Browsing does not require registration. | Preferences are specific to a browser and do not sync across devices. |
| Limit the finance illustration | The scope and assumptions remain visible. | It is not a full household Budget impact calculator or a substitute for personalised advice. |
| Keep monitoring separate from publication | A source change is not automatically proof of a policy outcome. | Human verification and periodic reviews are still needed. |

## Sources, privacy and limitations

Policytide points readers to original policy announcements, manifesto documents, official UK tax guidance and independent analysis where relevant. It draws on sources such as [UK Parliament](https://www.parliament.uk/), [GOV.UK](https://www.gov.uk/), [Labour's 2024 manifesto](https://labour.org.uk/updates/stories/labour-manifesto-2024-sign-up/) and [Full Fact](https://fullfact.org/government-tracker/).

Personalisation is kept in the browser. The prototype has no user accounts or app analytics. The calculator covers defined employment and loan scenarios, not every UK tax rule or personal circumstance. Please verify official sources and their dates before making decisions.

For instructions on using each section, read the [user guide](USER_GUIDE.md).
