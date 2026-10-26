# Amazon B2B Data Interchange

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

AWS B2B Data Interchange is a fully managed service that automates the transformation and exchange of electronic data interchange (EDI) documents at cloud scale. It enables businesses to onboard trading partners, transform X12 EDI documents to and from JSON or XML, and manage capabilities, profiles, and partnerships with pay-as-you-go pricing.

The service supports supply chain, healthcare, and financial services workflows and leverages Amazon Bedrock for AI-assisted mapping generation.

**Human URL:** [https://aws.amazon.com/b2b-data-interchange/](https://aws.amazon.com/b2b-data-interchange/)

**API Reference:** [https://docs.aws.amazon.com/b2bi/latest/APIReference/api-welcome.html](https://docs.aws.amazon.com/b2bi/latest/APIReference/api-welcome.html)

## APIs

### AWS B2B Data Interchange API

The AWS B2B Data Interchange API provides programmatic access to manage EDI transformation workflows, trading partner profiles, capabilities, partnerships, and transformers. It enables creation and management of inbound and outbound EDI pipelines using X12 standards and supports AI-assisted mapping template generation via Amazon Bedrock.

**Base URL:** `https://b2bi.us-east-1.amazonaws.com`

#### Key Operations

| Operation | Description |
|---|---|
| CreateProfile | Create an EDI sender/receiver profile |
| CreatePartnership | Connect a profile with a trading partner |
| CreateCapability | Define an EDI transformation pipeline |
| CreateTransformer | Build an EDI transformer with mapping template |
| StartTransformerJob | Execute an asynchronous EDI transformation job |
| GenerateMapping | Use Amazon Bedrock to auto-generate mapping templates |
| TestMapping | Validate mapping templates against sample data |
| TestParsing | Parse and validate EDI files |
| TestConversion | Test EDI document conversions end-to-end |

## Features

- **EDI Transformation** — Transform X12 EDI documents to JSON or XML and generate EDI from JSON/XML inputs
- **AI-Assisted Mapping** — Use Amazon Bedrock to automatically generate mapping templates, reducing mapping development time by up to 50%
- **Trading Partner Management** — Onboard and manage trading partners through profiles, capabilities, and partnerships
- **EDI Splitting** — Split inbound X12 EDI documents into individually processed single-transaction documents, supporting files up to 5GB
- **HIPAA Compliance** — Secure exchange of protected health information for healthcare EDI workflows

## Use Cases

- **Supply Chain Partner Onboarding** — Automate onboarding of trading partners without custom EDI development
- **Healthcare Claims Processing** — Streamline healthcare enrollment and claims with X12 EDI and HIPAA compliance
- **Financial Transaction Processing** — Expedite financial transactions through automated EDI transformation

## Integrations

- AWS Transfer Family
- Amazon S3
- Amazon EventBridge
- Amazon Bedrock

## Artifacts

| Type | URL |
|---|---|
| OpenAPI Spec | [openapi/aws-b2b-data-interchange-api-openapi.yml](openapi/aws-b2b-data-interchange-api-openapi.yml) |
| JSON Schema (Profile) | [json-schema/profile.json](json-schema/profile.json) |
| JSON Schema (Partnership) | [json-schema/partnership.json](json-schema/partnership.json) |
| JSON Schema (Transformer) | [json-schema/transformer.json](json-schema/transformer.json) |
| JSON Structure | [json-structure/b2bi-resource-structure.json](json-structure/b2bi-resource-structure.json) |
| JSON-LD Context | [json-ld/context.jsonld](json-ld/context.jsonld) |
| Spectral Ruleset | [spectral/ruleset.yml](spectral/ruleset.yml) |
| Capabilities | [capabilities/capabilities.yml](capabilities/capabilities.yml) |
| Vocabulary | [vocabulary/vocabulary.yml](vocabulary/vocabulary.yml) |
| Examples | [examples/](examples/) |

## Common Properties

| Type | URL |
|---|---|
| CLI Reference | [https://docs.aws.amazon.com/cli/latest/reference/b2bi/](https://docs.aws.amazon.com/cli/latest/reference/b2bi/) |
| JavaScript SDK | [https://github.com/aws/aws-sdk-js-v3/tree/main/clients/client-b2bi](https://github.com/aws/aws-sdk-js-v3/tree/main/clients/client-b2bi) |
| Go SDK | [https://pkg.go.dev/github.com/aws/aws-sdk-go-v2/service/b2bi](https://pkg.go.dev/github.com/aws/aws-sdk-go-v2/service/b2bi) |
| Rust SDK | [https://docs.rs/aws-sdk-b2bi](https://docs.rs/aws-sdk-b2bi) |
| Samples | [https://github.com/aws-samples/aws-b2b-data-interchange-toolkit](https://github.com/aws-samples/aws-b2b-data-interchange-toolkit) |
| CloudFormation | [https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/AWS_B2BI.html](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/AWS_B2BI.html) |
| Pricing | [https://aws.amazon.com/b2b-data-interchange/pricing/](https://aws.amazon.com/b2b-data-interchange/pricing/) |

## Maintainers

**Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com)
