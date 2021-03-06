[@heggert](https://github.com/heggert)
[@SvenHoeffler](https://github.com/SvenHoeffler)
[@jkopen](https://github.com/jkopen)
[@weberjm](https://github.com/weberjm)
[@IoannisLafiotis](https://github.com/IoannisLafiotis)
[@RobinBrinkmann](https://github.com/RobinBrinkmann)

# IssueList

### General Concepts

- Introduction to the framework to lay out basics and link important docs: [@RobinBrinkmann](https://github.com/RobinBrinkmann)
  - What it is: Framework, async flows etc, OS Community
  - TechStack / Common Tooling: node, rabbit, mongo, GCP etc
  - Common scenarios / Service compositions: H&S and/or Flows
  - Link to general concepts (flows, connectors, exection/service collab) and SetupGuides
- Service Collaboration Rework [@heggert](https://github.com/heggert)
  - whole execution flow with orchestrator / ferryman / queues / iam etc
  - probably rewrite: https://github.com/openintegrationhub/openintegrationhub.github.io/blob/master/docs/Service%20Collaboration/ServiceCollaborationOverview.md
- explanation of a flow (also on oih.org) [@SvenHoeffler](https://github.com/SvenHoeffler)
- rework connector intro [@IoannisLafiotis](https://github.com/IoannisLafiotis), [@SvenHoeffler](https://github.com/SvenHoeffler)
  - new terminology: component -> connector -> adapter & transformer (optional / outdated)
  - add eio + flowground for connector source
  - old connectors checklists (still linked? remove/rewrite)

### Deployment & Dev Process

- deployment / use of docker images (latest is not recommended, use release etc), our approach to versioning [@weberjm](https://github.com/weberjm)
- minimum resource requirements: https://github.com/openintegrationhub/openintegrationhub/issues/1002
- GCP Guide Helthcheck Behavior: https://github.com/openintegrationhub/openintegrationhub/issues/1125 [@weberjm](https://github.com/weberjm)
- Rewrite / Update Contributions Guidelines
  - create new Issue templates
  - how do we consider input and what do we expect in a PR
- check + update local + GCP installation guide [@SvenHoeffler](https://github.com/SvenHoeffler)

### Services (on github.io site + monorepo)

- workflow repo (minimum: mark as draft)
- rules engine (minimum: mark as draft)
- raw data missing (not yet released - cover later)
- data merge missing (not yet released - cover later)
- governance service missing [@jkopen](https://github.com/jkopen)
- template repository missing [@weberjm](https://github.com/weberjm)
- AppDirectory missing
- logging service (has been removed form monorepo)
- Ferryman docs missing (not a "service", but should be listed there?) [@jkopen](https://github.com/jkopen)
- Information for service deployment requirements per scenario above (i.e. <H&S: required> <core: optional>)
- Still up-to-date? / Need to be checked:
  - IAM
  - Secret Service
  - Comp Orchestrator
  - Comp Repository
  - Flow Repository
  - Data Hub

### Housekeeping & Structure

- improve README on monorepo to point to more dev resources right away and get a better overview / starting point [@heggert](https://github.com/heggert)
- cross-check monorepo and github.io
  - same / all services?
  - Link github.io conceptual services descriptions in monorepo readme per service
  - check links from github.io to monorepo
- describe how to use the docs (i.e. service readme in monorepo vs github.io docs)

### Decisions

- remove "workgroup" section in repos such as connectors, data models etc?
- remove old components (i.e. salesforce)
- do we still need all files in connector docu (i.e. checklist?)
- do we still need a seperate connectors repo (was supposed to be for workgroup and docs: workgroup doesnt exist and docs are somewhere else)
