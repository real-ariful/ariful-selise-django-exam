# SELISE DJANGO INTERVIEW EXAM: BUGS

## BUG 1: RuntimeError: Model class movies.models.Movie doesn't declare an explicit app_label and isn't in an application in INSTALLED_APPS.

Solution 1: Added `movies` inside the INSTALLED_APPS inside settings.py file.


## BUG 2: Unable to Access API `/api/v1/auth/register`

Solution 2: Added `path('api/v1/auth/', include('authentication.urls'))` to the url_patterns list inside api_cud/url.py file