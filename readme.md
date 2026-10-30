# NP Visa World

NP Visa World is a responsive ASP.NET public portal for a visa and immigration consultancy. Visitors can explore student, tourist, work, and PR visa services by country, check eligibility and document requirements, read success stories, and book a consultation or send an inquiry. The portal is SEO-friendly, mobile-ready, managed through an easy admin panel, and features interactive UI elements—such as a custom moving cursor—to enhance the visual experience.

## Features

- **Public landing pages** — home, about, services, countries, success stories, and contact pages with a clean, responsive layout.
- **Visa services by country** — explore student, tourist, work, and PR visa services categorized by destination country.
- **Eligibility checker** — interactive tool for visitors to check basic eligibility for selected visa categories.
- **Document requirements** — clear listings of required documents per visa type and country.
- **Success stories** — showcase of client success stories and testimonials.
- **Consultation booking** — free consultation booking form with validation.
- **Inquiry form** — contact form for general inquiries, with submissions stored and viewable in the admin panel.
- **Interactive UI** — custom moving cursor effect and smooth animations for an engaging, modern browsing experience.
- **SEO-friendly** — clean URLs, meta titles/descriptions, canonical tags, Open Graph tags, sitemap, and `robots.txt`.
- **Mobile-ready** — responsive layout for mobile, tablet, and desktop.
- **Admin panel** — manage pages, visa services, countries, success stories, consultation bookings, inquiries, and site settings.
- **Shared web UI** — Razor views, shared layout, partials, pagination helper, and client-side validation.

> Feature descriptions are based on the controllers, domain models, services, and views present in this repository. Actual behavior may depend on the connected database and configuration.

## Technology stack

- C# and .NET Framework 4.8 (or `<your target framework>`)
- ASP.NET MVC with Razor views
- Bootstrap for responsive UI
- HTML, CSS, JavaScript, and jQuery
- Visual Studio solution (`NPVisaWorld.sln`)
- Entity Framework + SQL Server for content, bookings, and inquiry storage
- SEO tooling: meta tags, sitemap, and `robots.txt`

## Solution structure

```text
V4/
├── NPVisaWorld.sln
├── NPVisaWorld/                           # ASP.NET MVC public portal
│   ├── Controllers/                       # Public + admin controllers
│   ├── Views/                             # Razor UI pages
│   │   ├── Shared/                        # Layout and partials
│   │   ├── Home/                          # Landing pages
│   │   ├── Services/                      # Visa services pages
│   │   ├── Countries/                     # Country-specific pages
│   │   ├── SuccessStories/                # Testimonials and stories
│   │   ├── Consultation/                  # Booking and inquiry forms
│   │   └── Admin/                         # Admin panel views
│   ├── Content/                           # CSS, JS, images, fonts, cursor effects
│   ├── App_Start/                         # Routes, filters, DI setup
│   ├── Config/                            # Environment-specific app settings
│   └── Web.config
├── NPVisaWorld.Domain/                    # Domain models and list/pagination models
├── NPVisaWorld.Infrastructure/            # Service interfaces, helpers, constants, exceptions
└── NPVisaWorld.Service/                   # Service implementations and data access