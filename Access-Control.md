# PortSwigger
- accessing to redirect body is not possible in network tab but in the BurpSuit repeater before clicking follow redirect
- in some cases we can find out the GUID of a user from the user profile
- changing the id parameter could cause redirect and we can capture and check the redirect body
- passwords can be shown in user profile in some cases
- `x-original-url` is a way for bypass 403 and access certain path like `/admin` or `/admin/delete?username=carlos` however it won't accept parameters and we should pass parameters in the exact url section
- changing method could bypass the `401 unauthorized`
- sometimes one extra parameter could bypass the `401 unauthorized`
- referer header could be use for authorization -> if the website checks where the request comes from.