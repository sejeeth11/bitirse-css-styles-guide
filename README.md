---
title: 1.0 Welcome & Quick Start
description: The primary developer onboarding hub and technical roadmap for building, testing, and deploying mobile solutions.
sidebar:
  order: 1
---

import { Aside, Steps } from '@astrojs/starlight/components';

<Aside type="tip">
👋 **Welcome to the Mobile Engineering Platform!** This portal serves as your comprehensive starting point for requesting repository access, configuring your local developer workstation, mastering our 3-layer Clean Architecture standards, and landing your first pull request smoothly. **Target Onboarding SLA: Land your first verified PR within 48 hours.**
</Aside>

## 1.0.1 Interactive Onboarding Decision Flowchart

Use this decision flowchart to determine your exact onboarding path based on your role background and target tech stack:

<pre class="mermaid">
flowchart TD
    Start["Start Onboarding Journey"] --> Q1{"Are you a Web or Backend Dev?"}
    
    Q1 -- "Yes (New to Mobile)" --> TrackA["Read 1.3 Non-Mobile Track"]
    Q1 -- "No (Mobile Engineer)" --> Q2{"What is your target stack?"}
    
    TrackA --> Q2
    
    Q2 -- "React Native" --> SetupRN["1.5 Setup Node.js, Watchman, Xcode & AS"]
    Q2 -- "Native iOS" --> SetupIOS["1.5 Setup macOS, Xcode & CocoaPods"]
    Q2 -- "Native Android" --> SetupAndroid["1.5 Setup Android Studio & JDK 17"]
    
    SetupRN --> Verification["Run Local Verification Build"]
    SetupIOS --> Verification
    SetupAndroid --> Verification
    
    Verification --> TrackB["1.2 Follow New Mobile Engineer Track"]
    TrackB --> Done["Submit & Merge First PR"]
</pre>

---

## 1.0.2 Onboarding Milestones & SLA Timeline

Every new developer follows our 4-phase onboarding SLA to ensure a predictable 0-to-1 setup:

| Phase | Milestone Goal | Key Action Required | Target SLA |
| :--- | :--- | :--- | :--- |
| **Phase 1** | Ecosystem & Architecture | Read [1.1 Platform Overview](/mobile/onboarding/platform-overview/) & governance policies | **Day 1 (Morning)** |
| **Phase 2** | Tech Stack Selection | Review [1.4 Tech Stack Selection](/mobile/onboarding/tech-stack-selection/) (React Native vs Native) | **Day 1 (Afternoon)** |
| **Phase 3** | Workstation Setup | Follow [1.5 Machine Setup Guide](/mobile/onboarding/machine-setup/) (macOS/Windows) | **Day 2 (Morning)** |
| **Phase 4** | First PR & Build Verification | Complete [1.2 New Mobile Engineer Track](/mobile/onboarding/new-engineer-onboarding/) & merge first PR | **Day 2 (Afternoon)** |

---

## 1.0.3 Role-Based Onboarding Pathways

### Track A: Experienced Mobile Engineers
Designed for developers with existing iOS (Swift), Android (Kotlin), or React Native experience. Skip basic mobile concepts and go directly to repo entitlement requests, IDE setup, and CI/CD quality gates.

- ➔ Open [1.2 New Mobile Engineer Track](/mobile/onboarding/new-engineer-onboarding/)

### Track B: Web & Backend Developers ("Mobile 100")
Designed for engineers transitioning from web or backend microservices. Covers mobile binary compilation, activity/view lifecycles, app signing certificates, and offline-first caching strategies.

- ➔ Open [1.3 Non-Mobile Engineer Track](/mobile/onboarding/non-mobile-engineer-guide/)

---

## 1.0.4 Account Entitlements & Platform Tooling

Before commencing local setup, verify that your manager has requested access to these core systems:

| Tool / Platform | Purpose | Access Request Channel | Verification Step |
| :--- | :--- | :--- | :--- |
| **GitHub Enterprise** | Source Code Repositories & PR Code Reviews | Access Portal / Manager Approval | Clone repository via SSH |
| **Bitrise CI/CD** | Automated Build Pipelines & Test Execution | SSO Entitlement Group | Log in to Bitrise Dashboard |
| **Apple Developer Portal** | iOS Provisioning Profiles & TestFlight Releases | Mobile Platform Admin Request | Verify Apple Developer Org invite |
| **Google Play Console** | Android Internal App Sharing & Store Releases | Mobile Platform Admin Request | Access Google Play Console invite |
| **Datadog RUM** | Real User Monitoring Telemetry & Crash Analytics | Datadog SSO Group | Access Mobile Telemetry Dashboard |

---

## 1.0.5 Community & Platform Support Channels

If you encounter build failures, credential issues, or setup blockers during onboarding, utilize our support channels:

- **MS Teams Support Channel:** `#mobile-engineering-support` (Asynchronous Q&A and build help)
- **Architecture Guild Meeting:** Thursdays @ 10:00 AM EST (Live RFC reviews and Q&A)
- **Documentation RFCs:** Submit a pull request to update or expand this portal.
