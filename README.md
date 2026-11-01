# Awesome-Mobile-CRM-Sales-App

# Top Mobile CRM & Sales App Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Native Mobile CRM, Offline-First Field Sales & Self-Hosted Relationship Management*  
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Mobile CRM & Sales Apps**. These tools enable sales teams and field representatives to manage contacts, update deal pipelines, and log activities directly from their phones—turning time between meetings into productive selling time.

**Examples** include HubSpot Mobile App, Salesforce Mobile, Pipedrive Mobile, Zoho CRM Mobile, Freshsales Mobile, Microsoft Dynamics 365 Mobile, Copper Mobile, Close Mobile, Base CRM Mobile, and Nimble Mobile (the category leaders).

**Open-source emphasis**: Mobile CRM is a domain where open-source tooling has **genuinely matured, and the standout option now offers a native mobile app alongside a full self-hosted backend**. **BottleCRM** is the clear leader—an MIT-licensed, self-hosted CRM with a **native Flutter app for iOS and Android**, a SvelteKit web app, and a documented REST API, all sharing one Django backend . **Twenty** has community-built native mobile clients: **TwentyMobile** (AGPL-3.0, connects directly to your self-hosted instance, includes business card scanning) and **Viginti** (native iOS/iPadOS/Mac client with offline support and a Pro subscription) . **EspoCRM** offers a native iPhone app (with Android currently web-only) . The critical caveat: **many "mobile CRM" open-source projects are templates or UI kits**—crm-lead-management-app-react-native is an Android template for lead management , and ClientFlow AI is a React Native template rather than a deployable product . **Krayin's community explicitly lists "Mobile app" as a weakness** (67% of reviewers cited it as needing improvement) . Choose based on whether you need a deployable backend (BottleCRM, Twenty) or a starting point to build your own (templates).

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[HubSpot Mobile App](https://www.hubspot.com/)**  
  Native mobile access to HubSpot CRM; manage contacts, deals, tasks, and activities with offline support and push notifications.

- **[Salesforce Mobile](https://www.salesforce.com/)**  
  Salesforce's native mobile app; access CRM records, update opportunities, log calls, and use Salesforce Mobile SDK for custom apps.

- **[Pipedrive Mobile](https://www.pipedrive.com/)**  
  Native mobile CRM focused on visual pipeline management; drag deals through stages and log activities on the go.

- **[Zoho CRM Mobile](https://www.zoho.com/crm/)**  
  Native mobile app within the Zoho ecosystem; manage leads, contacts, and deals with offline access.

- **[Freshsales Mobile](https://www.freshworks.com/freshsales/)**  
  Native mobile CRM with built-in phone and email; AI-powered deal insights on mobile.

- **[Microsoft Dynamics 365 Mobile](https://www.microsoft.com/en-us/dynamics-365)**  
  Native mobile app for Dynamics 365 Sales; access accounts, contacts, and opportunities with offline capability.

- **[Copper Mobile](https://www.copper.com/)**  
  Native mobile CRM built for Google Workspace; automatic activity capture from Gmail and Calendar on mobile.

- **[Close Mobile](https://close.com/)**  
  Conversation-first CRM with native mobile apps; calling, email, and SMS with sequences and smart views on the go.

- **[Base CRM Mobile](https://www.zenefits.com/)**  
  Mobile-first CRM (acquired by Zendesk, now part of Zendesk Sell); focused on pipeline management and activity tracking on mobile.

- **[Nimble Mobile](https://www.nimble.com/)**  
  Relationship-focused CRM with native mobile app; social insights and contact enrichment on the go.

## Open-Source GitHub Projects

### Full CRM with Native Mobile Apps (Self-Hosted)

- **[BottleCRM](https://github.com/django-crm/django-crm)**  
  The **strongest open-source mobile CRM option** available (MIT, Django 6/DRF, Svelte 5) . Features: **native Flutter app for iOS and Android** sharing one backend with the web app; **leads, accounts, contacts, opportunities, support tickets, tasks, and invoices**; **PostgreSQL Row-Level Security** for multi-tenant isolation at the database layer; **agent-ready REST API** with OpenAPI schema for AI agent access (Claude, Cursor, Codex, Gemini) with per-user tokens inheriting role and permissions; **full helpdesk** with SLA timers, approvals, escalations, macros, and knowledge base . **No per-seat pricing, no user caps, no feature paywall** . Docker Compose quick start (`docker compose up --build`) with frontend at :5181 and Swagger at :8000 . **Best for teams wanting a complete, self-hosted CRM with a native mobile app**—the closest open-source equivalent to HubSpot or Pipedrive with mobile access.

- **[EspoCRM](https://github.com/espocrm/espocrm)**  
  Mature open-source CRM (PHP, AGPL-3.0) with a **native iPhone app** available on the App Store . Features: calling and texting contacts, moving deals, checking pipelines, push notifications, AI assistant, and open-house capture (for real-estate use cases) . **Critical caveat**: **Android users must use the web portal**—no native Android app today . The app is included with every Espo account; what you can do follows your plan . **Best for iPhone-based sales teams** wanting a proven CRM with native mobile—but Android users are second-class citizens.

### Twenty CRM Mobile Clients (Community-Built)

- **[TwentyMobile](https://apps.apple.com/pk/app/twentymoblie/id6760371090)**  
  A **native mobile app for Twenty CRM** (AGPL-3.0, iOS/iPadOS/Mac) that connects directly to your self-hosted Twenty instance . Features: **Today screen** (overdue tasks, today's priorities, tomorrow's agenda, recent contacts); **business card scanning** (camera extracts name, email, phone, company—on-device, no internet); **smart reminders** (local push 30 minutes before deadlines); voice-to-text notes; vCard sharing via AirDrop/WhatsApp; dark/light theme . **Privacy-first**: no third-party servers, no data collection, no subscriptions—data transits only between device and your server . **Best for Twenty users wanting a native mobile companion**—but it is a third-party app, not officially maintained by Twenty.

- **[Viginti](https://app.sensortower.com/overview/6782863969?country=US)**  
  A **native iOS/iPadOS/Mac client for Twenty CRM** (released July 2026) . Features: contacts, companies, opportunities, tasks, notes, and custom objects; **searchable, fast, and offline**; "No web view. No compromise" . **Pro subscription**: $3.99/month or $24.99/year . **Best for Twenty users wanting a polished native Apple experience**—but it is a paid third-party client, and the Pro model may not suit everyone.

### Templates & Starting Points (Not Deployable Products)

- **[crm-lead-management-app-react-native](https://github.com/mah-shamim/crm-lead-management-app-react-native)**  
  An **Android-only React Native template** for lead and pipeline management (Redux, multi-language, notifications) . **Critical caveat**: it is a **UI template**, not a deployable CRM—no backend, no data layer, no production readiness. **Best for developers** wanting a starting point to build their own mobile CRM UI—not for teams seeking a working product.

- **[ClientFlow AI Mobile App](https://github.com/Priyansh-Agarwal/clientflowai-deployment)**  
  A **React Native mobile app implementation** for iOS and Android with CRM functionality: contact management, deal pipeline (Kanban), message center (SMS/email/WhatsApp), calendar, analytics, **offline support**, push notifications, biometric auth, and enterprise features (SSO, 2FA, encryption) . **Critical caveat**: it is an implementation document/repo, not a maintained product—verify activity and production readiness before adoption . **Best for developers** wanting a comprehensive React Native CRM template with enterprise features—not a turnkey solution.

- **[CRM-Real-Estate](https://github.com/NPSarode/CRM-Real-Estate)**  
  A **React Native mobile app** for real-estate lead management: view/update leads, contact management, role-based access, dashboard, and backend integration (Node/Express/PostgreSQL/JWT) . **Niche**: real-estate-focused rather than general CRM . **Best for real-estate developers** wanting a starting point—not a general-purpose CRM.

### Additional Strong Open-Source Options

- **Krayin** — Open-source Laravel CRM (MIT, 24k GitHub stars) with lead management, contacts, sales pipeline, tasks, custom fields, email integration, and reporting . **Critical caveat**: the community explicitly cites **"Mobile app" as a weakness** (67% of reviewers) —mobile access is via web, not a native app . **Best for teams prioritizing a full-featured web CRM** over native mobile.
- **SuiteCRM Mobile (legacy)** — A **React Native** mobile app for connecting to a SuiteCRM server (2017, React Native) . **Verify maintenance status**—it is a legacy project and may not be production-ready for current SuiteCRM versions .

**Frameworks for building custom systems**: For a **complete self-hosted CRM with a native Flutter app**, BottleCRM is the clear leader . For an **iPhone-native experience with a proven CRM**, EspoCRM . For **Twenty users wanting native mobile clients**, TwentyMobile (free, AGPL) or Viginti (paid, polished) . For **developers building their own mobile CRM**, crm-lead-management-app-react-native (Android UI) or ClientFlow AI (React Native enterprise features) serve as starting points . **Avoid relying on templates as production products**—they require backend development and hardening. **Krayin's lack of native mobile** makes it unsuitable if mobile-first is a hard requirement.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Mobile CRM platforms handling customer and deal data must comply with applicable privacy regulations (GDPR, CCPA) and organizational security policies; **self-hosted solutions place full responsibility for security patches, backups, and mobile sync infrastructure on the operator**.
- **Open-source mobile CRM is mature at the backend layer but native mobile support varies**—**BottleCRM provides a native Flutter app for iOS and Android** and is the strongest option , while **EspoCRM is iPhone-only** (no Android app) , and **Twenty relies on third-party clients** (TwentyMobile, Viginti) . **Krayin explicitly lacks a native mobile app** and the community cites this as a weakness . **Many "mobile CRM" repos are templates**, not deployable products—verify before committing.
- Verify license terms for commercial use; BottleCRM uses MIT , EspoCRM uses AGPL-3.0 , and TwentyMobile uses AGPL-3.0 . Viginti is a paid third-party client with Pro subscription .

---

**Made for sales leaders, field representatives, and organizations choosing their mobile CRM stack.**  
Let's make mobile CRM more open, but with clear eyes about the native app gap that separates a complete mobile experience from a web-wrapped compromise.
