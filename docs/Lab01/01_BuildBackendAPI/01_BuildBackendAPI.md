---
title: 'Exercise 01: Build a backend API'
layout: default
nav_order: 3
has_children: true
parent: 'Lab 1: TechLab MCP Server integration and connected agents'
---

# Exercise 01: Build a backend API

In this exercise, you'll set up an API based on Azure Functions and install it as an API plugin for Microsoft 365 Copilot.

<!-- <div class="lab-intro-video">
    <div style="flex: 1; min-width: 0;">
        <iframe  src="//www.youtube.com/embed/XO2aG3YPbPc" frameborder="0" allowfullscreen style="width: 100%; aspect-ratio: 16/9;">          
        </iframe>
    </div>
</div> -->

## Introduction

In this exercise, you'll set up a REST API for Trey Research, a hypothetical consulting company. It provides API's for accessing information about consultants (using the **/api/consultants** path) and about the current user (using the **/api/me** path). For now, the API doesn't support authentication, so the current user will always be a dummy user, Avery Howard.

The code consists of Azure Functions written in TypeScript, backed by a database in Azure Table storage. When you run the app locally, table storage will be provided by the Azurite storage emulator.

{: .knowledge } 
> **How was this API created?**
>
> The project was created using the Microsoft 365 Agents Toolkit. You can create the same scaffolding for your own project by opening an empty folder in VS Code and going to Agents Toolkit. [Read more](https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/build-declarative-agents).
