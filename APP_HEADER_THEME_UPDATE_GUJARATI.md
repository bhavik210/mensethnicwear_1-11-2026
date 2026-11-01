SHUBHVASTRA — Professional Header & Theme Update

1. Added a professional navy/blue gradient brand header with the Shubhvastra logo, title and secure portal label.
2. Improved page spacing, background, sidebar and responsive header styling while retaining existing app functionality and business data schema.
3. Added CSS to hide Streamlit's in-app toolbar/menu, Share/star/GitHub controls, deploy button and status widget where those elements are rendered inside the app DOM.

Important platform limitation:
The Streamlit Cloud "Manage app" control is part of the hosting/platform interface and is not controlled by the app's Python/CSS. It cannot be reliably removed from within the app code. The app-level toolbar/status elements are hidden where supported, but Streamlit may change its internal selectors in future releases.

Deployment:
Back up the database before updating GitHub. Replace application code/assets only; do not delete or replace the live database. Reboot the Streamlit Cloud app after pushing changes.
