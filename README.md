# Crash Course to DialogFlow
## What we will make:
* Postpaid Plan Inquiries
* Personality: Polite and Professional

## Conversational Design Flow
![alt text](images/image.png)

## Step - by - step building


### 1) Initialize the agent
Create an agent on the DialogFlow console and give it your desired name. `sample_agent` was used for this example
![alt text](images/df1.png)

### 1.1) DialogFlow Console
Short Introductory to the DialogFlow console:
![alt text](images/df0.png)
*1*: `Intents Tab`<br />
  Where you would build, delete and modify your intents<br />
*2*: `Entities Tab`<br />
  Where you would build, delete and modify your entities<br />
*3*: `Fulfillment Tab`<br />
  Where you would setup your fulfillment and webhooks<br />
*4*: `Integrations Tab`<br />
  Where you would setup your agent's integration<br />
*5*: `Tab Indicator`<br />
  Tells what tab you're currently at<br />
*6*: `Agent Tester`<br />
  Text Field are where you can test your agent (Intent invocations, etc.)


### 2) Change the response of the Default welcome Intent
There is a preloaded agent response provided by google under `Default Welcome Intent`, change it to the desired response when users greets the agent. In the example, we used:
```
Hi, Welcome to Sample Telecom! How may I help?
```
After changing the response, save it and use the `agent tester` to see the changes
![alt text](images/df2_1.png)

### 3) Add a new intent for catering the plans
* Create a new intent for when the user is Asking the Plans. In the example we named it: `plans`
* Add the training phrases or the user utterances. Or what the user must say to trigger the intent
* Add the agent's response when this trigger is intent. For the example, we used: 
```
We are offering multiple plans to fit your budget and needs. We have Sample Plan 499 and Sample Plan 999. Please let me know what plan you would like to know more.
```
* Save the agent
![alt text](images/df3.png)

### 4) Create entities for the plans
From this example, we have seen that there are two plans of choice given by the agent. And instead of creating two different sets of intents, we could just make an entity for it to know what `Postpaid Plan` our user is talking about.
* On the entity tab, click `Create Entity`
* Set the Entity Name to `postpaid_plans`
* Set the first property/parameter to `499` and set its synonyms
* Set the second property/parameter to `999` and set its synonyms
* Save the entity created
