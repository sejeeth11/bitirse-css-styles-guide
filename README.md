---
title: 1.0 Welcome & Quick Start
description: The central starting hub and onboarding roadmap for all engineers joining the Mobile Engineering Platform.
sidebar:
  order: 1
---

import { Aside, Steps } from '@astrojs/starlight/components';

<Aside type="tip">
👋 **Welcome to the Mobile Engineering Platform!** Follow the interactive decision flowchart and 4-step onboarding roadmap below to set up your workstation, obtain repository access, and land your first pull request smoothly.
</Aside>

## 1.0.1 Interactive Onboarding Decision Flowchart

Use this decision flowchart to determine your exact onboarding path based on your role background and target tech stack:

<pre class="mermaid">
flowchart TD
    Start(["🚀 Join Mobile Team"]) ==> Q1{"Are you a Web or Backend Dev?"}
    
    Q1 -- "Yes (New to Mobile)" --> TrackA["Read 1.3 Non-Mobile Track ('Mobile 100')"]
    Q1 -- "No (Mobile Engineer)" --> Q2{"What is your target stack?"}
    
    TrackA ==> Q2
    
    Q2 -- "React Native" --> SetupRN["1.5 Setup Node.js, Watchman, Xcode & AS"]
    Q2 -- "Native iOS" --> SetupIOS["1.5 Setup macOS, Xcode & CocoaPods"]
    Q2 -- "Native Android" --> SetupAndroid["1.5 Setup Android Studio & JDK 17"]
    
    SetupRN ==> Verification["Run Local Verification Build"]
    SetupIOS ==> Verification
    SetupAndroid ==> Verification
    
    Verification ==> TrackB["1.2 Follow New Mobile Engineer Track"]
    TrackB ==> Done(["🎉 Submit & Merge First PR"])
</pre>

---

## 1.0.2 Your 4-Step Onboarding Roadmap

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

## 1.0.3 Community & Support Channels

Need help during setup? Connect with the mobile platform team:

- **MS Teams Support Channel:** `#mobile-engineering-support`
- **Architecture Guild Meeting:** Thursdays @ 10:00 AM EST
- **Documentation RFCs:** Submit an RFC or PR to update this portal.

{/* Client-side Mermaid Hydration Script */}
<script is:inline src="https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.min.js"></script>
<script is:inline>
  if (typeof window !== 'undefined') {
    window.addEventListener('DOMContentLoaded', () => {
      mermaid.initialize({
        startOnLoad: true,
        theme: 'default',
        flowchart: { useMaxWidth: true, htmlLabels: true, curve: 'basis' }
      });
      mermaid.contentLoaded();
    });
  }
</script>
