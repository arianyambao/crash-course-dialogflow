# Crash Course to DialogFlow
## What we will make:
* Postpaid Plan Inquiries
* Personality: Polite and Professional

## Conversational Design Flow
![alt text](images/image.png)

## Step - by - step building
### 0) DialogFlow Console
Short Introductory to the DialogFlow console:<br />

*1*: Intents Tab<br />
  Where you would build, delete and modify your intents<br />
*2*: Entities Tab<br />
  Where you would build, delete and modify your entities<br />
*3*: Fulfillment Tab<br />
  Where you would setup your fulfillment and webhooks<br />
*4*: Integrations Tab<br />
  Where you would setup your agent's integration<br />
*5*: Tab Indicator<br />
  Tells what tab you're currently at<br />
*6*: Agent Tester<br />
  Text Field are where you can test your agent (Intent invocations, etc.)
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

