# Universal Chat Modulator

### Real-time multi-platform livestream chat aggregation and analysis

Universal Chat Modulator is a Python application designed to collect livestream chat from multiple platforms, unify incoming messages, and perform real-time conversational analysis.

The project currently provides working integrations for **Twitch and YouTube**, with an experimental TikTok connector under development.

---

## Demo

### Screenshots

#### Initialization

![Universal Chat Modulator Initialization](screenshots/Modulator%20Initialize.png)

#### Live Multi-Platform Processing

![Universal Chat Modulator Running](screenshots/Modulator%20Running.png)

#### Chat Analysis

![Universal Chat Modulator Analysis](screenshots/Modulator%20Analysis.png)

> Video demonstration coming soon.

---

## What It Does

Universal Chat Modulator creates a single processing pipeline for livestream chat coming from different platforms.

Instead of treating each platform independently, incoming messages are normalized into a common format and passed through the same analysis system.

### Supported Platforms

| Platform         | Status                 |
| ---------------- | ---------------------- |
| Twitch           | Working                |
| YouTube          | Working                |
| Twitch + YouTube | Working simultaneously |
| TikTok           | Experimental           |

---

## Features

### Multi-Platform Monitoring

Monitor Twitch and YouTube livestreams individually or simultaneously.

### Unified Chat Processing

Messages from different platforms are converted into a common format so they can be processed by the same system.

### Real-Time Statistics

The application tracks:

* Total messages
* Unique users
* Most active users
* Frequently used words
* Common phrases

### Reaction Detection

The system analyzes messages and identifies conversational reactions such as:

* Approval
* Disapproval
* Excitement
* Surprise

---

## Example Output

A multi-platform session can produce analysis similar to:

```text
==================================================
CHAT ANALYSIS
==================================================

Messages: 74
Unique users: 28

Top users:
  @example_user: 15
  @another_user: 9

Top words:
  hello: 9
  chat: 6
  yo: 4

Top phrases:
  hello chat: 2
  how are: 1

Reactions:
  disapproval: 35
  excitement: 22
  approval: 2
  surprise: 1
```

---

## Architecture

```text
                 LIVESTREAM PLATFORMS

        Twitch        YouTube        TikTok
           |             |        (Experimental)
           |             |             |
           +-------------+-------------+
                         |
                         v
                UNIFIED CHAT PROCESSOR
                         |
                         v
                   CHAT ANALYSIS
                         |
          +--------------+--------------+
          |              |              |
          v              v              v
      User Stats    Word/Phrase     Reactions
                     Analysis       Detection
```

The architecture is designed so additional platform connectors can feed into the same processing pipeline without requiring the analysis system to be rewritten for each platform.

---

## Technology

* **Python**
* Twitch EventSub
* YouTube Live Chat API
* OAuth authentication
* WebSocket communication
* Real-time event processing
* Text normalization
* Statistical text analysis

---

## Project Highlights

This project demonstrates experience with:

* API integration
* OAuth authentication
* WebSocket communication
* Real-time event handling
* Multi-platform data aggregation
* Text processing
* Data analysis
* Modular Python application design

---

## Project Status

### Working

* Twitch livestream chat
* YouTube livestream chat
* Simultaneous Twitch + YouTube monitoring
* Unified message processing
* User statistics
* Word and phrase analysis
* Reaction detection

### Experimental

* TikTok livestream integration

---

## Source Code

The complete source code is maintained in a **private repository**.

This public repository is intended to demonstrate the project's functionality, architecture, and capabilities without exposing the application's private implementation or API credentials.

---

## Author

**Bohdan Krasikov**

Computer Science student and software developer building projects involving automation, APIs, real-time systems, and AI-related applications.
