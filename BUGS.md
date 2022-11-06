# SELISE DJANGO INTERVIEW EXAM: BUGS

## BUG 1. RuntimeError: Model class movies.models.Movie doesn't declare an explicit app_label and isn't in an application in INSTALLED_APPS.

Solution 1: Added `movies` inside the INSTALLED_APPS inside settings.py file