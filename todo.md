# IPTV SaaS Platform - TODO

## Authentication System
- [x] Email/password registration with validation
- [x] Email verification with token system
- [x] Login with email/password
- [x] Forgot password / password reset flow
- [x] Role-based access control (admin/user)
- [x] Session management with JWT
- [x] Login-first architecture (no homepage, redirect to login)

## Subscription Plans
- [x] Plan CRUD operations (admin)
- [x] Dynamic connection slider (1-10 connections)
- [x] Real-time price calculation based on connections
- [x] Plan display with features list
- [x] Plan selection and checkout flow

## Payment System - NOWPayments
- [x] NOWPayments API integration
- [x] Invoice generation for crypto payments
- [x] Webhook verification for payment confirmation
- [x] Payment status tracking
- [x] Supported cryptocurrencies display

## Payment System - Manual Methods
- [x] Admin-configurable payment methods
- [x] Card manual payment instructions
- [x] PayPal manual payment instructions
- [x] Custom payment methods (admin defined)
- [x] Payment instructions with/without links
- [x] Per-plan payment link customization
- [x] Payment proof upload

## Order Management
- [x] Order creation on checkout
- [x] Order lifecycle (Pending → Processing → Verified/Paid)
- [x] Real-time order status updates
- [x] Admin order approval workflow
- [x] Order history for users
- [x] Order management for admins

## IPTV Credential Management
- [x] Xtream Codes credential support
- [x] M3U URL credential support
- [x] Portal URL credential support
- [x] Multi-connection logic per subscription
- [x] Credential assignment to orders
- [x] Credential display for users
- [x] Credential CRUD for admins

## Admin Dashboard
- [x] User management (list, view, edit, ban)
- [x] Order management with filters
- [x] Payment verification interface
- [x] Plan management CRUD
- [x] Credential pool management
- [x] Revenue analytics and charts
- [x] System activity logs
- [x] Dashboard overview with stats

## Real-time Chat System
- [x] Socket.IO integration
- [x] Chat widget component
- [x] Full-page chat interface
- [x] User-to-admin messaging
- [x] Admin/agent visibility and response
- [x] Message history persistence
- [x] Online status indicators
- [x] Typing indicators

## Email System (Brevo SMTP)
- [x] Brevo SMTP configuration
- [x] Email verification template
- [x] Password reset template
- [x] Order confirmation template
- [x] Payment notification template
- [x] Admin-editable email templates
- [x] Email sending service

## UI/UX
- [x] Light color theme
- [x] Professional SaaS design
- [x] Smooth animations (Framer Motion)
- [x] Toast notifications
- [x] Loading states and skeletons
- [x] Responsive design
- [x] Form validation with error messages

## Security
- [x] Password hashing (bcrypt)
- [x] CSRF protection
- [x] Rate limiting
- [x] Input sanitization
- [x] Secure webhook verification
- [x] Server-side secret handling

## Supabase Migration (In Progress)
- [ ] Migrate from MySQL to Supabase PostgreSQL
- [ ] Update database schema for Supabase
- [ ] Remove email/password auth, use Manus OAuth only
- [ ] Update authentication flow to use Manus OAuth
- [ ] Test verification email links with Supabase


## Critical Bugs - Supabase Auth Integration
- [x] Fix: "Welcome back" message showing for unverified users
- [x] Fix: Login not redirecting to dashboard after authentication
- [ ] Fix: Complete Supabase Auth integration in routers (optional - using MySQL auth for now)
- [x] Fix: Email verification flow with Supabase
- [x] Fix: Session management and cookie handling


## Advanced Features (Phase 2)
- [ ] Real-time order notifications via Socket.IO
- [ ] Automatic IPTV credential assignment to orders
- [ ] Subscription renewal reminder system (7 days before expiry)
- [ ] Advanced analytics dashboard with charts
- [ ] User profile and account settings page
- [ ] Subscription management (upgrade/downgrade/cancel)
- [ ] Admin revenue reports and export
- [ ] Webhook retry logic for failed payments
- [ ] Rate limiting and DDoS protection
- [ ] Performance optimization and caching
