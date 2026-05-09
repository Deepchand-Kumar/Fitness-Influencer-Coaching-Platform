# Fitness-Influencer-Coaching-Platform
The Fitness Influencer Coaching Platform is a database-driven system designed to support online coaching. It enables trainers to onboard clients, sell fitness plans, schedule consultations, manage subscriptions, track progress, and record weekly check-ins.
Fitness Influencer Coaching Platform
Web Dev Cohort 2026

# Project Overview
A fitness influencer has expanded their online coaching business beyond Instagram DMs and Meet calls. This platform will serve as a structured ecosystem where trainers can onboard clients, sell fitness plans, schedule consultations, manage subscriptions, track progress, and maintain regular check-ins.

Unlike a traditional gym management system, this platform focuses on online coaching support with flexible options for consultations, long-term coaching, live sessions, and personalized diet/workout guidance.

# Database Design Goals
The database should answer key business questions

Who are the trainers and who are the clients?

What plans or coaching programs exist?

Which client purchased which plan?

When does a client’s plan start and end?

Are consultations or sessions being scheduled?

Are clients submitting check-ins weekly?

How is progress being tracked?

Can multiple clients enroll in the same program?

Can one trainer handle many clients?

How should payment and subscription information be stored?

# Core Entities
Trainer: Coaches/influencers managing multiple clients.

Client: Users who subscribe to plans or book consultations.

Plan/Program: Fitness or diet coaching packages.

Subscription: Links clients to purchased plans with start/end dates.

Session/Consultation: Scheduled one-on-one or group meetings.

Check-in: Weekly updates from clients (weight, measurements, notes).

Progress Tracking: Stores client metrics separately from user details.

Payment: Records transactions, invoices, and subscription fees.

Trainer Notes: Feedback stored independently from check-ins.

# Keys & Relationships
Primary Keys (PK): Unique identifiers for each entity.

Foreign Keys (FK): Link clients to trainers, plans, subscriptions, and sessions.

Relationships:
-------------------

One trainer → Many clients

One client → Many plans (over time)

One plan → Many clients

One client → Many check-ins

One session → One or more clients
