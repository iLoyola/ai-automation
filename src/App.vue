<template>
  <div class="min-h-screen bg-firefly-50 text-gray-900 font-sans">
    <a class="sr-only focus:not-sr-only focus:absolute focus:top-4 focus:left-4 focus:bg-white focus:px-4 focus:py-2 focus:rounded-md focus:shadow" href="#main">Skip to content</a>

    <header class="max-w-6xl mx-auto px-6 py-6 flex items-center justify-between" role="banner">
      <div class="flex items-center gap-3">
        <div class="rounded-full bg-white p-2 border border-firefly-200" aria-hidden>
          <svg width="40" height="40" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden>
            <rect width="24" height="24" rx="6" fill="#3099aa" />
            <path d="M6 12h12M12 6v12" stroke="#fff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
        <div>
          <div class="text-lg font-semibold">iLoyola</div>
          <div class="text-xs text-gray-600">Workflow Automation • AI-first</div>
        </div>
      </div>

      <nav class="hidden md:flex items-center gap-6 text-sm" aria-label="Primary">
        <a href="#services" class="hover:underline focus:outline focus:outline-2 focus:outline-offset-2 focus:outline-firefly-300 rounded">Services</a>
        <a href="#case-studies" class="hover:underline focus:outline focus:outline-2 focus:outline-offset-2 focus:outline-firefly-300 rounded">Case Studies</a>
        <a href="#about" class="hover:underline focus:outline focus:outline-2 focus:outline-offset-2 focus:outline-firefly-300 rounded">About</a>
        <a href="#contact" class="rounded-md px-4 py-2 bg-damask-500 text-white focus:ring-2 focus:ring-damask-300">Book a Call</a>
      </nav>

      <button @click="mobileOpen = !mobileOpen" :aria-expanded="mobileOpen" aria-controls="mobile-menu" class="md:hidden p-2 rounded focus:ring-2 focus:ring-firefly-300">
        <span class="sr-only">Open menu</span>
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" aria-hidden>
          <path d="M4 6h16M4 12h16M4 18h16" stroke="#264753" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </button>
    </header>

    <div id="mobile-menu" v-if="mobileOpen" class="md:hidden px-6 pb-6" role="menu">
      <a href="#services" class="block py-2">Services</a>
      <a href="#case-studies" class="block py-2">Case Studies</a>
      <a href="#about" class="block py-2">About</a>
      <a href="#contact" class="block py-2">Book a Call</a>
    </div>

    <main id="main" class="max-w-6xl mx-auto px-6 py-12" role="main">

      <section class="grid gap-8 md:grid-cols-2 items-center" aria-labelledby="hero-heading">
        <div>
          <h1 id="hero-heading" class="text-4xl md:text-5xl font-extrabold leading-tight">Automate workflows. Reduce overhead. Move faster.</h1>
          <p class="mt-4 text-lg text-gray-700">iLoyola designs and implements workflow automations — from CRM pipelines to multi-step sales funnels — so your team spends time on strategic work, not repetitive tasks.</p>

          <div class="mt-6 flex gap-4">
            <a href="#contact" class="px-6 py-3 rounded-md bg-damask-500 text-white font-medium shadow focus:ring-2 focus:ring-damask-300">Book a free call</a>
            <a href="#services" class="px-6 py-3 rounded-md border border-gray-200 focus:outline focus:outline-2 focus:outline-firefly-300">Our Services</a>
          </div>

          <ul class="mt-6 text-sm text-gray-600 space-y-1" aria-hidden>
            <li><strong>Average time to pilot:</strong> 1–3 weeks</li>
            <li><strong>Typical ROI:</strong> 3–6 months</li>
          </ul>
        </div>

        <div class="relative">
          <img
            src="https://images.unsplash.com/photo-1551434678-e076c223a692?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80"
            alt="Team collaborating on workflow automation with laptops and charts"
            class="w-full h-auto rounded-2xl shadow-lg object-cover"
            loading="lazy"
          />
          <div class="absolute inset-0 bg-gradient-to-t from-firefly-900/20 to-transparent rounded-2xl"></div>
        </div>
      </section>

      <section id="services" class="mt-16" aria-labelledby="services-heading">
        <h2 id="services-heading" class="text-2xl font-bold">Core Offering — Workflow Automation</h2>
        <p class="mt-2 text-sm text-gray-600">We specialize in automating sales, marketing, and ops workflows so teams can scale without friction.</p>

        <div class="mt-6 grid gap-6 md:grid-cols-2">
          <article tabindex="0" class="p-6 bg-white rounded-2xl shadow focus:outline focus:outline-2 focus:outline-firefly-300" aria-labelledby="crm-title">
            <h3 id="crm-title" class="font-semibold">CRM Automation</h3>
            <p class="mt-2 text-sm text-gray-700">Lead routing, scoring, opportunity creation, and automated follow-ups (HubSpot, Salesforce, Pipedrive).</p>
          </article>

          <article tabindex="0" class="p-6 bg-white rounded-2xl shadow focus:outline focus:outline-2 focus:outline-firefly-300" aria-labelledby="funnel-title">
            <h3 id="funnel-title" class="font-semibold">Sales Funnel Automation</h3>
            <p class="mt-2 text-sm text-gray-700">From landing page to closed-won: multi-step nurture flows, dynamic personalization, and conversion tracking.</p>
          </article>

          <article tabindex="0" class="p-6 bg-white rounded-2xl shadow focus:outline focus:outline-2 focus:outline-firefly-300" aria-labelledby="ops-title">
            <h3 id="ops-title" class="font-semibold">Internal Ops & Handovers</h3>
            <p class="mt-2 text-sm text-gray-700">Automated handoffs, task creation, and notifications to reduce delays and human error.</p>
          </article>

          <article tabindex="0" class="p-6 bg-white rounded-2xl shadow focus:outline focus:outline-2 focus:outline-firefly-300" aria-labelledby="tools-title">
            <h3 id="tools-title" class="font-semibold">Tooling & Integrations</h3>
            <p class="mt-2 text-sm text-gray-700">Zapier, Make, native API integrations, and custom webhooks to connect systems reliably.</p>
          </article>
        </div>
      </section>

      <section id="case-studies" class="mt-16" aria-labelledby="case-heading">
        <h2 id="case-heading" class="text-2xl font-bold">Selected Results</h2>
        <div class="mt-4 grid gap-6 md:grid-cols-2">
          <div class="p-6 bg-damask-100 rounded-2xl border">
            <div class="text-sm font-medium">Acme Logistics</div>
            <div class="mt-2 text-sm text-gray-700">Automated order handoffs and notifications — reduced manual tickets by 48%.</div>
          </div>
          <div class="p-6 bg-damask-100 rounded-2xl border">
            <div class="text-sm font-medium">BrightRetail</div>
            <div class="mt-2 text-sm text-gray-700">End-to-end lead flow and nurture — 31% more MQL → SQL conversions.</div>
          </div>
        </div>
      </section>

      <section id="about" class="mt-16 p-6 bg-white/60 rounded-2xl" aria-labelledby="about-heading">
        <h2 id="about-heading" class="text-2xl font-bold">About iLoyola</h2>
        <p class="mt-2 text-sm text-gray-700">We help scaling teams remove repetitive work with pragmatic automation. Fast pilots, clear metrics, and reliable ops.</p>
      </section>

      <section id="contact" class="mt-16" aria-labelledby="contact-heading">
        <h2 id="contact-heading" class="text-2xl font-bold">Contact</h2>
        <div class="mt-6 grid gap-6 md:grid-cols-2">
            <div class="pr-6 pl-6 bg-white rounded-2xl shadow iLoyola-contact-form h-full" style="min-height: 588px;">
                <iframe
                    src="https://api.leadconnectorhq.com/widget/form/GijA1WWv0Z92rTYuYlem"
                    style="width:100%;height:100%;border:none;border-radius:3px"
                    id="inline-GijA1WWv0Z92rTYuYlem"
                    data-layout="{'id':'INLINE'}"
                    data-trigger-type="alwaysShow"
                    data-trigger-value=""
                    data-activation-type="alwaysActivated"
                    data-activation-value=""
                    data-deactivation-type="neverDeactivate"
                    data-deactivation-value=""
                    data-form-name="iLoyola Form"
                    data-height="849"
                    data-layout-iframe-id="inline-GijA1WWv0Z92rTYuYlem"
                    data-form-id="GijA1WWv0Z92rTYuYlem"
                    title="iLoyola Form"
                        >
                </iframe>
                <script src="https://link.msgsndr.com/js/form_embed.js"></script>
            </div>
          <aside class="p-6 rounded-2xl bg-white/60 flex flex-col gap-4" aria-labelledby="get-in-touch">
            <h3 id="get-in-touch" class="text-sm font-semibold">Get in touch</h3>
            <p class="text-xs text-gray-600 mt-1">Email: <a :href="`mailto:${contactEmail}`" class="underline">{{ contactEmail }}</a></p>
            <p class="text-xs text-gray-600 mt-1">Location: Remote — Canada & US</p>

            <!-- <div>
              <h4 class="text-sm font-semibold">Free Resources</h4>
              <p class="text-xs text-gray-600 mt-1">Download our automation starter guides and templates.</p>
              <div class="mt-3 space-y-2">
                <a href="#" class="block text-xs text-damask-600 hover:underline">• CRM Automation Checklist</a>
                <a href="#" class="block text-xs text-damask-600 hover:underline">• Sales Funnel Template</a>
                <a href="#" class="block text-xs text-damask-600 hover:underline">• ROI Calculator Tool</a>
              </div>
            </div>

            <div>
              <h4 class="text-sm font-semibold">Client Testimonial</h4>
              <blockquote class="text-xs text-gray-600 mt-1 italic">
                "iLoyola automated our entire lead qualification process. We now handle 3x more leads with the same team size."
              </blockquote>
              <cite class="text-xs text-gray-500 mt-1 block">— Sarah Chen, VP Sales at TechFlow</cite>
            </div> -->
          </aside>
        </div>
      </section>

      <footer class="mt-16 py-8 text-center text-sm text-gray-600" role="contentinfo">© {{ year }} iLoyola — Workflow Automation & AI</footer>
    </main>

    <a :href="calendly" target="_blank" rel="noreferrer" class="fixed right-6 bottom-6 rounded-full p-4 shadow-lg bg-firefly-500 text-white focus:outline focus:outline-2 focus:outline-firefly-300" aria-label="Book a call">Book</a>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      mobileOpen: false,
      calendly: 'https://calendly.com/your-calendar-link',
      contactEmail: 'oversight@iloyola.com',
      firefly500: '#3099aa',
      form: {
        name: '',
        email: '',
        message: '',
      },
      newsletterEmail: '',
      year: new Date().getFullYear(),
    }
  },
  methods: {
    onSubmit() {
      const subject = encodeURIComponent(`Website lead from ${this.form.name}`)
      const body = encodeURIComponent(`Name: ${this.form.name}\nEmail: ${this.form.email}\n\n${this.form.message}`)
      window.location.href = `mailto:${this.contactEmail}?subject=${subject}&body=${body}`
    },
    subscribe() {
      alert('Subscribed! Replace with your mailing provider integration.')
      this.newsletterEmail = ''
    }
  }
}
</script>

<style>
:focus { outline: none; }
:focus-visible { outline: 2px solid rgba(48,153,170,0.8); outline-offset: 3px; }

.sr-only { position: absolute; width: 1px; height: 1px; padding: 0; margin: -1px; overflow: hidden; clip: rect(0, 0, 0, 0); white-space: nowrap; border: 0; }

@media (max-width: 640px) {
  .focus\:not-sr-only:focus { position: absolute; left: 1rem; top: 1rem; }
}
</style>
