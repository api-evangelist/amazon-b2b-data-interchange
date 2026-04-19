# Amazon B2B Data Interchange

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
