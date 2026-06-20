# Architecture

## Core Concept

The central object of the Open Professional Identity ecosystem is the **Professional Identity**.

A Professional Identity is a structured, portable, and trusted representation of a person's professional experience, skills, projects, achievements, and other publicly shared professional information.

Everything else in OPI exists to create, maintain, publish, or consume a Professional Identity.

---

## High-Level Architecture

                           Publisher

        LinkedIn   GitHub   Upwork   CV   Portfolio
             │        │        │      │        │
             └────────┴────────┴──────┴────────┘
                              │
                              ▼
                      Identity Sources
                              │
                              ▼
                     OPI Builder (future)
                              │
                              ▼
                 Professional Identity
                     (Core Object)
                              │
              ┌───────────────┼───────────────┐
              │               │               │
              ▼               ▼               ▼
      Human Interface     API Endpoint    AI Interface
              │               │               │
              ▼               ▼               ▼
         Portfolio        Applications     AI Agents
