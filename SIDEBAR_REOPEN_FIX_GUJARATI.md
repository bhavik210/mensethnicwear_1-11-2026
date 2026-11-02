# Sidebar Reopen Control Fix

- Streamlit header shell and native collapsed-sidebar control are explicitly kept visible.
- Toolbar actions (Share, star, GitHub, menu) remain hidden without hiding the sidebar reopen control.
- Sidebar collapse button remains visible when the sidebar is open.
- Mobile touch target for the native reopen control is preserved.
- No database or business data changes.

Deploy by replacing app code and rebooting Streamlit Cloud. Verify the collapsed-control arrow on desktop and mobile.
