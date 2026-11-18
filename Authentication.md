# PortSwigger
- in some cases 2FA can be simply bypass by ignoring the page that needs 2FA code!!
- changing the username parameter to victim in valid reset password link of our own, may cause the reset password for victim account.
- in brute forcing, the response of valid username may be different than invalid ones even a `.` -> `Invalid username or password.` and `Invalid username or password` 
- we can use `x-forwarded-for` header for bypassing the kind of ip-based detection. (simply adding a digit or may be better to add range of IP addresses)
- in some cases, processing the valid username may take more time than invalid ones. -> we must add too much characters to password parameter like 100 characters to be able to make delay for server
- if our ip is blocked , may be there is reset function with compromising the valid user pass. so we can add the valid user pass between our payloads and bypass the restriction. keep in mind in this scenario we must send one request each time(using resource pool) .