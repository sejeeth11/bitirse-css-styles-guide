---
// src/components/HomeCard.astro
// Mobile Engineering Portal Dashboard
---

<div class="portal-container border rounded-xl p-5 md:p-6 shadow-xs max-w-full space-y-6">

  <!-- 1. TOP BREADCRUMB -->
  <div class="flex items-center gap-1.5 text-xs portal-subtitle">
    <a href="/getting-started/overview/" class="hover:underline font-medium" style="color: #008544;">Home</a>
    <span>&gt;</span>
    <span class="font-semibold portal-title">Mobile Engineering Portal</span>
  </div>

  <!-- 2. MAIN PAGE HEADER -->
  <div class="flex items-center gap-3.5 pb-2 border-b portal-divider">
    <div class="w-12 h-12 rounded-xl flex items-center justify-center shrink-0" style="background-color: rgba(0, 133, 68, 0.1); color: #008544;">
      <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="14" height="20" x="5" y="2" rx="2" ry="2"/><path d="M12 18h.01"/></svg>
    </div>
    <div>
      <h1 class="text-xl font-bold portal-title">Mobile Engineering Portal</h1>
      <div class="w-12 h-1 rounded-full my-1" style="background-color: #008544;"></div>
      <p class="text-xs portal-subtitle">Your complete guide to building, deploying and scaling mobile solutions.</p>
    </div>
  </div>

  <!-- 3. SECTION TITLE & VIEW ALL -->
  <div class="flex items-center justify-between">
    <div>
      <h2 class="text-base font-bold portal-title">Quick Access Modules</h2>
      <p class="text-xs portal-subtitle">Explore key platform modules. Click any sub-topic or "View All" to get started.</p>
    </div>
    <a href="/getting-started/overview/" class="text-xs font-semibold px-3 py-1.5 rounded-lg border hover:underline transition-all" style="color: #008544; background-color: rgba(0, 133, 68, 0.08); border-color: rgba(0, 133, 68, 0.25);">View All Modules ➔</a>
  </div>

  <!-- 4. 3-COLUMN CARDS GRID (ALL 8 MODULES) -->
  <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
    
    <!-- Module 1 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #008544;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09z"/><path d="m12 15-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z"/><path d="M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0"/><path d="M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">1. Onboarding & Developer Journeys</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Platform ecosystem, workstation setup, fast-track checklists, and framework selection.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/getting-started/overview/" class="sublink-pill">1.1 Overview</a>
          <a href="/getting-started/new-engineer-onboarding/" class="sublink-pill">1.2 Checklist</a>
          <a href="/getting-started/non-mobile-engineer-guide/" class="sublink-pill">1.3 Non-Mobile</a>
          <a href="/getting-started/tech-stack-selection/" class="sublink-pill">1.4 Tech Stack</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/getting-started/overview/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 2 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #059669;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="7" height="7" x="3" y="3" rx="1"/><rect width="7" height="7" x="14" y="3" rx="1"/><rect width="7" height="7" x="14" y="14" rx="1"/><rect width="7" height="7" x="3" y="14" rx="1"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">2. Architecture & Platform Standards</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Clean architecture layers, Circuit Breaker resilience, feature flags, and branching rules.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/architecture/overview/" class="sublink-pill">2.1 Architecture</a>
          <a href="/architecture/circuit-breaker/" class="sublink-pill">2.2 Resilience</a>
          <a href="/architecture/feature-flags/" class="sublink-pill">2.3 Feature Flags</a>
          <a href="/architecture/git-rules/" class="sublink-pill">2.4 Git Rules</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/architecture/overview/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 3 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #7c3aed;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">3. Development Platforms & SDKs</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Android, iOS, React Native catalogs, shared libraries, and app core foundations.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/platforms/android/" class="sublink-pill">3.1 Android SDK</a>
          <a href="/platforms/ios/" class="sublink-pill">3.2 iOS SDK</a>
          <a href="/platforms/react-native/" class="sublink-pill">3.3 RN Packages</a>
          <a href="/platforms/essentials/" class="sublink-pill">3.5 Essentials</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/platforms/android/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 4 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #ea580c;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12a9 9 0 0 0-9-9 9.75 9.75 0 0 0-6.74 2.74L3 8"/><path d="M3 3v5h5"/><path d="M3 12a9 9 0 0 0 9 9 9.75 9.75 0 0 0 6.74-2.74L21 16"/><path d="M16 16h5v5"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">4. Build & Release Kit (CI/CD)</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Bitrise pipelines, camp.yml spec reference, Danger PR inspection, and automated builds.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/cicd/overview/" class="sublink-pill">4.1 Build Kit</a>
          <a href="/cicd/camp-spec/" class="sublink-pill">4.3 CAMP Spec</a>
          <a href="/cicd/bitrise/" class="sublink-pill">4.4 Bitrise CI</a>
          <a href="/cicd/danger-bot/" class="sublink-pill">4.5 Danger Bot</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/cicd/overview/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 5 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #0d9488;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"/><path d="m9 12 2 2 4-4"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">5. Observability, Security & Services</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Push notifications, Datadog RUM telemetry, security checklist, and data wipe protocol.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/services/push-notifications/" class="sublink-pill">5.1 Push Notify</a>
          <a href="/services/datadog-rum/" class="sublink-pill">5.2 Datadog RUM</a>
          <a href="/services/security-checklist/" class="sublink-pill">5.3 Security</a>
          <a href="/services/data-wipe/" class="sublink-pill">5.4 Data Wipe</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/services/push-notifications/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 6 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #db2777;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m7.5 4.27 9 5.15"/><path d="M21 8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16Z"/><path d="m3.3 7 8.7 5 8.7-5"/><path d="M12 22V12"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">6. App Store & Distribution</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Enterprise App Store, Google Play deployment, Apple App Store publishing, and signing.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/store/enterprise-store/" class="sublink-pill">6.1 Ent Store</a>
          <a href="/store/google-play/" class="sublink-pill">6.2 Play Store</a>
          <a href="/store/apple-app-store/" class="sublink-pill">6.3 App Store</a>
          <a href="/store/certificates/" class="sublink-pill">6.4 Certs & Signing</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/store/enterprise-store/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 7 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #4f46e5;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="16" height="16" x="4" y="4" rx="2"/><rect width="6" height="6" x="9" y="9" rx="1"/><path d="M15 2v2"/><path d="M15 20v2"/><path d="M2 15h2"/><path d="M2 9h2"/><path d="M20 15h2"/><path d="M20 9h2"/><path d="M9 2v2"/><path d="M9 20v2"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">7. GenAI & Developer Productivity</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Machine-readable index (llms.txt), AI rules (.cursorrules), FAQs, and prompts.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/genai/llms-txt/" class="sublink-pill">7.1 llms.txt</a>
          <a href="/genai/cursorrules/" class="sublink-pill">7.2 AI Rules</a>
          <a href="/genai/faqs/" class="sublink-pill">7.3 FAQs</a>
          <a href="/genai/prompts/" class="sublink-pill">7.4 Prompts</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/genai/llms-txt/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 8 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #0284c7;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 14h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-7a9 9 0 0 1 18 0v7a2 2 0 0 1-2 2h-1a2 2 0 0 1-2-2v-3a2 2 0 0 1 2-2h3"/></svg>
        </div>
        <h3 class="text-xs font-bold portal-title leading-snug">8. Support & Troubleshooting Hub</h3>
        <p class="text-[11px] portal-subtitle mt-0.5 mb-2.5">Support policies, MS Teams channel, troubleshooting matrix, RFC process, and noticeboard.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/support/teams-channel/" class="sublink-pill">8.1 Teams Support</a>
          <a href="/support/troubleshooting/" class="sublink-pill">8.2 Troubleshoot</a>
          <a href="/support/rfc-process/" class="sublink-pill">8.3 RFC Process</a>
          <a href="/support/noticeboard/" class="sublink-pill">8.4 Noticeboard</a>
        </div>
      </div>
      <div class="pt-2 border-t portal-divider flex items-center justify-end">
        <a href="/support/teams-channel/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

  </div>

  <!-- 5. PERFECTLY ALIGNED 2-TIER BOTTOM HERO CARD ("Start from here") -->
  <div class="hero-banner space-y-4 mt-8">
    
    <!-- Top Row: Icon + Title + CTA Button -->
    <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4">
      <div class="flex items-center gap-3">
        <div class="w-10 h-10 rounded-xl text-white flex items-center justify-center shrink-0 shadow-2xs" style="background-color: #008544;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><polygon points="16.24 7.76 14.12 14.12 7.76 16.24 9.88 9.88 16.24 7.76"/></svg>
        </div>
        <div>
          <h3 class="text-sm font-bold portal-title">Start from Here — Onboarding Journey</h3>
          <p class="text-xs portal-subtitle">Complete the 4 fast-track phases to onboard to the mobile platform.</p>
        </div>
      </div>
      <a href="/getting-started/new-engineer-onboarding/" class="text-xs font-bold px-4 py-2 rounded-lg text-white shadow-xs hover:opacity-95 transition-opacity whitespace-nowrap shrink-0" style="background-color: #008544;">
        Go to Onboarding Journey ➔
      </a>
    </div>

    <!-- Bottom Row: 4 Equal-Width Step Cards in a 4-Column Grid -->
    <div class="grid grid-cols-2 sm:grid-cols-4 gap-2 pt-3 border-t portal-divider">
      
      <div class="stepper-pill p-2 rounded-lg flex items-center gap-2">
        <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">1</span>
        <div class="text-[11px] leading-tight">
          <span class="font-bold block portal-title">Access & Tools</span>
          <span class="text-[10px] portal-subtitle">GitHub & Jira</span>
        </div>
      </div>

      <div class="stepper-pill p-2 rounded-lg flex items-center gap-2">
        <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">2</span>
        <div class="text-[11px] leading-tight">
          <span class="font-bold block portal-title">Workstation</span>
          <span class="text-[10px] portal-subtitle">IDE & SDKs</span>
        </div>
      </div>

      <div class="stepper-pill p-2 rounded-lg flex items-center gap-2">
        <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">3</span>
        <div class="text-[11px] leading-tight">
          <span class="font-bold block portal-title">Architecture</span>
          <span class="text-[10px] portal-subtitle">Rules & Git</span>
        </div>
      </div>

      <div class="stepper-pill p-2 rounded-lg flex items-center gap-2">
        <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">4</span>
        <div class="text-[11px] leading-tight">
          <span class="font-bold block portal-title">First PR</span>
          <span class="text-[10px] portal-subtitle">CI Build</span>
        </div>
      </div>

    </div>

  </div>

</div>

<style>
  /* ----------------------------------------------------
     LIGHT MODE DEFAULTS
     ---------------------------------------------------- */
  .squircle {
    width: 2.25rem;
    height: 2.25rem;
    border-radius: 0.625rem;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #ffffff;
    flex-shrink: 0;
  }
  .portal-container {
    background-color: #ffffff;
    border-color: #e2e8f0;
    color: #0f172a;
  }
  .portal-title { color: #0f172a; }
  .portal-subtitle { color: #64748b; }
  .portal-divider { border-color: #f1f5f9; }

  .portal-card {
    border: 1px solid #e2e8f0;
    border-radius: 0.75rem;
    padding: 1rem 1.125rem;
    background-color: #ffffff;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: all 0.2s ease-in-out;
    box-shadow: 0 1px 3px rgba(0,0,0,0.05);
  }
  .portal-card:hover {
    transform: translateY(-2px);
    border-color: #008544 !important;
    box-shadow: 0 4px 14px rgba(0, 133, 68, 0.15);
  }

  .sublink-pill {
    font-size: 0.68rem;
    font-weight: 600;
    color: #475569;
    padding: 0.35rem 0.45rem;
    border-radius: 0.375rem;
    background-color: #f8fafc;
    border: 1px solid #e2e8f0;
    transition: all 0.15s ease;
    text-decoration: none;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    display: block;
  }
  .sublink-pill:hover {
    color: #008544 !important;
    border-color: rgba(0, 133, 68, 0.4) !important;
    background-color: rgba(0, 133, 68, 0.05) !important;
  }

  .hero-banner {
    background-color: rgba(0, 133, 68, 0.04);
    border: 1px solid rgba(0, 133, 68, 0.25);
    border-left: 4px solid #008544;
    border-radius: 0.875rem;
    padding: 1.25rem 1.5rem;
  }

  .stepper-pill {
    background-color: #ffffff;
    border: 1px solid #e2e8f0;
    color: #334155;
  }

  /* ----------------------------------------------------
     DARK MODE OVERRIDES (Astro Starlight & Tailwind)
     ---------------------------------------------------- */
  :global([data-theme="dark"]) .portal-container,
  :global(.dark) .portal-container,
  :global(.theme-dark) .portal-container {
    background-color: #0f172a !important;
    border-color: #1e293b !important;
    color: #f8fafc !important;
  }

  :global([data-theme="dark"]) .portal-title,
  :global(.dark) .portal-title,
  :global(.theme-dark) .portal-title {
    color: #ffffff !important;
  }

  :global([data-theme="dark"]) .portal-subtitle,
  :global(.dark) .portal-subtitle,
  :global(.theme-dark) .portal-subtitle {
    color: #94a3b8 !important;
  }

  :global([data-theme="dark"]) .portal-divider,
  :global(.dark) .portal-divider,
  :global(.theme-dark) .portal-divider {
    border-color: #1e293b !important;
  }

  :global([data-theme="dark"]) .portal-card,
  :global(.dark) .portal-card,
  :global(.theme-dark) .portal-card {
    background-color: #1e293b !important;
    border-color: #334155 !important;
  }

  :global([data-theme="dark"]) .sublink-pill,
  :global(.dark) .sublink-pill,
  :global(.theme-dark) .sublink-pill {
    color: #cbd5e1 !important;
    background-color: #0f172a !important;
    border-color: #334155 !important;
  }

  :global([data-theme="dark"]) .hero-banner,
  :global(.dark) .hero-banner,
  :global(.theme-dark) .hero-banner {
    background-color: rgba(0, 133, 68, 0.12) !important;
    border-color: rgba(0, 133, 68, 0.35) !important;
    border-left: 4px solid #008544 !important;
  }

  :global([data-theme="dark"]) .stepper-pill,
  :global(.dark) .stepper-pill,
  :global(.theme-dark) .stepper-pill {
    background-color: #1e293b !important;
    border-color: #334155 !important;
    color: #f1f5f9 !important;
  }
</style>
