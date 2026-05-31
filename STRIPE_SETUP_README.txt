Stripe Payment Link Setup
=========================

I updated get-started.html so the Subscribe button redirects users to Stripe Checkout instead of using the fake card form.

Before publishing:
1. Open get-started.html.
2. Find this section:
   const stripePaymentLinks = {
     freemium: "",
     premium: "#PASTE_PREMIUM_STRIPE_PAYMENT_LINK_HERE",
     professional: "#PASTE_PROFESSIONAL_STRIPE_PAYMENT_LINK_HERE",
     enterprise: "#PASTE_ENTERPRISE_STRIPE_PAYMENT_LINK_HERE",
     elite: "#PASTE_ELITE_STRIPE_PAYMENT_LINK_HERE"
   };
3. Replace each placeholder with the correct Stripe Payment Link.
4. Save and upload the website.

Example:
professional: "https://buy.stripe.com/test_xxxxxxxxxxxxx"

The plan detail pages already send users to:
get-started.html?plan=premium
get-started.html?plan=professional
get-started.html?plan=enterprise
get-started.html?plan=elite

So the correct plan will be pre-selected automatically.
