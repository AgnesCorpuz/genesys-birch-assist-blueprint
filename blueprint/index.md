# Birch Assist

BirchAI introduces Birch Assist to help automate the complex after-call-work using our own state-of-the-art AI tools. We offer variety of options including **Live Call Analytics** - Task Tracking, Sentiment Tracking, Fields Extraction, Pacing guidance among others and **After Call Work** that involves summary, call reason, call classification. 

For more information and how to setup Birch Assist for your organization within the Genesys Cloud, contact us [here](https://birch.ai/#footerscroll).

# Architecture Overview
The following illustration shows the integration overview between the Genesys Cloud and BirchAI:

![Birch Assist Integration](images/genesys_birchai_workflow.png "Birch Assist Integration Overview")


# Solution components
## Genesys Cloud
A suite of Genesys cloud services for enterprise-grade communications, collaboration, and contact center management.

## Genesys AppFoundry
The Genesys app marketplace for solutions that run on the Genesys Cloud platform. You download the integration used in this solution from the Genesys AppFoundry.

## BirchAI Account
You would need an active BirchAI account.

## AudioHook integration
For the live call streams - audio hook integration is required. 

## Specialized knowledge
Administrator-level knowledge of Genesys Cloud  
Experience using the Genesys Cloud OAuth Process for third party apps


# Deployment Steps

The Birch AI integration has the following steps:

* Create a custom role for Birch Assist
* Create a Client Credentials OAuth Client for Birch in the Genesys Cloud
* Setup AudioHook integration for your organization
* Contact Birch to link AudioHook to Birch Assist

## Create a custom role for Birch Assist
1. Login to your Genesys Cloud organization and [create a new role](https://help.mypurecloud.com/articles/add-roles/) with the following permissions:

    * Analytics  Agent Conversation Detail  View
    * Analytics  Conversation Detail  View
    * Authorization  Role  View
    * OAuth  Client  View
    * Integrations  Integration  Edit

2. Assign the role to yourself

## Create a Client Credentials OAuth Client
1. Login to your Genesys Cloud organization and [create a Client Credentials OAuth Client](https://help.mypurecloud.com/articles/create-an-oauth-client/)
2. Select Client Credentials in the Grant Types and click the Roles tab
3. Assign the custom role created above to the OAuth Client and save
4. Note the Client ID and the Client Secret

## Setup the AudioHook Integration
1. Setup the AudioHook integration for your Genesys Cloud organization (skip if you already have AudioHook setup)

## Contact Birch
1. Share the Client ID and Client Secret for the OAuth Client with the Birch Team.
2. Once AudioHook is setup, we will provide you with a Connection URI to configure AudioHook to start streaming live audio to Birch.



For any questions regarding the setup process, please contact us here - demo@birch.ai
