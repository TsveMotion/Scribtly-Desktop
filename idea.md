# Scribtly Desktop - AI Script Generator

### OCR A-Level Computer Science | Component 03 Project Idea

**Language:** Python | **GUI Library:** Tkinter | **Database:** SQLite

---

## Overview

Scribtly Desktop is a standalone Python desktop application for content creators. The user inputs their platform, hook type, topic, and target audience. The app calls an AI API to generate a full video script, saves it to a local SQLite database, and allows the user to manage, rate, search, and organise their entire script library over time.

The app also features a **Content Roadmap** tool, which uses Dijkstra's shortest path algorithm to suggest the optimal sequence of video topics to produce, based on how well past topics have performed and how logically they connect to one another.

---

## The Problem It Solves

Content creators waste time staring at a blank page figuring out what to make next. They also have no central place to store, track, and review the scripts they have already written. Scribtly Desktop solves both problems: it generates scripts on demand and acts as a personal script library with performance tracking built in.

---

## Core Features

### Script Generation

* User selects platform (YouTube, TikTok, Instagram), hook type, tone, and video length
* User types in their topic and target audience
* App builds a structured prompt and sends it to the Anthropic API
* Generated script is displayed in the GUI and can be edited before saving

### Script Library

* All saved scripts stored in SQLite with full metadata
* Sort by date created, performance rating, platform, or word count
* Search by keyword, topic, hook type, or platform
* Click any script to view full content, edit it, or save a new version

### Version History

* Every time a script is edited and re-saved, a new version is created
* User can compare versions and revert to an older one at any time
* All versions stored persistently in the database

### Content Roadmap (Dijkstra's)

* Topics are stored as nodes in a weighted graph
* Edge weights are calculated from performance ratings of past scripts
* User inputs a starting topic and a goal topic
* Dijkstra's algorithm finds the optimal sequence of videos to produce to get from A to B
* Result displayed as a step-by-step content plan in the GUI

### Performance Tracking

* User can rate each script after filming it (1 to 5)
* Matplotlib charts show performance trends over time by platform and hook type
* App surfaces which hook types and platforms are working best

---

## OOP Class Structure

| Class            | Responsibility                                       |
| ---------------- | ---------------------------------------------------- |
| `User`         | Stores user profile and preferences                  |
| `Platform`     | Stores platform rules, tone defaults, max length     |
| `Script`       | Represents a single script with all metadata         |
| `Generator`    | Handles API prompt construction and response parsing |
| `ContentGraph` | Builds topic graph and runs Dijkstra's shortest path |

---

## A-Level Concepts Covered

| Requirement             | How It Is Met                                                     |
| ----------------------- | ----------------------------------------------------------------- |
| Object Oriented Design  | 5 core classes with encapsulation, methods, and relationships     |
| Permanent Storage       | SQLite database stores scripts, versions, ratings, and graph data |
| Shortest Path Algorithm | Dijkstra's used in ContentGraph to find optimal topic sequence    |
| Sorting                 | Script library sortable by multiple attributes                    |
| Searching               | Keyword and filter-based search across the script database        |
| Use of Libraries        | `tkinter`,`sqlite3`,`anthropic`,`matplotlib`              |

---

## Libraries Used

| Library        | Purpose                      | Source                  |
| -------------- | ---------------------------- | ----------------------- |
| `tkinter`    | GUI framework                | Python standard library |
| `sqlite3`    | Local database               | Python standard library |
| `anthropic`  | AI API for script generation | pip install             |
| `matplotlib` | Performance charts           | pip install             |

---

## GUI Screens

1. **Home** — welcome screen, quick stats, recent scripts
2. **Generate** — input form, generate button, output display, save button
3. **Library** — searchable and sortable table of all scripts
4. **Roadmap** — topic input, Dijkstra's output displayed as a content plan
5. **Settings** — API key, default preferences, user profile

---

## Possible Extensions

* Export any script to PDF using `reportlab`
* Multi-user profiles for teams or agencies & Using a extrenal db to store data
* Tag scripts with custom labels
* Track real-world view counts against scripts
* Suggest hook types based on historical performance data
