# VibeCoding Portfolio Website

testing Lovable for making professional portfolio website including booking feature.


```
Build a professional counseling website with three main purposes:
1) Portfolio
2) Appointment Booking
3) Media / Press Coverage page

This website represents a licensed therapist. It must feel trustworthy, calm, and professional.

--------------------------------
🌿 BRAND TONE & DESIGN
--------------------------------
- Emotional tone: Calm, safe, psychologically comforting
- Visual style: Minimal, spacious layout
- Color palette: White + soft beige (#F5EBE0 tone) + subtle gray(#EDEDE9)
- Typography: Clean sans-serif (Pretendard or similar)
- Avoid heavy animations
- Mobile-first responsive design
- Accessibility friendly (clear buttons, large tap areas)

--------------------------------
🏠 PAGES STRUCTURE
--------------------------------

1) Home
- Hero section with therapist introduction
- Short tagline about counseling philosophy
- CTA button: “Book a Session”
- Trust indicators (years of experience, certifications)
- Link to media coverage

2) About / Portfolio
- Profile image
- Professional background
- Certifications
- Counseling specialties (Anxiety, Depression, Couples therapy, etc.)
- Counseling philosophy section
- Testimonials section

3) Booking Page
Core features:
- use Calendly to connect with google calendar
- Calendar UI showing available dates only
- User selects date → available time slots appear
- Booking form:
   - Name
   - Email
   - Phone
   - counseling session type
- Confirmation screen after booking 

Logic requirements:
- Prevent double booking
- Store booking in database
- Admin can view bookings
- Send confirmation email to client

4) Media / Press Page
- List layout of press articles 
- Each item includes:
   - Thumbnail image
   - Article title
   - Media outlet name
   - Publication date
   - External link
- Admin can add/edit/delete articles

--------------------------------
🔐 ADMIN SYSTEM
--------------------------------
- Admin login required
- Admin dashboard:
   - View bookings
   - Add media articles
   - Edit testimonials

--------------------------------
📅 GOOGLE CALENDAR INTEGRATION
--------------------------------
Booking system must integrate with Google Calendar by using Calendly:

- Only fetch free/busy time slots
- Do NOT expose full calendar details-Only use Google free/busy endpoint. Do not return event details to client
- When booking is confirmed:
    - Create event in therapist's Google Calendar
- All Google API calls must be server-side only
- API keys stored securely in environment variables

--------------------------------
🧠 UX REQUIREMENTS
--------------------------------
- User flow must feel simple and safe
- Maximum 3 steps to complete booking
- Clear confirmation message
- Error handling for unavailable time
- Timezone handling included

--------------------------------
🗄 DATA STRUCTURE
--------------------------------
Booking model:
- id
- name
- email
- phone
- sessionType
- date
- time
- status
- createdAt

Media model:
- id
- title
- outlet
- date
- thumbnail
- url

--------------------------------
🚀 OUTPUT EXPECTATION
--------------------------------
Generate:
- Full page structure
- UI components
- Database schema
- API routes logic
- Google Calendar integration logic
- Admin dashboard layout
- Responsive design

This must be production-ready.
```
