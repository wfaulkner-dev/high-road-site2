# High Road Business Solutions — Starter Site

This is a Netlify‑ready static site (HTML/CSS) with:
- Contact form powered by **Netlify Forms**
- Booking via embedded **Calendly**
- Responsive layout and simple styling

## Quick start

1. Replace the Calendly URL in `index.html` (`YOUR_HANDLE`) with your link.
2. Edit copy, email, and links as needed.
3. Push this folder to a new GitHub repo.

## Deploy to Netlify

1. In Netlify, click **Add new site → Import an existing project** and connect your GitHub repo.
2. Build command: _None_ (static)
3. Publish directory: `/` (root)
4. Click **Deploy site**.

### Forms setup
- Netlify scans `index.html` for the form:
  ```html
  <form name="contact" method="POST" data-netlify="true" netlify-honeypot="bot-field" action="/thank-you.html">
    <input type="hidden" name="form-name" value="contact">
  </form>
  ```
- After the first deploy and test submission, enable email notifications in **Netlify → Forms**.

### Custom domain & HTTPS
- In Netlify → **Domain management**, add your custom domain. Netlify will provision **Let’s Encrypt** SSL automatically.

### Optional tweaks
- Add your LinkedIn/Twitter etc.
- Update colors in `styles.css`.
- Add analytics (e.g., Netlify Analytics, plausible, GA).

---

**Note:** If you convert this to a framework later (Astro/Next.js), Netlify supports CI/CD from GitHub out of the box.
