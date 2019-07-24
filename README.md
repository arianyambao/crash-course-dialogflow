# Crash Course to DialogFlow
## What we will make:
* Postpaid Plan Inquiries
* Personality: Polite and Professional

## Conversational Design Flow
![alt text](images/image.png)

## Step - by - step building
### 0) DialogFlow Console
Short Introductory to the DialogFlow console:
*1*: Intents Tab
   * Where you would build, delete and modify your intents
*2*: Entities Tab
   * Where you would build, delete and modify your entities
*3*: Fulfillment Tab
   * Where you would setup your fulfillment and webhooks
*4*: Integrations Tab
   * Where you would setup your agent's integration
*5*: Tab Indicator
   * Tells what tab you're currently at
*6*: Agent Tester
   * Text Field are where you can test your agent (Intent invocations, etc.)
![alt text](images/df0.png)

### 1) Initialize the agent
Create an agent on the DialogFlow console and give it your desired name. `sample_agent` was used for this example
![alt text](images/df1.png)

### 2) Change the response of the Default welcome Intent
There is a preloaded agent response provided by google under `Default Welcome Intent`, change it to the desired response when users greets the agent. In the example, we used:
```
Hi, Welcome to Sample Telecom! How may I help?
```
After changing the response, save it and use the `agent tester` to see the changes
![alt text](images/df2_1.png)

