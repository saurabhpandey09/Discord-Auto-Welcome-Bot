# Discord Auto Welcome Bot

A production-ready automation that greets new Discord members, assigns roles, and kicks off onboarding flows automatically—no manual mod work required. Built for Android device/emulator control, the bot mimics human actions to DM welcomes, post channel greetings, and route users through rules or verification. The result: faster onboarding, higher engagement, and consistent member experience powered by the **Discord Auto Welcome Bot**.

<p align="center">
  <a href="https://Appilot.app" target="_blank">
    <img src="media/appilot-baner.png" alt="Appilot Banner" width="100%">
  </a>
</p>
<p align="center">
  <a href="https://t.me/devpilot1" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20Appilot%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:support@appilot.app" target="_blank">
    <img src="https://img.shields.io/badge/Email-support@appilot.app-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://appilot.app" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>

<p align="center"> 
   Created by Appilot, built to showcase our approach to Automation!<br>
   <strong>If you are looking for custom Discord Auto Welcome Bot, you've just found your team — Let’s Chat.👆👆</strong>
</p>

## Introduction

**What it does:** Automates Discord server welcomes—detects new joins, sends personalized DMs, posts channel greetings, assigns roles, and triggers onboarding steps (rules, forms, verification).

**Problem it solves:** Moderators waste time greeting newcomers and applying rules consistently; manual workflows are slow, inconsistent, and prone to mistakes.

**Benefit:** Always-on, policy-compliant onboarding that scales to hundreds of servers and accounts with human-like behavior and robust anti-detection patterns.

### Automating Discord Member Onboarding
- Detects member join events and triggers multi-step welcome flows (DM + channel post + role assignment).
- Context-aware messages (server name, invite source, locale, time window) with smart throttling and schedules.
- Works on real devices and emulators via Appilot + UI Automator/Appium for resilient UI control.
- Built-in retry, logging, and analytics dashboards for mod teams and growth managers.
- Integrates with webhooks/CRMs to qualify leads or send onboarding form responses downstream.

## Core Features

- **Real Devices and Emulators:** Drive physical Android phones and emulators (Bluestacks/Nox) for reliable Discord app control with UI Automator/Appium.  
- **No-ADB Wireless Automation:** ADB-less, socket-based control path to reduce detection vectors and support devices without USB tethering.  
- **Mimicking Human Behavior:** Randomized delays, gesture curves, typing cadence, scroll variance, and session warmups to emulate real usage.  
- **Multiple Accounts Support:** Rotate verified Discord accounts with isolated app profiles/containers, independent caches, and per-account rules.  
- **Multi-Device Integration:** Parallel workers across 5–300+ devices; central scheduler assigns tasks and balances throughput.  
- **Exponential Growth for Your Account:** Faster welcome-to-first-message times, higher retention via personalized onboarding and CTA routing.  
- **Premium Support:** Priority SLAs, device-farm advisory, custom flows, and white-glove deployment.  
- **Role Assignment Rules:** Auto-assign starter roles based on invite link, locale, or questionnaire responses.  
- **Verification & Safety Steps:** Optional captcha/emoji reactions, rules acknowledgment, or age gates before unlocking roles/channels.  
- **Webhook/CRM Integrations:** Send join metadata and DM form responses to Slack, Notion, Sheets, or webhooks for lead tracking.

**Additional Feature Set**

| Feature | Description |
|---|---|
| Template-Driven Messaging | Markdown-ready DM/channel templates with variables (username, server name, invite code, timestamps). |
| Smart Scheduling | Time windows, per-account daily caps, cooldowns, and burst protection to avoid rate limits. |
| Invite Source Routing | Different flows for organic joins vs. campaign links; A/B test welcome scripts. |
| Audit & Compliance Logs | Structured logs for each action (tap, type, send) with screenshots and device IDs. |
| Proxy & IP Hygiene | Per-device proxy assignment, sticky sessions, and locale-aligned profiles. |
| Crash & Retry Orchestrator | Detects UI stalls, reboots app/device when needed, and resumes the exact step safely. |

</p>
<p align="center">
  <a href="https://appilot.app" target="_blank">
    <img src="media/{{Discord Auto Welcome Bot-banner}.png" alt="{{Discord Auto Welcome Bot-architecture}" width="95%">
  </a>
</p>

## How It Works

1. **Input or Trigger** — From the Appilot dashboard, select target servers/accounts and choose the welcome flow (DM + role + channel post), limits, and schedules.  
2. **Core Logic** — Appilot controls the Android device/emulator via **UI Automator** or **ADB** alternatives, navigating the Discord app UI, opening member lists, composing DMs, and tapping reaction/verification steps.  
3. **Output or Action** — Sends configured welcomes, assigns roles, posts channel greetings, and records join metadata to logs or webhooks.  
4. **Other functionalities** — Retry logic for rate limits, screenshot logging, error classification, and parallel device execution are configurable in the dashboard.

## Tech Stack

- **Language:** Kotlin, Java, Python, JavaScript  
- **Frameworks:** Appium, UI Automator, Espresso, Robot Framework, Cucumber  
- **Tools:** Appilot, Android Debug Bridge (ADB), Appium Inspector, Bluestacks, Nox Player, Scrcpy, Firebase Test Lab, MonkeyRunner, Accessibility  
- **Infrastructure:** Dockerized device farms, cloud emulators, proxy networks, parallel device execution, task queues, real device farm

## Directory Structure
```
    discord-auto-welcome-bot/
    │
    ├── src/
    │   ├── main.py
    │   ├── automation/
    │   │   ├── detectors/
    │   │   │   ├── join_watchdog.py
    │   │   │   └── rate_limit_guard.py
    │   │   ├── flows/
    │   │   │   ├── dm_welcome.py
    │   │   │   ├── channel_greeting.py
    │   │   │   └── role_assignment.py
    │   │   ├── device/
    │   │   │   ├── controller.py
    │   │   │   └── gestures.py
    │   │   └── utils/
    │   │       ├── logger.py
    │   │       ├── proxy_manager.py
    │   │       └── template_engine.py
    │
    ├── config/
    │   ├── servers.yaml
    │   ├── accounts.yaml
    │   └── schedules.yaml
    │
    ├── dashboards/
    │   └── metrics_panel.md
    │
    ├── logs/
    │   └── events.jsonl
    │
    ├── output/
    │   ├── screenshots/
    │   └── audit/
    │       └── actions.csv
    │
    ├── device-farm/
    │   ├── docker-compose.yaml
    │   └── README.md
    │
    ├── requirements.txt
    └── README.md
```

## Use Cases

- **Community managers** use it to greet newcomers and assign starter roles, so they can increase first-day engagement and reduce churn.  
- **Gaming servers** use it to funnel players into role-gated channels, so they can reduce spam and ensure rules are acknowledged.  
- **Education communities** use it to DM onboarding instructions and forms, so they can qualify students and route them to the right cohorts.  
- **Product teams** use it to identify invite sources and run A/B welcome scripts, so they can improve activation and measure campaigns.

## FAQs

**How do I configure this for multiple accounts?**  
Define each account in `config/accounts.yaml` with its device profile. The scheduler enforces per-account caps, cooldowns, and time windows to stay within rate limits.

**Does it support proxy rotation or anti-detection?**  
Yes. Assign per-device proxies with sticky sessions and region alignment. Human-like gestures, randomized delays, and staggered launches reduce behavioral fingerprints.

**Can I schedule it to run periodically?**  
Absolutely. Use `schedules.yaml` to set daily time windows, minute-level cron expressions, and per-server limits. The orchestrator will queue tasks across available devices.

**What if Discord changes the UI?**  
Selectors are versioned with fallback patterns; the controller includes visual anchors and heuristic recovery to adapt. Update packs can be rolled out without changing your flows.

## Performance & Reliability Benchmarks

- **Execution Speed:** 1–2 seconds to open DM composer, ~3–5 seconds per welcome end-to-end (device/network dependent).  
- **Success Rate:** 95% welcome flow completion across mixed devices in internal tests.  
- **Scalability:** Proven parallelization from 5 to 300+ Android devices; horizontal scale via additional device pods.  
- **Resource Efficiency:** Headless emulator profiles where possible; capped CPU shares and I/O throttling to keep worker density high.  
- **Error Handling:** Structured retries with backoff for rate limits; auto app relaunch on crash; screenshot + event logs; Slack/Telegram alerts for repeated failures.

##
<p align="center">
<a href="https://cal.com/app-pilot-m8i8oo/30min" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
</p>
