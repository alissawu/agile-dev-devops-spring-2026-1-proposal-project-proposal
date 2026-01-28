# InternNest

**Verified Sublets for Interns**

## What and Why?

### The Problem

Subletting your apartment to a stranger is risky. You have little recourse if they damage your place, skip rent, or cause problems. Current platforms like Craigslist and Facebook groups offer zero verification. Subleasors often resort to awkward social media stalking, or just pray for the best. 
(Personally, I've subleased from ppl who felt safer knowing my Linkedin/school/credit score/employment, but I've also subleased from people who just didn't know me. The subleasing ecosystem is default quite lawless.)

### The Solution

**InternNest** is a sublet platform specifically designed for subleasors to find verified interns as tenants.

All users must complete at least one identity verification (LinkedIn, .edu email, or social media). Interns must additionally upload their offer letter as a PDF to prove their intern status—this ensures only real interns can apply for sublets.

### Why Interns Make Ideal Tenants

- **Employed** - They have income from their internship
- **Temporary** - Internship length (typically 10-12 weeks) matches common sublet durations
- **Professional** - They are responsible enough to get a job and have reputations to protect at their companies. They've also typically already gone through background checks.
- **Highly verifiable** - Multiple data points to confirm identity and legitimacy

### Why This Matters

Every summer, thousands of interns flood cities like NYC, SF, and Seattle searching for temporary housing. Simultaneously, thousands of students studying abroad and professionals traveling need to sublet their apartments. Trust is the main friction point on both sides. InternNest solves this by creating a verified marketplace.

## For Whom?

### Subleasors (Verified Listers)

College students studying abroad, young professionals traveling for work, or anyone who needs to sublet their apartment and wants a trustworthy tenant. These users need to complete at least one identity verification to list, which protects interns from scam listings. In return, they get access to a pool of verified, employed tenants.

### Subletters (Verified Interns Only)

Only verified interns can sign up to find housing. This includes summer interns at tech companies, finance firms, consulting companies, and other organizations who need temporary housing near their workplace. This also includes off-season interns, who can sublet off study-abroad students, without hoping for some NYU/Columbia/Stanford/Cal/[insert college in city of internship] student mutual that'll connect them with a study-abroading peer. 

### Why This Model Works

- **Subleasors** get access to a curated pool of verified, employed tenants—no more gambling on strangers
- **Interns** get a platform where landlords are also verified, reducing scam risk, plus their verification gives them a competitive advantage over random applicants on other platforms
- **Two-sided verification** builds trust for both parties—interns know the listing is legitimate, subleasors know the tenant is real and employed

### Why These Are Real Users

This is a problem the proposer and their peers personally face. Every summer, friends scramble to find sublets for internships while others struggle to find trustworthy tenants when studying abroad. The demand on both sides is real and recurring.

## How?

### Verification Requirements

All users must complete at least one identity verification:
- Connect LinkedIn profile
- Verify university email (.edu)
- Link Instagram or other social media

Interns must additionally upload their offer letter as a PDF (company name and dates visible, salary and everything else can be blurred) to prove their intern status. This is required on top of the one identity verification minimum.

### For Interns (Subletters)

1. **Sign up and verify:**
   - Upload offer letter as PDF (required to prove intern status)
   - Complete at least one identity verification (LinkedIn, .edu email, or social media)

2. **Browse available sublets** filtered by city, dates, and price

3. **Apply to listings** - Subleasors see your verification badges and professional profile

4. **Message subleasors**, arrange viewings, and finalize the sublet

### For Subleasors

1. **Sign up and verify** - Complete at least one identity verification (LinkedIn, email, or social media)

2. **Create a listing** with photos, price, dates, amenities, and location

3. **Receive applications** only from verified interns

4. **View applicant profiles** - See their company, school, LinkedIn, and verification badges

5. **Find a subletter with confidence** knowing they've been verified

### Key Features

- **Verification badge system** - Visual indicators showing what's verified (offer letter, LinkedIn, .edu, etc.)
- **Search and filter** - Find sublets by city, date range, and price
- **Messaging system** - Direct communication between subleasors and applicants
- **Listing creation** - Full listing support with photos and details

## Scope

### Why This Is Right-Sized for 4-6 Programmers in One Semester

**Core features are achievable:**
- User authentication and profiles
- Verification integrations (LinkedIn OAuth, email verification, file upload for offer letters)
- Listing CRUD (create, read, update, delete)
- Search and filter functionality
- Messaging between users
- Basic responsive web UI

### Not Too Easy

- **Multiple user types** with different flows (subleasors vs. subletters)
- **Two-sided verification** - Both interns and subleasors must verify, with different verification requirements for each
- **Third-party integrations** - LinkedIn API, email verification services
- **File uploads and storage** - Handling offer letters and listing photos
- **Messaging system** - Real-time or near-real-time communication between users
- **OAuth implementation** - Non-trivial authentication flow with LinkedIn

### Not Too Ambitious

- **Well-defined feature set** - Clear boundaries on what's in scope
- **No payment processing** - MVP doesn't require handling money (users arrange payment offline. This just connects them.)
- **No recommendation algorithms** - Simple season &  date search/filter instead of AI matching
- **No complex ML/AI** - Offer letter verification uses a cheap LLM (GPT-4o mini) to validate company name and dates from uploaded documents. The text is obtainable from pdf-parse.
- **Standard web app architecture** - Proven tech stack, no experimental technologies

The project has enough technical depth through OAuth integrations, file handling, and messaging to be challenging, while remaining achievable without requiring payment infrastructure, machine learning, or complex algorithms.
