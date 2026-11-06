# Laboratory Activity: Secure API with Laravel 13

**Name:** Cris Lawrence M. Dano
**Section:** BSICT-3B
**Repository:** https://github.com/entrinax22/laravel_new_act_integ2

## Screenshots checklist
- [x] 01-public-api-200.png
- [x] 02-register-201.png
- [x] 03-login-200.png
- [x] 04-profile-no-token-401.png
- [x] 05-profile-with-token-200.png
- [x] 06-invalid-login-422.png
- [x] 07-logout-200.png
- [x] 08-revoked-token-401.png

## Reflection
A 401 response means the request had no valid token, so access to the
protected profile endpoint was denied. A successful authenticated profile
response (200) means the Bearer token was valid, so the user's data was
returned. After logout, the token is deleted, so using the same token on the
profile endpoint returns 401 again.