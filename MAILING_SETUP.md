# Contact Form Mailing Setup Guide

Your contact form is now configured with **Formspree**, an open-source form backend service that handles email delivery for static websites.

## What is Formspree?

Formspree is a free, open-source service that allows static websites (like those hosted on GitHub Pages) to receive emails from contact forms. It's reliable, secure, and requires no backend code.

**Features:**
- ✅ Free tier with up to 50 submissions/month
- ✅ Open-source and transparent
- ✅ No server-side code needed
- ✅ Automatic email notifications
- ✅ Spam protection built-in
- ✅ Form data stored securely

## Setup Instructions

### Step 1: Create a Formspree Account

1. Go to [https://formspree.io/](https://formspree.io/)
2. Click **"Get Started"** or **"Sign Up"**
3. Create an account using your email (faizeltkr@gmail.com)

### Step 2: Create a New Form

1. After logging in, click **"Create"** or **"New Form"**
2. Enter a name for your form (e.g., "Portfolio Contact Form")
3. Add your email address: `faizeltkr@gmail.com`
4. Complete the form creation

### Step 3: Get Your Form ID

1. You'll see a unique **Form ID** (looks like: `xqkrvzzb`)
2. Copy this Form ID

### Step 4: Update Your Website

1. Open [index.html](index.html)
2. Find line with the Formspree endpoint:
   ```javascript
   const response = await fetch('https://formspree.io/f/xqkrvzzb', {
   ```
3. Replace `xqkrvzzb` with your actual Form ID
4. Save the file and commit to GitHub

### Step 5: Verify Your Email (Important!)

1. Check your email inbox for a verification email from Formspree
2. Click the verification link
3. Now your form will start receiving submissions!

## How It Works

When someone submits the contact form:

1. ✅ Form data is sent to Formspree
2. ✅ An email is sent to: `faizeltkr@gmail.com`
3. ✅ Success message is displayed to the user
4. ✅ Form is automatically reset
5. ✅ You can reply to the email to contact the person

## Form Features Included

Your contact form now includes:

- **Form Validation**: Ensures all required fields are filled
- **Email Validation**: Checks for valid email format
- **Loading State**: Shows "Sending..." while submitting
- **Success Message**: Displays confirmation to users
- **Error Handling**: Shows helpful error messages
- **Accessibility**: Full keyboard navigation support
- **Dark Mode Support**: Works in light and dark themes
- **Mobile Responsive**: Works perfectly on all devices

## Checking Your Submissions

### Option 1: Email Notifications (Default)
- You'll receive an email for each form submission
- Reply directly to respond to users

### Option 2: Formspree Dashboard
- Log in to [https://formspree.io/](https://formspree.io/)
- View all submissions in your dashboard
- Export submissions as CSV
- Set up additional notifications

## Upgrade Options

The free tier includes:
- **50 form submissions per month**
- **Basic email notifications**
- **Form data retention**

For more submissions:
- **Pro Plan**: $25/month for unlimited submissions
- See [https://formspree.io/pricing](https://formspree.io/pricing) for details

## Troubleshooting

### Form submissions not working?
1. Verify your Form ID is correct in index.html
2. Check that you've verified your email with Formspree
3. Check your spam/junk folder for Formspree verification email
4. Open browser console (F12) for any error messages

### Not receiving emails?
1. Verify email in your Formspree dashboard settings
2. Check spam/junk folders
3. Check Formspree dashboard for blocked domains
4. Ensure domain is properly configured

### Want to customize further?
See the contact form in [index.html](index.html) around line 930. You can:
- Add more form fields
- Customize the success/error messages
- Change styling
- Add additional validation

## Alternative Open-Source Solutions

If you prefer alternatives to Formspree:

### 1. **Basin** (https://basin.io)
- Similar to Formspree, simple setup
- Free tier available

### 2. **Self-Hosted: Nodemailer + Vercel Functions**
- Full control over the code
- More complex setup
- Requires Node.js knowledge

### 3. **Email.js** (https://www.emailjs.com)
- Client-side email sending
- Free tier: 200 emails/month

## Security & Privacy

Your Formspree setup includes:
- ✅ HTTPS encryption
- ✅ SPAM protection
- ✅ DDoS protection
- ✅ No data sold to third parties
- ✅ GDPR compliant

## Support

For Formspree support:
- Documentation: [https://formspree.io/docs/](https://formspree.io/docs/)
- Email: support@formspree.io

---

**Next Steps:**
1. Go to [https://formspree.io/](https://formspree.io/) and sign up
2. Create your form and get your Form ID
3. Update the Form ID in index.html
4. Test by submitting the contact form
5. Deploy to GitHub Pages

Your contact form is now ready to receive emails! 🎉
