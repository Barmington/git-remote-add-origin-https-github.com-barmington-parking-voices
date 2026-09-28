Parking Voices

A community platform where UK road users share their driving and parking experiences, and push for positive change.

Parking Voices gives drivers a place to be heard. Whether it's confusing signage, unfair enforcement, or a lack of safe spaces, users can raise concerns, talk with others who share them, and help build a collective voice for improvement.



Live demo: https://drive.google.com/file/d/1Kv8sGk65w5Od4TQCk3Xfd34z3tckjl2/view?usp=sharing

<img width="333" height="501" alt="image" src="https://github.com/user-attachments/assets/d71dfce8-47e9-49d0-b963-34144d7a8652" />

Features
Real-time chat: talk with other road users instantly.
Voice chat: join live voice conversations with the community.
Clean, intuitive interface: a visually appealing design that is easy to pick up.
Accessibility-first: buttons have clear, descriptive accessible names, and ARIA attributes are used throughout to support assistive technologies.
Automatic user sync: Clerk webhooks keep user data in sync with the database.
♿ Accessibility

Parking Voices is designed to be usable by everyone. This includes:

Descriptive, meaningful accessible names on all interactive elements
ARIA attributes to communicate roles, states, and live updates to screen readers
An interface designed to be intuitive and easy to navigate

Tech Stack
Frontend: e.g. React / Next.js
Authentication: Clerk
Database: e.g. PostgreSQL / Supabase
Real-time & voice: e.g. WebSockets / WebRTC

Clerk Webhook Sync

User events from Clerk (such as sign-up, profile updates, and account deletion) are received via webhooks and written directly to the application database, so user data stays consistent without manual syncing.

Environment variables
Variable	Description
CLERK_PUBLISHABLE_KEY	Clerk publishable key
CLERK_SECRET_KEY	Clerk secret key
CLERK_WEBHOOK_SECRET	Signing secret for Clerk webhooks
DATABASE_URL	Database connection string

Adjust the names above to match your project.

My Contributions
I implemented the Clerk webhook integration and database sync
Designed and implemented the accessible UI (ARIA attributes, accessible button names)


