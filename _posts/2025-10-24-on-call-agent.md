---
layout: post
title: "On-Call Agent"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: OnCallAgent_Architecture.png
---

This capstone project from [Agent Engineering Bootcamp](https://maven.com/agent-lab/agent-engineering-bootcamp) introduces an On-Call Support Agent to assist engineers with application maintenance and operational support. Built using [Slack](https://slack.com), [Claude Sonnet](https://www.anthropic.com/claude/sonnet), [LangChain](https://www.langchain.com/), [OpenAI](https://openai.com/api/) and [Chroma](https://www.trychroma.com/), the agent uses operational runbooks and [GitHub](https://github.com) repositories to provide relevant, context-aware responses to help engineers quickly resolve incidents and better understand the technical details of an application.

## Goals

* Accelerate incident response by providing on-call engineers with targeted resolution steps.

* Answer system architecture questions by analyzing GitHub repositories.

* Help onboard new engineers with an assistant that answers questions about the operational and technical details of an application.

## Takeaways

* Retrieval-Augmented Generation (RAG) with operational runbooks gives the agent a solid foundation for relevant and accurate responses.

* The GitHub Model Context Protocol (MCP) server allows the agent to search and analyze the codebase in real-time to answer any system design questions.

* Slack commands helped to create purpose-built workflows, with distinct commands for incident response, repository analysis and private messaging.

## Documents

* [Presentation](/assets/pdf/OnCallAgent_Presentation.pdf)
* [Demo](https://www.youtube.com/watch?v=I8wt8cshQQE)
* [Code](https://github.com/dweinflash/slack-on-call-agent)
