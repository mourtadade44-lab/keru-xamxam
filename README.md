**Project Name:** Këru XamXam (House of Knowledge)
**Project Type:** Educational Learning Management System (LMS) and Tutoring Hub
**Subjects:** Islamic Sciences (Sharia, Fiqh, etc.) & English Language

Here is the comprehensive blueprint to hand over to your developer friend. It breaks down the architecture, user experience, and technical requirements so they know exactly what to build.

---

## 1. Site Architecture (Sitemap)

This is what a visitor will see when they arrive at the site.

* **Home:** A welcoming landing page introducing you, highlighting the two main branches of study (Islamic Sciences and English), and showing featured courses.
* **Course Catalog:** A library where visitors can browse available pre-recorded courses and group modules.
* **Private Tutoring:** A page explaining your 1-on-1 customized teaching services, complete with a booking or inquiry form.
* **About the Teacher:** Your credentials, teaching philosophy, and background in both Sharia and English.
* **Student Portal (Dashboard):** A private, logged-in area where students access their purchased materials, schedules, and private lessons.

## 2. Core Functionality: The Student Experience

The site needs to act as a virtual school. Your friend should build a robust Student Dashboard that includes:

* **Role-Based Access Control:**
* *Group Students:* Have access to shared modules, standard course materials, and group live-session links.
* *Private Students:* Have a dedicated profile where you can manually assign them "hidden" or customized courses built specifically for them.


* **The "Paywall" (Smart Course Unlocking):**
* Integration with an automated payment gateway.
* Once a student pays for a specific module or signs up for a private package, the site must automatically change their account status and unlock the corresponding videos, PDFs, or Zoom links.
* *Local Payment Note:* Depending on where your students are, ensure the developer integrates international gateways (Stripe, PayPal) and/or local African payment systems (like Paystack, Flutterwave, Wave, or Orange Money) if applicable.


* **Progress Tracking:** Students should see a progress bar (e.g., "75% complete") for their pre-recorded courses so they know exactly where they left off.

## 3. Course Delivery Features

You are teaching two different ways (Pre-recorded and Live). The platform must support both smoothly:

* **Pre-Recorded Courses (VOD):**
* Structured into Modules and Lessons.
* Secure video hosting (your developer should embed videos using Vimeo or a secure server to prevent illegal downloading).
* Downloadable resource sections for PDFs and reading materials.


* **Live Classes (Group & Private):**
* Integration with Zoom, Google Meet, or Microsoft Teams.
* A calendar view inside the student dashboard showing upcoming live classes.
* An automated email system that sends a reminder 1 hour before a live class starts.



## 4. User Experience (UX) & Design Guidelines

Because accessibility and ease of use are priorities, outline these design rules for your friend:

* **Mobile-First Design:** The majority of online students, especially in language and religious studies, will likely access the site via their smartphones. The dashboard, video player, and reading materials must format perfectly on small screens.
* **Clean, Uncluttered Interface:** Use a calming, academic color palette (e.g., deep greens, whites, and gold for the Islamic sciences; clean blues or neutrals for the English section).
* **Easy Navigation:** A student should be able to log in, find their current lesson, and start learning in three clicks or less.
* **Accessibility Features:** Clear, readable fonts, high contrast between text and background, and easily identifiable buttons for non-tech-savvy users.

## 5. Developer Notes (Technical Recommendations)

*Pass this specific section directly to your friend to save them development time.*

* **CMS & LMS Framework:** The most cost-effective and flexible way to build this is using **WordPress** paired with an LMS plugin like **Tutor LMS**, **LearnDash**, or **MasterStudy**. These systems already have the "pay-to-unlock" logic and student dashboards built-in.
* **E-Commerce Integration:** Use **WooCommerce** to handle the checkout process. It connects seamlessly with LMS plugins and supports almost every payment gateway in the world.
* **Custom Post Types / Groups:** For the private 1-on-1 students, the LMS plugin should have a "Group" or "Cohort" feature, allowing the admin to create a private course and enroll a single user ID into it, keeping it hidden from the public catalog.
* **Speed Optimization:** Ensure a caching plugin is installed and images are compressed, so the site loads quickly even for students with slower internet connections.
