---
// src/components/HomeCard.astro
// Mobile Engineering Portal Dashboard
---

<div class="bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-xl p-5 md:p-6 shadow-xs max-w-full space-y-6">

  <!-- 1. TOP BREADCRUMB -->
  <div class="flex items-center gap-1.5 text-xs text-slate-500 dark:text-slate-400">
    <a href="/getting-started/overview/" class="hover:underline font-medium" style="color: #008544;">Home</a>
    <span>&gt;</span>
    <span class="font-semibold text-slate-800 dark:text-slate-200">Mobile Engineering Portal</span>
  </div>

  <!-- 2. MAIN PAGE HEADER -->
  <div class="flex items-center gap-3.5 pb-2 border-b border-slate-100 dark:border-slate-800">
    <div class="w-12 h-12 rounded-xl flex items-center justify-center shrink-0" style="background-color: rgba(0, 133, 68, 0.1); color: #008544;">
      <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="14" height="20" x="5" y="2" rx="2" ry="2"/><path d="M12 18h.01"/></svg>
    </div>
    <div>
      <h1 class="text-xl font-bold text-slate-900 dark:text-white">Mobile Engineering Portal</h1>
      <div class="w-12 h-1 rounded-full my-1" style="background-color: #008544;"></div>
      <p class="text-xs text-slate-500 dark:text-slate-400">Your complete guide to building, deploying and scaling mobile solutions.</p>
    </div>
  </div>

  <!-- 3. SECTION TITLE & VIEW ALL -->
  <div class="flex items-center justify-between">
    <div>
      <h2 class="text-base font-bold text-slate-900 dark:text-white">Quick Access Modules</h2>
      <p class="text-xs text-slate-500 dark:text-slate-400">Explore key platform modules. Click any sub-topic or "View All" to get started.</p>
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
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">1. Onboarding & Developer Journeys</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Platform ecosystem, workstation setup, fast-track checklists, and framework selection.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/getting-started/overview/" class="sublink-pill">1.1 Overview</a>
          <a href="/getting-started/new-engineer-onboarding/" class="sublink-pill">1.2 Checklist</a>
          <a href="/getting-started/non-mobile-engineer-guide/" class="sublink-pill">1.3 Non-Mobile</a>
          <a href="/getting-started/tech-stack-selection/" class="sublink-pill">1.4 Tech Stack</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/getting-started/overview/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 2 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #059669;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="7" height="7" x="3" y="3" rx="1"/><rect width="7" height="7" x="14" y="3" rx="1"/><rect width="7" height="7" x="14" y="14" rx="1"/><rect width="7" height="7" x="3" y="14" rx="1"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">2. Architecture & Platform Standards</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Clean architecture layers, Circuit Breaker resilience, feature flags, and branching rules.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/architecture/overview/" class="sublink-pill">2.1 Architecture</a>
          <a href="/architecture/circuit-breaker/" class="sublink-pill">2.2 Resilience</a>
          <a href="/architecture/feature-flags/" class="sublink-pill">2.3 Feature Flags</a>
          <a href="/architecture/git-rules/" class="sublink-pill">2.4 Git Rules</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/architecture/overview/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 3 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #7c3aed;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">3. Development Platforms & SDKs</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Android, iOS, React Native catalogs, shared libraries, and app core foundations.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/platforms/android/" class="sublink-pill">3.1 Android SDK</a>
          <a href="/platforms/ios/" class="sublink-pill">3.2 iOS SDK</a>
          <a href="/platforms/react-native/" class="sublink-pill">3.3 RN Packages</a>
          <a href="/platforms/essentials/" class="sublink-pill">3.5 Essentials</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/platforms/android/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 4 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #ea580c;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12a9 9 0 0 0-9-9 9.75 9.75 0 0 0-6.74 2.74L3 8"/><path d="M3 3v5h5"/><path d="M3 12a9 9 0 0 0 9 9 9.75 9.75 0 0 0 6.74-2.74L21 16"/><path d="M16 16h5v5"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">4. Build & Release Kit (CI/CD)</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Bitrise pipelines, camp.yml spec reference, Danger PR inspection, and automated builds.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/cicd/overview/" class="sublink-pill">4.1 Build Kit</a>
          <a href="/cicd/camp-spec/" class="sublink-pill">4.3 CAMP Spec</a>
          <a href="/cicd/bitrise/" class="sublink-pill">4.4 Bitrise CI</a>
          <a href="/cicd/danger-bot/" class="sublink-pill">4.5 Danger Bot</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/cicd/overview/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 5 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #0d9488;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"/><path d="m9 12 2 2 4-4"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">5. Observability, Security & Services</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Push notifications, Datadog RUM telemetry, security checklist, and data wipe protocol.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/services/push-notifications/" class="sublink-pill">5.1 Push Notify</a>
          <a href="/services/datadog-rum/" class="sublink-pill">5.2 Datadog RUM</a>
          <a href="/services/security-checklist/" class="sublink-pill">5.3 Security</a>
          <a href="/services/data-wipe/" class="sublink-pill">5.4 Data Wipe</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/services/push-notifications/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 6 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #db2777;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m7.5 4.27 9 5.15"/><path d="M21 8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16Z"/><path d="m3.3 7 8.7 5 8.7-5"/><path d="M12 22V12"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">6. App Store & Distribution</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Enterprise App Store, Google Play deployment, Apple App Store publishing, and signing.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/store/enterprise-store/" class="sublink-pill">6.1 Ent Store</a>
          <a href="/store/google-play/" class="sublink-pill">6.2 Play Store</a>
          <a href="/store/apple-app-store/" class="sublink-pill">6.3 App Store</a>
          <a href="/store/certificates/" class="sublink-pill">6.4 Certs & Signing</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/store/enterprise-store/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 7 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #4f46e5;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="16" height="16" x="4" y="4" rx="2"/><rect width="6" height="6" x="9" y="9" rx="1"/><path d="M15 2v2"/><path d="M15 20v2"/><path d="M2 15h2"/><path d="M2 9h2"/><path d="M20 15h2"/><path d="M20 9h2"/><path d="M9 2v2"/><path d="M9 20v2"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">7. GenAI & Developer Productivity</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Machine-readable index (llms.txt), AI rules (.cursorrules), FAQs, and prompts.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/genai/llms-txt/" class="sublink-pill">7.1 llms.txt</a>
          <a href="/genai/cursorrules/" class="sublink-pill">7.2 AI Rules</a>
          <a href="/genai/faqs/" class="sublink-pill">7.3 FAQs</a>
          <a href="/genai/prompts/" class="sublink-pill">7.4 Prompts</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/genai/llms-txt/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

    <!-- Module 8 -->
    <div class="portal-card">
      <div>
        <div class="squircle mb-2" style="background-color: #0284c7;">
          <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 14h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-7a9 9 0 0 1 18 0v7a2 2 0 0 1-2 2h-1a2 2 0 0 1-2-2v-3a2 2 0 0 1 2-2h3"/></svg>
        </div>
        <h3 class="text-xs font-bold text-slate-900 dark:text-white leading-snug">8. Support & Troubleshooting Hub</h3>
        <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-0.5 mb-2.5">Support policies, MS Teams channel, troubleshooting matrix, RFC process, and noticeboard.</p>
        
        <div class="grid grid-cols-2 gap-1.5 mb-3">
          <a href="/support/teams-channel/" class="sublink-pill">8.1 Teams Support</a>
          <a href="/support/troubleshooting/" class="sublink-pill">8.2 Troubleshoot</a>
          <a href="/support/rfc-process/" class="sublink-pill">8.3 RFC Process</a>
          <a href="/support/noticeboard/" class="sublink-pill">8.4 Noticeboard</a>
        </div>
      </div>
      <div class="pt-2 border-t border-slate-100 dark:border-slate-800 flex items-center justify-end">
        <a href="/support/teams-channel/" class="text-xs font-bold hover:underline" style="color: #008544;">View All ➔</a>
      </div>
    </div>

  </div>

  <!-- 5. FINAL ONBOARDING HERO CARD ("Start from here") -->
  <div class="relative overflow-hidden rounded-2xl border border-slate-200/90 dark:border-slate-800 bg-gradient-to-r from-emerald-950/5 via-slate-50 to-emerald-900/5 dark:from-slate-900 dark:to-slate-800 p-6 shadow-xs mt-8 border-l-4" style="border-left-color: #008544;">
    
    <!-- Top Micro Badge -->
    <div class="flex items-center justify-between mb-4">
      <div class="inline-flex items-center gap-2 px-2.5 py-1 rounded-full text-[11px] font-bold tracking-wide uppercase" style="background-color: rgba(0, 133, 68, 0.12); color: #008544;">
        <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
        Engineer Onboarding Roadmap
      </div>
      <span class="text-[11px] font-semibold text-slate-400">4 Quick Steps</span>
    </div>

    <div class="flex flex-col lg:flex-row items-start lg:items-center justify-between gap-6">
      
      <!-- Left Content -->
      <div class="flex items-start gap-4 max-w-xl">
        <div class="w-12 h-12 rounded-xl text-white flex items-center justify-center shrink-0 shadow-xs" style="background-color: #008544;">
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><polygon points="16.24 7.76 14.12 14.12 7.76 16.24 9.88 9.88 16.24 7.76"/></svg>
        </div>
        <div>
          <h3 class="text-base font-extrabold text-slate-900 dark:text-white tracking-tight">New to Mobile Engineering Platform?</h3>
          <p class="text-xs text-slate-600 dark:text-slate-300 mt-1 leading-relaxed">Follow our streamlined 4-phase developer journey to configure your environment, join internal slack/teams channels, and land your first pull request smoothly.</p>
        </div>
      </div>

      <!-- Right Timeline Stepper + CTA Button -->
      <div class="flex flex-col sm:flex-row items-stretch sm:items-center gap-4 w-full lg:w-auto shrink-0">
        
        <!-- Connected Stepper Pills -->
        <div class="grid grid-cols-2 sm:grid-cols-4 gap-2 text-xs w-full">
          
          <div class="bg-white dark:bg-slate-800 border border-slate-200/80 dark:border-slate-700 rounded-lg p-2 flex items-center gap-2 shadow-2xs">
            <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">1</span>
            <div class="leading-none">
              <p class="text-[10px] font-bold text-slate-900 dark:text-white">Access</p>
              <p class="text-[9px] text-slate-400">GitHub & Jira</p>
            </div>
          </div>

          <div class="bg-white dark:bg-slate-800 border border-slate-200/80 dark:border-slate-700 rounded-lg p-2 flex items-center gap-2 shadow-2xs">
            <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">2</span>
            <div class="leading-none">
              <p class="text-[10px] font-bold text-slate-900 dark:text-white">Setup</p>
              <p class="text-[9px] text-slate-400">IDE & SDKs</p>
            </div>
          </div>

          <div class="bg-white dark:bg-slate-800 border border-slate-200/80 dark:border-slate-700 rounded-lg p-2 flex items-center gap-2 shadow-2xs">
            <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">3</span>
            <div class="leading-none">
              <p class="text-[10px] font-bold text-slate-900 dark:text-white">Standards</p>
              <p class="text-[9px] text-slate-400">Arch & Git</p>
            </div>
          </div>

          <div class="bg-white dark:bg-slate-800 border border-slate-200/80 dark:border-slate-700 rounded-lg p-2 flex items-center gap-2 shadow-2xs">
            <span class="w-5 h-5 rounded-full text-white text-[10px] flex items-center justify-center font-bold shrink-0" style="background-color: #008544;">4</span>
            <div class="leading-none">
              <p class="text-[10px] font-bold text-slate-900 dark:text-white">First PR</p>
              <p class="text-[9px] text-slate-400">CI Build</p>
            </div>
          </div>

        </div>

        <!-- Action Button -->
        <a href="/getting-started/new-engineer-onboarding/" class="group text-center text-xs font-bold px-5 py-3 rounded-xl text-white shadow-xs hover:shadow-md transition-all flex items-center justify-center gap-2 whitespace-nowrap shrink-0" style="background-color: #008544;">
          Start Onboarding
          <span class="group-hover:translate-x-1 transition-transform inline-block">➔</span>
        </a>

      </div>

    </div>
  </div>

</div>

<style>
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
  :global(.dark) .portal-card {
    background-color: #0f172a;
    border-color: #1e293b;
  }
  .portal-card:hover {
    transform: translateY(-2px);
    border-color: #008544;
    box-shadow: 0 4px 14px rgba(0, 133, 68, 0.12);
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
  :global(.dark) .sublink-pill {
    color: #cbd5e1;
    background-color: #1e293b;
    border-color: #334155;
  }
  .sublink-pill:hover {
    color: #008544 !important;
    border-color: rgba(0, 133, 68, 0.4);
    background-color: rgba(0, 133, 68, 0.05);
  }
</style>
