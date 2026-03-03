# Email Setup Guide - 5 Minutes

Your contact form is ready to send emails to **theleavesinthetrees@gmail.com**!

You just need to complete this quick setup:

---

## Step 1: Create Free Formspree Account

1. Go to: **https://formspree.io/**
2. Click **"Get Started"** or **"Sign Up"**
3. Create a free account (no credit card needed)
4. Free plan includes **50 submissions per month** - perfect for a business website

---

## Step 2: Create Your Form

1. Once logged in, click **"+ New Form"**
2. **Form Name:** "DUMBROD Media Contact Form" (or whatever you want)
3. **Email Address:** `theleavesinthetrees@gmail.com`
4. Click **"Create Form"**

---

## Step 3: Get Your Form Endpoint

After creating the form, Formspree will give you a **unique form endpoint URL**. It looks like:

```
https://formspree.io/f/xyzabc123
```

**Copy this URL!** You'll need it in the next step.

---

## Step 4: Update Your Website

Open your contact page file and find this line (around line 48):

```html
<form class="contact-form-main" id="contactForm" action="https://formspree.io/f/xyzyzyzw" method="POST">
```

**Replace** `https://formspree.io/f/xyzyzyzw` with your actual Formspree endpoint from Step 3.

For example:
```html
<form class="contact-form-main" id="contactForm" action="https://formspree.io/f/xyzabc123" method="POST">
```

Save the file.

---

## Step 5: Test It!

1. Go to your contact page: http://192.168.1.193:8080/contact.html
2. Fill out the form with test information
3. Click **"SUBMIT FORM"**
4. **First submission:** Formspree will ask you to confirm your email
5. Check **theleavesinthetrees@gmail.com** for:
   - Confirmation email from Formspree (click the link)
   - Your test submission

---

## That's It!

Once confirmed, all future form submissions will automatically arrive at **theleavesinthetrees@gmail.com**!

The email will include:
- Full Name
- Email Address
- Subject
- Message

---

## Need Help?

If you get stuck:
1. Make sure you confirmed the email from Formspree
2. Check spam/junk folder
3. Verify the form action URL is correct in contact.html
4. Try submitting again after confirmation

Let me know if you need help with any step!
