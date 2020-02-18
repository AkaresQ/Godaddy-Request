import requests
un = "username"
pw = "password"
headers = {"content-type": "application/json"}
payload = {"username":un,"password":pw,"remember_me":"True","plid":1,"API_HOST":"godaddy.com"}
Sess = requests.post(f"https://sso.godaddy.com/v1/api/idp/login?realm=idp&path=%2Fproducts&app=account", json=payload,headers=headers)

if "error" in Sess.text:
    print("Invalid Account")
else:
    print("Valid Account")

