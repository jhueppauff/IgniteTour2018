# Modernize your infrastructure moving to Infrastructure as Code

## Where we come from

- Transactional sytems administrators (ticket-based workflows)
  - Queue Based Workloads
  - Siloed responsibilities (esp. developer and operations)
- NOC's
- GUI based systems administrators
  - Handover is difficult (repeatable process), documentations
- "Big" releases at the end of the waterfall
- linear scaling (touch every mashine)

## Welcome to the cloud

### From Ops perspective

- provisioning and expantion done form API not PO
- decomissioning can be done from API not datacenter ticket
- connectivity can be managed from api, not a network group ticket
- applications can be deployed from api, not a word document

#### What we get

- repeatability
- velocity
- scalability
- self service
- infrastructure as code

#### How does our Operations deliver Business Value

- features and capabilities are great but they are not business value

## Dev Ops

- Definition and practices can help narrow in on DevOps

## Site Reliability Engineerung (SRE)

- Reliability
  - What matters is the service delivered (Infrastructure does not matter if the applications aren't reliability)
- Appropriate
- Sustainably

### Toil

- manual
- repetitive
- automatable
- tactical
- devoid

## Automation (DevOps/SRE)

- the only way that we can reliably deploy complex infrastrucutre and applications is to automate the proces

- code has some nice properties
  - reusability
  - source control management
  - searchability

## CI/CD

- CI
  - trunk based development
  - integrate development work into releasable from serveral times + test
- CDelivery
  - further tooling to allow release to be allow release to be deployed via automation
- continous deployment
  - if releas paases muster

### Importance

- Fewer bugs introduced
- smaller bugs, faster fixes
- reduced risk
- fast landing of freatures, easier experimentation
- faster feedback from production
- lighter weight process
- better for operations staff (no huge releases)

#### Importance of automated delivery

- repro builds
- automated testing
- more frequent releases
- less risk

## Further possible directions for infra/app deployment

- bring infra as code alongside the application code
  - same repository as the code
- Containers
  - Orchestration
- serverless 