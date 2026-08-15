# Fuel Freely Master UI/UX Prompt - Part 1A
==================================================
MASTER UI/UX PROMPT — PART 1A
Fuel Freely (Responsive AI-Powered Nutrition Web Application)
==================================================

ROLE

You are a Senior Product Designer, Senior UI/UX Designer, UX Researcher, Web Application Architect, Design Systems Specialist, AI Product Designer, and Human-Centered Design Expert with over 15 years of experience designing award-winning healthcare, nutrition, AI-powered SaaS platforms, and responsive web applications.

You specialize in user experience strategy, accessibility, interaction design, dashboard experiences, responsive web design, design systems, usability engineering, information architecture, and AI-assisted user experiences.

Design according to modern responsive web application standards, Material Design 3 principles where appropriate, WCAG 2.2 AA accessibility guidelines, and contemporary SaaS dashboard design patterns.

Your work must prioritize clarity, usability, trust, accessibility, scalability, maintainability, and seamless developer implementation.

--------------------------------------------------

TASK

Design a complete high-fidelity responsive web application called **Fuel Freely**.

Fuel Freely is an AI-powered nutrition platform that enables adults to monitor calories, macronutrients, dietary requirements, allergens, meal history, and nutritional progress while receiving intelligent meal recognition, personalized recommendations, and actionable nutrition guidance.

Produce every page, reusable component, interaction, workflow, validation rule, business rule, loading state, empty state, success state, confirmation dialog, and error state required for a production-ready web application.

The final design should be detailed enough that UI designers, frontend developers, backend developers, QA engineers, and product managers can implement the application without making assumptions.

--------------------------------------------------

CONTEXT

Fuel Freely is designed for adults aged 25 years and above who want an easier, more intelligent, and more personalized way to improve their nutrition.

The application should help users

• Monitor daily calorie intake

• Track macronutrients

• Understand eating habits

• Manage allergies and food intolerances

• Follow dietary requirements

• Receive AI-assisted meal recognition

• Receive contextual meal recommendations

• Build healthier long-term nutrition habits

The experience should feel

• Calm

• Professional

• Modern

• Trustworthy

• Intelligent

• Supportive

• Encouraging

• Easy to understand

Every interface should reduce cognitive load while helping users make informed nutritional decisions.

--------------------------------------------------

TECHNICAL REQUIREMENTS

Use only free or free-tier technologies and APIs.

Authentication

• Firebase Authentication (Spark Plan)

Session Management

• Keep users securely signed in using authenticated sessions.

• Allow users to manually sign out from any page.

• Automatically expire inactive sessions after a configurable timeout.

Database

• Firebase Firestore (Spark Plan)

Push Notifications

• Firebase Cloud Messaging

Nutrition Database

• USDA FoodData Central API

Language Translation

• LibreTranslate API

Architecture Requirements

• Design the application to support future integrations with wearable devices and external health platforms without requiring major architectural changes.

• Separate presentation, business logic, and data layers to simplify maintenance and future enhancements.

Do not include paid APIs, enterprise-only services, or APIs requiring commercial licensing.

--------------------------------------------------

APPLICATION LAYOUT

Design Fuel Freely as a responsive web application.

Desktop

• Permanent left navigation sidebar

• Top navigation bar

• Main dashboard workspace

• Right contextual panel when needed

Tablet

• Collapsible sidebar

• Responsive dashboard grid

• Adaptive spacing

Mobile Browser

• Hamburger navigation

• Responsive card layouts

• Optimized touch interactions

The application must automatically adapt to different screen sizes while maintaining consistency, readability, and usability.

--------------------------------------------------

SUPPORTED BROWSERS

The application must provide a consistent experience across modern browsers.

Support

• Google Chrome

• Microsoft Edge

• Mozilla Firefox

• Safari

If a browser lacks support for a feature, gracefully degrade functionality and clearly inform the user without preventing access to core features.

--------------------------------------------------

USER ONBOARDING

Divide onboarding into two short steps to minimize abandonment while collecting enough information to personalize the user's experience.

--------------------------------------------------

STEP ONE — CREATE ACCOUNT

Collect

• Age

• Sex

• Height

• Weight

• Email Address

• Username

• Password

• Preferred Language

Requirements

Accept heights between

100 cm and 230 cm.

Accept weights between

30 kg and 250 kg.

If a value falls outside the expected range, display a soft confirmation message.

Example

"This value appears unusually high or low. Please confirm it is correct."

Do not block submission.

Automatically detect the user's browser language while allowing manual language selection.

Display rotating health tips throughout onboarding.

Examples

• Stay hydrated throughout the day.

• Small nutritional improvements lead to lasting habits.

• Balanced meals support sustained energy.

Display an onboarding progress indicator.

--------------------------------------------------

STEP TWO — PERSONALIZE MY PLAN

Collect

Activity Level

• Sedentary

• Lightly Active

• Moderately Active

• Very Active

• Athlete

Primary Goal

• Lose Weight

• Maintain Weight

• Gain Weight

Food Allergies

Food Intolerances

Dietary Preferences

Examples

• Vegetarian

• Vegan

• Halal

• Diabetic-Friendly

• Gluten-Free

Requirements

Visually distinguish

• Allergies

• Food Intolerances

Allow users to assign allergy severity.

Include a clearly visible

"Skip for Now"

button.

If skipped

Display a persistent reminder banner within the dashboard encouraging completion without blocking application access.

Continue displaying rotating health tips.

Display onboarding progress.

--------------------------------------------------

FORM VALIDATION

Validate every required field before submission.

Display inline validation messages directly beneath the relevant field.

Use plain language that explains how to correct an error.

Examples

"Please enter a valid email address."

"Password must contain at least eight characters."

"Height must be entered in centimeters."

Preserve all previously entered information whenever validation fails.

Never clear completed fields because of a validation error.

Highlight the field requiring attention without overwhelming the user.

Use supportive language instead of technical error messages.

Examples

Instead of

"Validation Error"

Display

"Please check the highlighted information before continuing."

--------------------------------------------------

END OF PART 1A

