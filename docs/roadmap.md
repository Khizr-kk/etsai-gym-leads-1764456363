# Roadmap

## Week 1
- Set up core project structure and version control.
- Implement basic user authentication (registration, login) and session management.
- Develop basic Gym Profile setup page.
- Integrate WhatsApp Business API webhook to receive messages.
- Integrate Instagram Graph API webhook to receive messages.
- Create a basic database schema for `Leads`, `Messages`, `Users`, `Gyms`.
- Develop a "Unified Inbox" UI to display incoming messages (initially just text) from both WhatsApp and Instagram, sorted by most recent.
- Create a "Lead Profile View" page to display basic contact details (name, phone/handle) and source for a selected lead.
- Implement a simple mechanism to change a lead's status (e.g., "New" to "Contacted") within the Lead Profile.
- Enable adding a simple text note to a lead.
- Deploy a clickable demo environment.

## Weeks 2-4
- **Lead Ingestion & API Integration (WhatsApp, Instagram)**
    - Enhance WhatsApp and Instagram integrations for two-way communication (sending replies).
    - Handle various message types (text, images, links).
    - Implement robust error handling and logging for API integrations.
    - Develop a standardized data model for incoming leads from different sources.
- **Lead Management & CRM Core**
    - Refine "Lead Profile View" to include full interaction history with timestamps.
    - Implement comprehensive Lead Status Tracking (New, Contacted, Follow-up, Converted, Lost) with clear UI indicators.
    - Develop UI and backend for adding and managing custom tags for leads.
    - Implement "Basic Follow-up Reminders" feature, allowing users to schedule a reminder for a specific lead.
- **Communication Hub (Unified Inbox)**
    - Enhance Unified Inbox with real-time message updates.
    - Implement reply functionality directly from the inbox.
    - Add filters and search capabilities to the inbox (by lead, status, source).
- **User & Gym Management**
    - Expand Gym Profile settings (e.g., logo, business hours).
    - Implement password reset functionality.
- **Reporting & Analytics Engine**
    - Develop "Dashboard" UI to display key metrics: total leads, leads by source, conversion rate (basic calculation based on status changes).
    - Implement data aggregation for dashboard metrics.
- **ML Lead Scoring Service (Initial Data Collection)**
    - *ML Note*: Begin collecting and structuring lead interaction data (source, status changes, notes content, message length) as a foundation for future ML models. No ML models are trained or deployed yet.

## Month 2-3
- **Infrastructure & Stability**
    - Implement robust database backups and restore procedures.
    - Optimize database queries and schema for performance.
    - Set up comprehensive monitoring and alerting for system health and API integrations.
    - Implement rate limiting for external API calls to comply with platform policies.
    - Enhance security: Implement data encryption at rest and in transit, enforce stricter access controls.
    - Refactor critical modules for scalability and maintainability.
    - Establish CI/CD pipeline for automated testing and deployment.
- **Polishing & UX**
    - Conduct user testing and incorporate feedback for UI/UX improvements.
    - Develop an intuitive onboarding wizard for new gyms.
    - Enhance responsiveness and cross-device compatibility of the application.
    - Improve error messages and user notifications.
    - Implement pre-defined message templates for quick replies.
- **Analytics & Reporting**
    - Expand Dashboard capabilities with more granular filtering (e.g., by date range, staff if applicable).
    - Implement basic export functionality for lead data.
- **Documentation & Support**
    - Create user guides and FAQs.
    - Set up an in-app help system or knowledge base.
- **Preparation for Sellable Product**
    - Implement subscription/payment gateway integration (if applicable for pricing model).
    - Finalize product branding and marketing materials.

## Task Backlog
- ML-driven lead scoring and prioritization (hot/warm/cold) - *ML integration*
- Automated suggestions for optimal follow-up actions - *ML integration*
- Bulk messaging capabilities (within WhatsApp Business API limits)
- Staff accounts with role-based access control
- Integration with basic calendar for appointment scheduling
- Advanced analytics and customizable reports
- NLP for sentiment analysis of lead messages - *ML integration*
- Implement media gallery for lead attachments
- Develop a mobile application companion
- Integrate with other communication channels (e.g., Facebook Messenger, SMS)
- Customizable lead forms for website integration
- A/B testing framework for message templates
- Integration with CRM systems (e.g., HubSpot, Salesforce)