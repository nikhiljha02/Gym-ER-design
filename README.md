🏋️ Fitness Coaching Platform – ER Diagram

This repository contains the database design and ER diagram for an online fitness coaching platform.
The system is designed for trainers/influencers who manage clients, plans, subscriptions, payments, sessions, check-ins, progress, and diet plans.

📌 Overview

The platform supports:

Client and trainer management
Coaching plans and subscriptions
Online sessions (yoga, zumba, cardio, PT, etc.)
Progress tracking (weight, measurements, diet, workout adherence)
Diet plans created by trainers
Payment tracking for each subscription
Client check-ins and activity logs



🧱 Entities
Clients

Stores client details and profile information.

Trainers

Stores trainer/influencer data and expertise.

Plans

Fitness and coaching packages available for purchase.

Subscriptions

Tracks which client purchased which plan and under which trainer.

Payments

Stores payment details for each subscription.

Sessions

Scheduled online sessions or consultations.

Check-Ins

Daily or weekly client check-ins.

Diet Plans

Customized diet plans created by trainers.

Progress

Weekly or monthly progress tracking.



Relationships
Clients <> Trainers (many-to-many through subscriptions)
Plans < Subscriptions
Clients < Subscriptions
Subscriptions < Payments
Trainers < Diet Plans
Clients <> Diet Plans (if assignment exists)
Clients < Sessions
Trainers < Sessions
Clients < CheckIns
Clients < Progress


Use Cases Supported
Assign clients to trainers
Manage multiple coaching programs
Track subscription status (active, expired, cancelled)
Record payments and transaction details
Schedule and track sessions
Track client progress over time
Maintain diet and workout adherence
Manage check-ins and attendance
