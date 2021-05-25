import http.client
import urllib
import time

key = "1R57OC7KVYD74ELR"  # Put your API Key here
predicted_value = 555

params = urllib.parse.urlencode({'field1': predicted_value, 'key': key})
headers = {"Content-typZZe": "application/x-www-form-urlencoded", "Accept": "text/plain"}
conn = http.client.HTTPConnection("api.thingspeak.com:80")
try:
    conn.request("POST", "/update", params, headers)
    response = conn.getresponse()
    print(predicted_value)
    print(response.status, response.reason)
    data = response.read()
    conn.close()
except:
    print("connection failed")
