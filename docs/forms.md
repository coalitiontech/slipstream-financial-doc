# Forms

The Homepage Hero and Contact Lead blocks integrate with **Gravity Forms**. Each has a **Gravity Form ID** field. The homepage hero also exposes an optional form-shortcode field; ask the developer to confirm its use before replacing an existing setup.

## Basic maintenance

1. Open **Forms** in WordPress and identify the form used by the page.
2. Edit its fields in Gravity Forms. Review confirmations and notifications in the form settings.
3. Keep the page block’s Gravity Form ID matched to the intended form.
4. Save and test the form on the front end, including required-field errors and the confirmation message.

Form headings in the page block are separate from form input labels. If the form does not render, have the developer verify plugin activation and the selected form ID.

Developer follow-up: document the actual form names/IDs, notification recipients, delivery setup, integrations and spam protection after checking the current configuration. Do not add credentials or submission data to this guide.
