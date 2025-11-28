# Event Context
This is an exploratory proof of concept to explore what and end-to-end use case for Cvent could look like--assembling all the existing standards in a single place to help inform what the capability schema might look like to support our pilot customers use case, while providing governance along the way.

## Use Case
This is an applicaiton of the AI Context use cases for Cvent or pilot customer, leveraging the use case schema being developed to drive use case conversations, as well as how they are applied to each individual capability.

- [AI Context](use-case/ai-context.yml) - Using a capability as the context window for producing MCP servers.

## Capabilities
This end-to-end use cases has six separate capabilities, providing five individual capabilities that can be applied individually, as well as an aggregate capability that brings them all together to provide the right-size context window for an MCP server.

- [Events (Aggregate)](capability-event-context.yml) - A single aggregate events capability.
- [Events](capability-event-context-events.yml) - An individual events capability.
- [Atendees](capability-event-context-attendees.yml) - An individual attendees capability.
- [Exhibitors](capability-event-context-exhibitors.yml) - An individual exhibitors capability.
- [Sessions](capability-event-context-sessions.yml) - An individual sessions capability.
- [Speakers](capability-event-context-speakers.yml) - An individual speakers capability.

## Image
This is an image of this aggregate events AI context capability to try and capture everything going on in the visual language we already use for our deck.

![Alt text](diagrams/event-ai-context-engine.png "Event AI Context Capability")

## Folders
This repository is currently broken down into the following folders that help support references made within each capability, providing different layers of the capabilities using existing standards that our customers are using.

- api-commons - Using two API commons schema for plans and rate limits.
- arazzo - Using Arazzo for the oauth workflows and eventually events.
- bruno - Every HTTP adapter is setup and tested using Bruno client.
- diagrams - Produced a diagram to help illustrate how capability works.
- json-schema - Localizing all the JSON schema needed to validate.
- model-context-protocol - Generating MCP servers from each OpenAPI.
- openapi - Providing all of the OpenAPI needed for each HTTP adapter.
- spectral - Providing all of the rules used to gover the capabilities.
- use-case - The use case being applied as part of this aggregate capability.

## Schemas
All of the JSON Schema are stored locally in this folder for development and learning purposes, but all schema are centralized via the schema repository to ensure their reuse across each of the capabilities and use cases being developed as part of this work.

## Changes
I am rapidly iterating upon this set of capabilities as part of ongoing Cvent conversations, helping evolve and strengthen our AI Context use case. To help capture the changes I will try to do bulk updates via commits and PRs, but will wrap with an issue for logging purposes.

- [AI Context Change Log #1](https://github.com/naftiko-capabilities/event-context/issues/1)

## Contributions
I need your feedback. Please leave via [issues](https://github.com/naftiko-capabilities/event-context/issues) or in [Slack](https://naftiko.slack.com/archives/C09LLFZDLL9), but also don't hesitate submitting pull requests to fix any problems encountered and leave feedback to help contribute to this work as it happening.