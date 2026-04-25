# AI Finance Agent with Amazon Bedrock

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-genai-bedrock-agent)

**Author:** Shahryar Ahmed  
**Email:** ashahryar200@gmail.com

---

---

## Introducing Today's Project!

In this project, I will build Bedrock Agent that look into my finanical data and makes suggestion. I'm doing this project to learn how to use AWS Bedrock Agents.

### Key services and concepts

I used Amazon Bedrock Agents and Code Interpreter to build a finance advisor that writes and runs Python code on its own. Key concepts I picked up include prompt engineering, agent traces, foundation models, and enabling agent memory for cross-session context.

### Challenges and wins

This project took me about an hour to complete, and the most challenging part was understanding how agent traces work and iterating on prompt instructions. The most rewarding part was seeing the agent autonomously write Python code and generate spending charts from just a simple conversation.

---

## Exploring Amazon Bedrock and Foundation Models

In this step, I am navigating to AWS Bedrock because I'm working with AWS Bedrock Agents. I'm then going to preview the Bedrock Agents features.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_w5x8n1q4)

### Understanding foundation models

A foundation model is a large AI model pre-trained on massive data that you access via an API. We use Amazon Nova 2 Lite because it's Amazon-owned and automatically available. It's also lightweight, cost-effective, and handles code generation well.

### Discovering Bedrock Agents

A Bedrock Agent is an AI that reasons through multi-step tasks autonomously. Unlike a simple chatbot that just answers questions, an agent can decide what actions to take, execute code, call APIs, and iterate on results. You give it instructions in plain English and it figures out the steps on its own — this is Agentic AI.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_h4t7y1a5)

---

## Creating the AI Finance Agent

In this step, I will create an Bedrock Agent as a personal financial advisor. Enable to write and execute Python Code.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_q4j6r2m8)

### Crafting the agent instructions

I wrote instructions that tell my agent to analyze spending data. This is important because it iswhat is the agent bases its responses around.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_f2d8g4l6)

---

## Analyzing Spending Data with Code Interpreter

In this step, I will test my finance Bedrock Agent. I will upload a CSV and get it to summarise my data. 

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_p4r7t9v1)

### How Code Interpreter processed the data

I uploaded transcation.csv. The agent used Code Interpreter to write Python code that analyzes my csv file. The output shows the total spendingby category.

---

## Iterating on Agent Instructions with Traces

I changed the instructions to give a % output break down. The output improved by showing a table with the cst of two decimal place and % a breakdown.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_q5s8u2w4)

---

## Enabling Cross-Session Agent Memory

In this project extension, I'm  enabling agent memory with session summarization so the Bedrock Agent retains context across separate conversations. Without it, the agent forgets everything and starts from scratch every time a user returns. Cross-session memory lets the agent recall past spending patterns and budget goals, making it actually useful over time.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_n5m3k7j1)

### Session summarization vs full history

I configured compresses each conversation into a compact summary and stores it in agent memory, so context carries over to future sessions. Without it, the agent treats every new session as a blank slate with zero knowledge of prior interactions. For a finance agent, this means it can recall your past spending patterns, budget goals, and preferences instead of asking the same questions again.

![Image](http://learn.nextwork.org/cheerful_lavender_wise_quoll/uploads/aws-genai-bedrock-agent_t8h1g5f3)

### Testing cross-session recall

In this project extension, I tested the memory feature of Bedrock agents. The agent recalled all three suggestions it had give me eariler

---

## Wrapping Up

I did this project today to learn how to build an AI agent that can reason and act on its own using Amazon Bedrock. Next, I'd love to explore connecting agents to external APIs and databases so they can do even more in the real world.

---

---
