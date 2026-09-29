---
title: 1.0 Welcome & Quick Start
description: The primary developer onboarding hub and technical roadmap for building, testing, and deploying mobile solutions.
sidebar:
  order: 1
---

import { Aside, Card, CardGrid, Steps, Tabs, TabItem } from '@astrojs/starlight/components';

<Aside type="tip">
👋 **Welcome to the Mobile Engineering Platform!** Follow the decision guide and 4-step onboarding roadmap below to set up your workstation, obtain repository access, and land your first pull request smoothly. **Target Onboarding SLA: Land your first verified PR within 48 hours.**
</Aside>

## 1.0.1 Onboarding Decision Guide

Choose your role and target framework to route to your specific onboarding guide:

<CardGrid>
  <Card title="Track A: Experienced Mobile Engineer" icon="rocket">
    For developers with existing iOS (Swift), Android (Kotlin), or React Native experience. Skip mobile basics and request repo entitlements & IDE tools.
    
    [Open 1.2 New Mobile Engineer Track ➔](/mobile/onboarding/new-engineer-onboarding/)
  </Card>

  <Card title="Track B: Web & Backend Developer" icon="open-book">
    For developers transitioning from Web (React/Vue) or Backend microservices. Read the "Mobile 100" primer on app binaries, lifecycles & signing.
    
    [Open 1.3 Non-Mobile Engineer Track ➔](/mobile/onboarding/non-mobile-engineer-guide/)
  </Card>
</CardGrid>

---

## 1.0.2 Target Framework & Workstation Setup

Select your target stack to open the step-by-step installation instructions:

<Tabs>
  <TabItem label="React Native">
    **Cross-Platform Stack:** Node.js 18+, Watchman, React Native CLI, Xcode & Android Studio.
    
    ➔ [Open 1.5 Machine Setup Guide for React Native](/mobile/onboarding/machine-setup/)
  </TabItem>
  <TabItem label="Native iOS">
    **iOS Stack:** macOS, Xcode 15+, Swift 5.10+, Swift Package Manager & CocoaPods.
    
    ➔ [Open 1.5 Machine Setup Guide for iOS](/mobile/onboarding/machine-setup/)
  </TabItem>
  <TabItem label="Native Android">
    **Android Stack:** Android Studio Hedgehog+, JDK 17, Kotlin 1.9+ & Gradle 8+.
    
    ➔ [Open 1.5 Machine Setup Guide for Android](/mobile/onboarding/machine-setup/)
  </TabItem>
</Tabs>

---

## 1.0.3 Your 4-Step Onboarding Roadmap

Follow these 4 phases to get your mobile development environment up and running smoothly:

<Steps>

1. **Understand the Ecosystem**
   Read [1.1 Platform Overview](/mobile/onboarding/platform-overview/) to learn about our team structure, governance model, and core architectural pillars.

2. **Select Your Technology Stack**
   Review [1.4 Tech Stack Selection](/mobile/onboarding/tech-stack-selection/) to determine whether React Native or Native iOS/Android fits your application requirements.

3. **Set Up Your Workstation**
   Follow the step-by-step [1.5 Machine Setup Guide](/mobile/onboarding/machine-setup/) for macOS or Windows to install Xcode, Android Studio, Node.js, and root certificates.

4. **Complete Your Checklist & Submit Your First PR**
   Use the [1.2 New Mobile Engineer Track](/mobile/onboarding/new-engineer-onboarding/) checklist to verify your local build and submit your first pull request via Bitrise CI/CD.

</Steps>

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
