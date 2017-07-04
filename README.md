https://www.polar.com/accesslink-api/?shell#authorization-endpoint

Account is created successfully
Your account is created successfully

Your Polar AccessLink account is now ready for use.
Below you’ll find your client key and client secret. Use these credentials to access Polar AccessLink.
The client key and client secret will only be shown once. If you lose either one you can create new credentials in the Admin tool.
Note that if the client key or client secret is renewed, the authentication in the http headers must be changed accordingly.

Client key
ac001bab-6acf-494d-a0e9-865e860f8fcf

Client Secret
d0f1f358-ff86-4b6a-ade2-5b1f8e31089a

https://flow.polar.com/oauth2/authorization?response_type=code&scope=accesslink.read_all&client_id=ac001bab-6acf-494d-a0e9-865e860f8fcf

http://www.patnaj.pl/?code=99750454167b8f5e34630c965cb05118

echo "ac001bab-6acf-494d-a0e9-865e860f8fcf:d0f1f358-ff86-4b6a-ade2-5b1f8e31089a" | base64
YWMwMDFiYWItNmFjZi00OTRkLWEwZTktODY1ZTg2MGY4ZmNmOmQwZjFmMzU4LWZmODYtNGI2YS1h
ZGUyLTViMWY4ZTMxMDg5YQo=

YWMwMDFiYWItNmFjZi00OTRkLWEwZTktODY1ZTg2MGY4ZmNmOmQwZjFmMzU4LWZmODYtNGI2YS1hZGUyLTViMWY4ZTMxMDg5YQ0K

curl -H"Content-Type:application/x-www-form-urlencoded" -H"Accept:application/json;charset=UTF-8" -u ac001bab-6acf-494d-a0e9-865e860f8fcf:d0f1f358-ff86-4b6a-ade2-5b1f8e31089a -X POST https://polarremote.com/v2/oauth2/token -d 'grant_type=authorization_code&code=43d22c2059c07f21f7ff9fd94941b3d6'

{"access_token":"5e853887af911696dc4caf9a0fa8dbca","token_type":"bearer","expires_in":473039999,"x_user_id":36101474}

{"access_token":"426216f0ca83d4065ec197a734a5a429","token_type":"bearer","expires_in":473039999,"x_user_id":36101474}


curl -v -u ac001bab-6acf-494d-a0e9-865e860f8fcf:d0f1f358-ff86-4b6a-ade2-5b1f8e31089a https://www.polaraccesslink.com/v3/notifications
