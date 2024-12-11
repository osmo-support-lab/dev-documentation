---
description: This documentation contains all technical details about the ISG backend
---

# ISG Backend Documentation

## About this document

This document provides technical details of the ISG Backend features, along with the context and rationale behind each design choice.

## General approach

The project's goal is to provide a modular backend approach. This aims to eliminate maintaining multiple codebases by creating a single codebase that can serve various purposes (e.g., database, API, engine, etc.).

Each feature is encapsulated within a module that contains all the logic and workflows. In addition to these modules, the project will provide key services to them,

* Database
* API (including authentication provided by the user module)
* Event handler

Modules can utilize services, such as adding API routes or registering event handlers Some modules, like the User module, are critical and should be dealt with caution. Any module that supports a service or another module is considered a key module.

Each database model typically has its own dedicated module. For example, the Chat module manages chat creation, tags, statuses, and more. Similarly, the Message module is responsible for creating messages, retrieving them, and other related functionalities.
