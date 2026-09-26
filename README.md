

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
