# Designing resilient cloud applications

## Description

Building a resilient application means leaning on the distributed nature of the cloud. In this talk, we’ll
show you how Tailwind Traders reduced single point of failure by deploying backend services to multiple
regions using Azure App Service and Azure Traffic Manager. We’ll then create a CDN using Azure Blob
Storage to deliver static assets such as images and frontend code. Finally, we’ll deploy our data with
full geo-redundancy using Cosmos DB and Azure SQL Database.

Once we’ve set everything up, we’ll test it out and see how our application handles, and recovers
from, catastrophic failure.

Speaker: Brian Hold

## Content

Credential Management

- Growing Structure in Developers

- Keys Included in Code

- Gets Distributed to more and more People

Move to KeyVault

- Multiple KeyVaults (Dev, Q, Prod)

### Azure Key Vault

- Manage all Secrets in one Place

- Seamlessly move between dev, QA, and prod enviroments

- Update your Credentials in one Spot

- Version Credentials/Rollback

- Add a credential and all devs have instantly access

- Secure

#### Dont you need Credentials to access the Key Vault

- Enable MSI on your VM, App Service, or function

- when those production enviroments are spun up, they are given a local endpoint to request to get credentials

- you dont have to inject those variables, those already have

### Cosmodb

- Has common Adapters/Multi Paradigm (Mongo, Sql, Casandra, etc..)

- Connect to Apache Spark

- Infinitely scaling

- Fully managed sharding, replica, etc

Connection String will find the lowest latency datacenter over the world

easy to connect VS Code to Azure and CosmosDb

### Azure App Service

- Runs your Code in the Cloud

- Scales up and scales out your app as necessary

- fokus on what makes your business unique

easy to connect VS code to App Services

### Azure Storage

- anything static you need to store in the cloud

- A few way of storing data
  - Blob
  - Disk
  - Table
  - Files
  - Queues

- Add CDN

### Azure Static Sites

- Currently in Preview

- Static Website, to serve your website from a web server that are contained in blob

- Attaches proper MIME types!

- Stick files in "$web$ directory

### Azure FrontDoor

- Distribute Services globally

- automatically spin up/spin down regions

- app connetcts to front door and will be routed to the best/nearest backend service

- currently preview

- simple to setup

- allow you to seamlessly
  - spin up/spin down

- fails over automatically
  - Region/instance Failure, switch over to other Region

### Multi Master CosmosDb

- Every Region can be written to

- makes writing much quicker affair

- seamlessly spin up/down new regions

## Links

Usefull links

#### Microsoft Learn

aka.ms/learn-dev10

#### Microsoft Docs

aka.ms/docs-dev10