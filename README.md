# Responsive HTML Email Boilerplate

A production-ready HTML email template built to demonstrate industry-standard email development practices. 

When transitioning from modern web development (Flexbox/Grid) to email development, the primary challenge is rendering consistency across fragmented email clients (especially desktop Outlook). This boilerplate addresses those specific challenges.

## 🛠️ Technical Highlights

* **Table-Based Layouts:** Built entirely using `<table>`, `<tr>`, and `<td>` tags to ensure structural integrity across all email clients.
* **Outlook MSO Ghost Tables:** Utilizes conditional comments (`<!--[if mso]>`) to lock maximum widths for desktop versions of Microsoft Outlook, preventing layout breakage.
* **Bulletproof CTA Buttons:** Buttons are coded as nested tables with background colors and padding applied directly to the `<td>` and `<a>` tags. This ensures the button renders perfectly even if the user's email client blocks images by default.
* **Retina-Ready Assets:** Image containers are built to handle 2x resolution assets (e.g., loading a 1200x600 image into a 600px wide container) for crisp display on Apple devices and high-DPI screens.
* **Inline CSS:** All critical styling is strictly inline, with a `<style>` block reserved only for mobile media queries.

## 📱 Compatibility

Tested and optimized for:
* Gmail (Web, iOS, Android)
* Apple Mail (macOS, iOS)
* Microsoft Outlook (Windows 2013, 2016, 2019, Office 365)
* Yahoo! Mail

## 🚀 Usage

You can open `index.html` directly in your browser. To test the rendering in an actual inbox, you can copy the raw HTML and send it via tools like [PutsMail](https://putsmail.com/) or inject it into ESPs like Klaviyo, Mailchimp, or HubSpot.
