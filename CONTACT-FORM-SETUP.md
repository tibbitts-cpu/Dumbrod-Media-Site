# Contact Form Setup Guide

The contact form is now installed on your website! However, you need to complete one quick setup step to make it send emails to **theleavesinthetrees@gmail.com**.

## Option 1: Formspree (Recommended - Free & Easy)

Formspree is a free service that handles form submissions and sends them as emails.

### Setup Steps:

1. **Go to Formspree:** https://formspree.io/
2. **Sign up** for a free account (50 submissions/month)
3. **Create a new form:**
   - Click "New Form"
   - Enter email: `theleavesinthetrees@gmail.com`
   - Copy the form endpoint (looks like `https://formspree.io/f/xyzabc123`)
4. **Update your website:**
   - Open `index.html`
   - Find this line (around line 177):
     ```html
     <form class="contact-form" id="contactForm" action="https://formspree.io/f/xyzyzyzw" method="POST">
     ```
   - Replace `https://formspree.io/f/xyzyzyzw` with your actual Formspree endpoint

5. **Done!** Test the form and check theleavesinthetrees@gmail.com for submissions.

## Option 2: Netlify Forms (If hosting on Netlify)

If you're hosting on Netlify, it's even easier:

1. Add `netlify` attribute to the form tag
2. Netlify automatically handles submissions
3. Configure email notifications in Netlify dashboard

## Option 3: EmailJS (Alternative)

If you prefer EmailJS:
1. Sign up at https://www.emailjs.com/
2. Create an email service and template
3. Update the JavaScript to use EmailJS API

---

## Current Status

✅ Contact form UI is complete
✅ Modal opens/closes properly
✅ Form validation works
⚠️ Email delivery needs Formspree setup (5 minutes)

Once you complete the Formspree setup, the form will automatically send all submissions to Shawna's email!
