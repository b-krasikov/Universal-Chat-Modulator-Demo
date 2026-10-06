\# Universal Chat Modulator



\### Real-time multi-platform livestream chat aggregation and analysis



Universal Chat Modulator is a Python application designed to collect livestream chat from multiple platforms, unify the incoming messages, and perform real-time conversational analysis.



The project currently provides working integrations for \*\*Twitch and YouTube\*\*, with an experimental TikTok connector under development.



\---



\## Demo



> \*\*Demo video coming soon\*\*



The demonstration shows the application connecting to multiple livestream platforms, receiving messages in real time, and generating chat analytics.



\---



\## What It Does



Universal Chat Modulator creates a single processing pipeline for livestream chat coming from different platforms.



Instead of treating each platform independently, incoming messages are normalized into a common format and passed through the same analysis system.



\### Supported Platforms



| Platform         | Status                     |

| ---------------- | ------------------------   |

| Twitch           | Working                    |

| YouTube          | Working                    |

| Twitch + YouTube | Working simultaneously     |

| TikTok           |Research \& Development Phase|



\---



\## Features



\### Multi-Platform Monitoring



Monitor Twitch and YouTube livestreams individually or simultaneously.



\### Unified Chat Processing



Messages from different platforms are converted into a common format so they can be processed by the same system.



\### Real-Time Statistics



The application tracks:



\* Total messages

\* Unique users

\* Most active users

\* Frequently used words

\* Common phrases



\### Reaction Detection



The system analyzes messages and identifies conversational reactions such as:



\* Approval

\* Disapproval

\* Excitement

\* Surprise



\---



\## Example Output



A multi-platform session can produce analysis similar to:



```text

==================================================

CHAT ANALYSIS

==================================================



Messages: 74

Unique users: 28



Top users:

&#x20; @example\_user: 15

&#x20; @another\_user: 9



Top words:

&#x20; hello: 9

&#x20; chat: 6

&#x20; yo: 4



Top phrases:

&#x20; hello chat: 2

&#x20; how are: 1



Reactions:

&#x20; disapproval: 35

&#x20; excitement: 22

&#x20; approval: 2

&#x20; surprise: 1

```



\---



\## Architecture



```text

&#x20;                   LIVESTREAM PLATFORMS

&#x20;                          │

&#x20;         ┌────────────────┼────────────────┐

&#x20;         │                │                │

&#x20;      Twitch           YouTube          TikTok

&#x20;         │                │          (Experimental)

&#x20;         └────────────────┼────────────────┘

&#x20;                          │

&#x20;                          ▼

&#x20;                UNIFIED CHAT PROCESSOR

&#x20;                          │

&#x20;                          ▼

&#x20;                   CHAT ANALYSIS

&#x20;                          │

&#x20;         ┌────────────────┼────────────────┐

&#x20;         │                │                │

&#x20;    User Stats       Word/Phrase      Reactions

&#x20;                      Analysis         Detection

```



The architecture is designed so additional platform connectors can feed into the same processing pipeline without requiring the analysis system to be rewritten for each platform.



\---



\## Technology



\* \*\*Python\*\*

\* Twitch EventSub

\* YouTube Live Chat API

\* OAuth authentication

\* WebSocket communication

\* Real-time event processing

\* Text normalization

\* Statistical text analysis



\---



\## Project Highlights



This project demonstrates experience with:



\* API integration

\* OAuth authentication

\* WebSocket communication

\* Real-time event handling

\* Multi-platform data aggregation

\* Text processing

\* Data analysis

\* Modular Python application design



\---



\## Project Status



\### Working



\* Twitch livestream chat

\* YouTube livestream chat

\* Simultaneous Twitch + YouTube monitoring

\* Unified message processing

\* User statistics

\* Word and phrase analysis

\* Reaction detection



\### Experimental



\* TikTok livestream integration



\---



\## Source Code



The complete source code is maintained in a \*\*private repository\*\*.



This public repository is intended to demonstrate the project's functionality, architecture, and capabilities without exposing the application's private implementation or API credentials.



\---



\## Author



\*\*Bohdan Krasikov\*\*



Computer Science student and software developer building projects involving automation, APIs, real-time systems, and AI-related applications.



