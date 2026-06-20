# OPI Concepts

This document defines the core concepts used by Open Professional Identity (OPI).

The goal is to create a shared vocabulary for the specification, implementation, documentation, and future ecosystem.

## Professional Identity

A structured representation of a person's professional background, experience, skills, projects, achievements, education, public work, and trusted references.

In OPI, a professional identity is designed to be readable by both humans and software systems, including AI agents.

## Publisher

A person who owns, curates, and publishes their professional identity.

Publishers may connect existing sources such as LinkedIn, GitHub, personal websites, resumes, portfolios, freelance platforms, publications, and certifications.

The publisher remains the owner of the professional identity.

## Consumer

A human, organization, application, or AI system that reads, analyzes, compares, or interacts with a professional identity.

Consumers may include recruiters, headhunters, employers, clients, investors, marketplaces, ATS systems, and AI agents.

## Identity Source

An original source of professional information.

Examples include LinkedIn, GitHub, Dribbble, Upwork, a personal website, a resume, a portfolio, a blog, a certification platform, or a publication database.

## Connector

A component that imports, extracts, or synchronizes information from an identity source into the OPI format.

Connectors allow OPI to aggregate fragmented professional information without replacing existing platforms.

## Professional Knowledge Base

A curated collection of structured and semi-structured information that represents a publisher's professional identity.

The knowledge base may include profile information, experience, projects, skills, education, certifications, articles, presentations, recommendations, and other public professional content.

## OPI Manifest

A machine-readable file that describes where and how a professional identity can be accessed.

The manifest may point to public profile data, structured files, APIs, search endpoints, or AI agent interfaces.

Example:

```json
{
  "version": "0.1",
  "name": "Jane Doe",
  "profile": "/profile.json",
  "projects": "/projects.json",
  "skills": "/skills.json"
}
```

## Identity Endpoint

A public URL where a professional identity can be accessed by humans or software systems.

An identity endpoint may expose static files, an API, a chat interface, an MCP server, or other supported access methods.

## Professional Agent

An optional AI-powered interface that can answer questions, summarize experience, compare a profile with a job description, or help consumers understand a professional identity.

A professional agent should use the publisher's professional knowledge base as its source of truth.

## Human-Readable Representation

A version of the professional identity designed for people.

Examples include portfolio pages, case studies, timelines, resumes, and profile pages.

## AI-Readable Representation

A structured or semi-structured version of the professional identity designed for software systems and AI agents.

Examples include JSON files, APIs, manifests, schemas, embeddings, or MCP tools.

## Source of Truth

The trusted version of a professional identity maintained by the publisher.

OPI aims to help professionals maintain one source of truth that can be reused across many interfaces and consumed by many systems.
