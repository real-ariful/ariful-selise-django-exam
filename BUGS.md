# SELISE DJANGO INTERVIEW EXAM: BUGS

## BUG 1: RuntimeError: Model class movies.models.Movie doesn't declare an explicit app_label and isn't in an application in INSTALLED_APPS.

Solution 1: Added `movies` inside the INSTALLED_APPS inside settings.py file.


## BUG 2: Unable to Access API `/api/v1/auth/register`

Solution 2: Added `path('api/v1/auth/', include('authentication.urls'))` to the url_patterns list inside api_cud/url.py file


## BUG 3: AssertionError: May not set both `read_only` and `required` for password  and password2 under RegisterSerializer

Solution 3: Replace `read_only` from password and password2 under RegisterSerializer with `write_only`.

## BUG 4: User can not be registered.  RegisterView access given for only Admin Users.

Solution 4: Replace `permission_classes = (IsAdminUser,)` for RegisterView with `permission_classes = (AllowAny,)`.