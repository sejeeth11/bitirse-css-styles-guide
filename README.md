---
// HomeCard.astro - Single Self-Contained File (No external CSS required!)

const modules = [
  {
    id: 1,
    title: '1. Onboarding & Developer Journeys',
    description: 'Get started with platform overview, setup, and your development journey.',
    link: '/01-onboarding/1-1-overview-and-ecosystem/',
    iconBgClass: 'bg-squircle-blue',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09z"/><path d="m12 15-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z"/><path d="M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0"/><path d="M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5"/></svg>`
  },
  {
    id: 2,
    title: '2. Architecture & Platform Standards',
    description: 'Learn our architecture principles, security, branching, and best practices.',
    link: '/02-architecture/2-1-cargill-architecture/',
    iconBgClass: 'bg-squircle-emerald',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="7" height="7" x="3" y="3" rx="1"/><rect width="7" height="7" x="14" y="3" rx="1"/><rect width="7" height="7" x="14" y="14" rx="1"/><rect width="7" height="7" x="3" y="14" rx="1"/></svg>`
  },
  {
    id: 3,
    title: '3. Development Platforms & SDKs',
    description: 'Explore platform-specific guidelines, internal SDKs and app foundations.',
    link: '/03-development-platforms/3-1-android-guidelines-sdks/',
    iconBgClass: 'bg-squircle-purple',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>`
  },
  {
    id: 4,
    title: '4. Build & Release Kit (CI/CD)',
    description: 'Automate builds, tests, and releases with our CI/CD pipeline and build kit.',
    link: '/04-cicd/4-3-camp-spec-reference/',
    iconBgClass: 'bg-squircle-orange',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12a9 9 0 0 0-9-9 9.75 9.75 0 0 0-6.74 2.74L3 8"/><path d="M3 3v5h5"/><path d="M3 12a9 9 0 0 0 9 9 9.75 9.75 0 0 0 6.74-2.74L21 16"/><path d="M16 16h5v5"/></svg>`
  },
  {
    id: 5,
    title: '5. Observability, Security & Platform Services',
    description: 'Set up push notifications, analytics, security and platform services.',
    link: '/05-services/5-1-push-notifications/',
    iconBgClass: 'bg-squircle-teal',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"/><path d="m9 12 2 2 4-4"/></svg>`
  },
  {
    id: 6,
    title: '6. App Store & Distribution',
    description: 'Publish and distribute your apps across enterprise, Play Store and App Store.',
    link: '/06-app-store/6-1-enterprise-app-store/',
    iconBgClass: 'bg-squircle-pink',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m7.5 4.27 9 5.15"/><path d="M21 8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16Z"/><path d="m3.3 7 8.7 5 8.7-5"/><path d="M12 22V12"/></svg>`
  },
  {
    id: 7,
    title: '7. GenAI & Developer Productivity',
    description: 'Leverage AI, documentation and knowledge base to work smarter.',
    link: '/07-genai/7-1-machine-readable-index/',
    iconBgClass: 'bg-squircle-indigo',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="16" height="16" x="4" y="4" rx="2"/><rect width="6" height="6" x="9" y="9" rx="1"/><path d="M15 2v2"/><path d="M15 20v2"/><path d="M2 15h2"/><path d="M2 9h2"/><path d="M20 15h2"/><path d="M20 9h2"/><path d="M9 2v2"/><path d="M9 20v2"/></svg>`
  },
  {
    id: 8,
    title: '8. Support & Troubleshooting Hub',
    description: 'Get help, find solutions, and report issues with our support ecosystem.',
    link: '/08-support/8-1-support-policies/',
    iconBgClass: 'bg-squircle-sky',
    iconSvg: `<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 14h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-7a9 9 0 0 1 18 0v7a2 2 0 0 1-2 2h-1a2 2 0 0 1-2-2v-3a2 2 0 0 1 2-2h3"/></svg>`
  }
];

const steps = [
  { id: 1, title: 'Get Access & Entitlements', badgeBg: 'bg-emerald-600' },
  { id: 2, title: 'Setup Your Environment', badgeBg: 'bg-blue-600' },
  { id: 3, title: 'Learn the Platform', badgeBg: 'bg-purple-600' },
  { id: 4, title: 'Make Your First PR', badgeBg: 'bg-orange-600' }
];
---

<div class="portal-dashboard-container">
  <!-- Top Breadcrumb -->
  <nav class="portal-breadcrumb">
    <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m3 9 9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
    <a href="/">Home</a>
    <span>&gt;</span>
    <span>Mobile Engineering Portal</span>
  </nav>

  <!-- Main Header -->
  <div class="portal-header-wrapper">
    <div class="portal-header-icon">
      <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="14" height="20" x="5" y="2" rx="2" ry="2"/><path d="M12 18h.01"/></svg>
    </div>
    <div class="portal-header-content">
      <h1 class="portal-header-title">Mobile Engineering Portal</h1>
      <div class="portal-green-bar"></div>
      <p class="portal-header-subtitle">Your complete guide to building, deploying and scaling mobile solutions.</p>
    </div>
  </div>

  <!-- Quick Access Section -->
  <div style="margin-bottom: 2.5rem;">
    <div class="portal-section-header">
      <div class="portal-section-title-box">
        <h2>Quick Access</h2>
        <p>Explore the key areas of the mobile engineering platform. Click any card to get started.</p>
      </div>
      <a href="/01-onboarding/1-1-overview-and-ecosystem/" class="portal-btn-view-all">
        <span>View All Modules</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
      </a>
    </div>

    <!-- 3-Column Cards Grid -->
    <div class="portal-modules-grid">
      {modules.map((item) => (
        <a href={item.link} class="portal-card group">
          <div class="portal-card-body">
            <div class={`icon-squircle ${item.iconBgClass}`}>
              <Fragment set:html={item.iconSvg} />
            </div>
            <h3 class="portal-card-title">{item.title}</h3>
            <p class="portal-card-desc">{item.description}</p>
          </div>
          <div class="portal-card-link">
            <span>View Details</span>
            <svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
          </div>
        </a>
      ))}
    </div>
  </div>

  <!-- Start from here Hero Banner -->
  <div class="portal-hero-banner">
    <div style="display: flex; align-items: flex-start; gap: 1.25rem; max-width: 42rem;">
      <div style="width: 3.5rem; height: 3.5rem; border-radius: 9999px; background-color: #2563eb; color: #fff; display: flex; align-items: center; justify-content: center; flex-shrink: 0; box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1);">
        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><polygon points="16.24 7.76 14.12 14.12 7.76 16.24 9.88 9.88 16.24 7.76"/></svg>
      </div>
      <div>
        <h3 style="font-size: 1.25rem; font-weight: 800; margin: 0 0 0.5rem 0;">Start from here</h3>
        <p style="font-size: 0.75rem; font-weight: 600; margin-bottom: 0.5rem;">Welcome to the <strong>Mobile Platform Team!</strong></p>
        <p style="font-size: 0.75rem; line-height: 1.6; margin-bottom: 1.25rem;">This onboarding guide provides a structured path for new mobile engineers to get started quickly and confidently. Follow each phase to obtain required access, set up your development environment, learn the platform architecture, configure developer tooling, and submit your first Pull Request.</p>
        <a href="/01-onboarding/1-1-overview-and-ecosystem/" class="portal-btn-primary">
          <span>Go to Onboarding Journey</span>
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
        </a>
      </div>
    </div>
    <div class="portal-steps-list">
      {steps.map((step) => (
        <div class="portal-step-item">
          <div class={`step-number-badge ${step.badgeBg}`}>{step.id}</div>
          <span style="font-size: 0.75rem; font-weight: 600;">{step.title}</span>
        </div>
      ))}
    </div>
  </div>
</div>

<style>
  .portal-dashboard-container { max-width: 80rem; margin: 0 auto; padding: 1rem; font-family: 'Inter', system-ui, sans-serif; }
  .portal-breadcrumb { display: flex !important; align-items: center !important; gap: 0.375rem !important; font-size: 0.75rem !important; color: #64748b !important; margin-bottom: 1.5rem !important; }
  .portal-breadcrumb a { color: #2563eb !important; text-decoration: none !important; }
  .portal-header-wrapper { display: flex !important; align-items: flex-start !important; gap: 1rem !important; margin-bottom: 2rem !important; }
  .portal-header-icon { width: 3.25rem !important; height: 3.25rem !important; border-radius: 0.875rem !important; background-color: #dbeafe !important; color: #2563eb !important; display: flex !important; align-items: center !important; justify-content: center !important; flex-shrink: 0 !important; }
  .portal-header-content { display: flex !important; flex-direction: column !important; }
  .portal-header-title { font-size: 1.75rem !important; font-weight: 800 !important; color: #0f172a !important; margin: 0 0 0.35rem 0 !important; line-height: 1.25 !important; border: none !important; }
  :global([data-theme='dark']) .portal-header-title { color: #ffffff !important; }
  .portal-green-bar { width: 3rem !important; height: 0.25rem !important; background-color: #059669 !important; border-radius: 9999px !important; margin-bottom: 0.5rem !important; }
  .portal-header-subtitle { font-size: 0.925rem !important; color: #64748b !important; margin: 0 !important; }
  :global([data-theme='dark']) .portal-header-subtitle { color: #cbd5e1 !important; }
  .portal-section-header { display: flex !important; align-items: flex-end !important; justify-content: space-between !important; margin-bottom: 1.25rem !important; gap: 1rem !important; }
  .portal-section-title-box h2 { font-size: 1.25rem !important; font-weight: 700 !important; color: #0f172a !important; margin: 0 0 0.25rem 0 !important; border: none !important; }
  :global([data-theme='dark']) .portal-section-title-box h2 { color: #ffffff !important; }
  .portal-section-title-box p { font-size: 0.75rem !important; color: #64748b !important; margin: 0 !important; }
  .portal-btn-view-all { display: inline-flex !important; align-items: center !important; gap: 0.375rem !important; padding: 0.375rem 0.875rem !important; font-size: 0.75rem !important; font-weight: 600 !important; color: #2563eb !important; border: 1px solid #bfdbfe !important; border-radius: 0.5rem !important; text-decoration: none !important; white-space: nowrap !important; }
  :global([data-theme='dark']) .portal-btn-view-all { color: #38bdf8 !important; border-color: #1e3a8a !important; }
  .portal-modules-grid { display: grid !important; grid-template-columns: repeat(3, 1fr) !important; gap: 1.25rem !important; }
  @media (max-width: 1024px) { .portal-modules-grid { grid-template-columns: repeat(2, 1fr) !important; } }
  @media (max-width: 640px) { .portal-modules-grid { grid-template-columns: repeat(1, 1fr) !important; } }
  .portal-card { border: 1px solid #e2e8f0; border-radius: 0.75rem; padding: 1rem 1.125rem !important; background-color: #ffffff; display: flex !important; flex-direction: column !important; justify-content: space-between !important; min-height: 10.5rem !important; text-decoration: none !important; transition: all 0.2s ease-in-out; }
  .portal-card:hover { transform: translateY(-2px); border-color: #cbd5e1; }
  :global([data-theme='dark']) .portal-card { background-color: #1e293b; border-color: #334155; }
  .portal-card-title { font-size: 0.875rem !important; line-height: 1.25rem !important; font-weight: 700 !important; margin: 0 0 0.35rem 0 !important; color: #0f172a !important; border: none !important; }
  :global([data-theme='dark']) .portal-card-title { color: #ffffff !important; }
  .portal-card-desc { font-size: 0.75rem !important; line-height: 1.125rem !important; margin: 0 0 0.5rem 0 !important; color: #64748b !important; }
  :global([data-theme='dark']) .portal-card-desc { color: #94a3b8 !important; }
  .portal-card-link { display: inline-flex !important; align-items: center !important; gap: 0.25rem !important; font-size: 0.75rem !important; font-weight: 600 !important; color: #2563eb !important; margin-top: auto !important; }
  :global([data-theme='dark']) .portal-card-link { color: #38bdf8 !important; }
  .icon-squircle { width: 2.25rem !important; height: 2.25rem !important; border-radius: 0.625rem !important; display: flex !important; align-items: center !important; justify-content: center !important; color: #ffffff !important; margin-bottom: 0.625rem !important; }
  .bg-squircle-blue { background-color: #3b82f6; } .bg-squircle-emerald { background-color: #10b981; } .bg-squircle-purple { background-color: #8b5cf6; } .bg-squircle-orange { background-color: #f97316; } .bg-squircle-teal { background-color: #14b8a6; } .bg-squircle-pink { background-color: #ec4899; } .bg-squircle-indigo { background-color: #6366f1; } .bg-squircle-sky { background-color: #0284c7; }
  .portal-hero-banner { background: linear-gradient(to right, #eff6ff, #f0f9ff, #e0f2fe); border: 1px solid #bae6fd; border-radius: 1rem; padding: 1.75rem; display: flex; justify-content: space-between; align-items: center; gap: 2rem; margin-top: 2.5rem; }
  :global([data-theme='dark']) .portal-hero-banner { background: linear-gradient(to right, #0f172a, #1e293b); border-color: #1e3a8a; }
  .portal-steps-list { display: flex; flex-direction: column; gap: 0.625rem; width: 20rem; flex-shrink: 0; }
  .portal-step-item { display: flex; align-items: center; gap: 0.75rem; padding: 0.75rem 1rem; background-color: #ffffff; border: 1px solid #e2e8f0; border-radius: 0.75rem; }
  :global([data-theme='dark']) .portal-step-item { background-color: #1e293b; border-color: #334155; }
  .step-number-badge { width: 1.5rem; height: 1.5rem; border-radius: 9999px; color: #ffffff; font-size: 0.75rem; font-weight: 700; display: flex; align-items: center; justify-content: center; flex-shrink: 0; }
  .step-number-badge.bg-emerald-600 { background-color: #059669 !important; } .step-number-badge.bg-blue-600 { background-color: #2563eb !important; } .step-number-badge.bg-purple-600 { background-color: #9333ea !important; } .step-number-badge.bg-orange-600 { background-color: #ea580c !important; }
  .portal-btn-primary { display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.625rem 1.25rem; background-color: #2563eb; color: #ffffff !important; font-size: 0.875rem; font-weight: 600; border-radius: 0.5rem; text-decoration: none !important; }
</style>
