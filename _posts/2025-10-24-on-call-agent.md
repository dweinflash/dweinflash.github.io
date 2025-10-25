---
layout: post
title: "On-Call Agent"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: OnCallAgent_Architecture.png
---

This project introduces an On-Call Support Agent built with Slack, Claude Sonnet, RAG and MCP to support engineers during incident response and system design. The agent integrates Retrieval-Augmented Generation (RAG) for searching
operational runbooks and Model Context Protocol (MCP) for live codebase analysis. By utilizing RAG to retrieve relevant documentation and MCP to explore GitHub repositories, the agent provides context-aware responses
to accelerate user onboarding and incident resolution.

## Goals

* Accelerate incident resolution by providing on-call engineers with instant access to documented resolution steps through a RAG-powered knowledge base.

* Enable self-service code exploration, allowing engineers to query system architecture and implementation details through MCP-powered GitHub repository analysis.

* Help onboard new engineers by providing an interactive assistant that answers questions about both operational procedures and technical details.

## Takeaways

* RAG transforms static documentation into actionable knowledge by embedding markdown runbooks into a vector database, allowing for relevant and targeted responses.

* MCP enables direct integration between LLMs and development tools, allowing the agent to search and analyze GitHub repositories in real-time for code exploration and system understanding.

* Slack commands create purpose-built workflows, with distinct commands for incident response (/incident), repository analysis (/code) and private messaging (/ask).

## Documents

* [Presentation](/assets/pdf/OnCallAgent_Presentation.pdf)
* [Demo](https://www.youtube.com/watch?v=I8wt8cshQQE)
* [Code](https://github.com/dweinflash/slack-on-call-agent)
