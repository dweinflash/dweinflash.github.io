---
layout: post
title: "On-Call Agent"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: OnCallAgent_Architecture.png
---

Aiming to bring together the major topics discussed during [Agent Engineering Bootcamp](https://maven.com/agent-lab/agent-engineering-bootcamp), this capstone project introduces an On-Call Support Agent to assist engineers with application support. Built using [Slack](https://slack.com), [Claude Sonnet](https://www.anthropic.com/claude/sonnet), [LangChain](https://www.langchain.com/), [OpenAI](https://openai.com/api/) and [Chroma](https://www.trychroma.com/), the agent uses operational runbooks and [GitHub](https://github.com) repositories to provide relevant, context-aware responses to help engineers quickly resolve incidents and better understand the overall design of the system.

## Goals

* Accelerate incident response by providing on-call engineers with targeted resolution steps.

* Answer system architecture and implementation detail questions by analyzing GitHub repositories.

* Help onboard new engineers with an assistant that answers questions about the operational and technical details of an application.

## Takeaways

* Retrieval-Augmented Generation (RAG) transforms static documentation into actionable knowledge, giving the agent a solid foundation for relevant and accurate responses.

* Model Context Protocol (MCP) enables direct integration between Claude Sonnet and GitHub, allowing the agent to search and analyze the codebase in real-time for code exploration and system understanding.

* Slack commands helped to create purpose-built workflows, with distinct commands for incident response, repository analysis and private messaging.

## Documents

* [Presentation](/assets/pdf/OnCallAgent_Presentation.pdf)
* [Demo](https://www.youtube.com/watch?v=I8wt8cshQQE)
* [Code](https://github.com/dweinflash/slack-on-call-agent)
