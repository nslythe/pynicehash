# pynicehash
# feature
For now pynicehash support only rig management, get and set mining rig state.

# usage

```
nh = pynicehash.NiceHash(api_url, organisation_id, api_key, api_secret)

rigs = nh.get_rigs()

for rig in rigs:
  print (rig.name)
  for device in rig.devices:
    print (device.name)
```

When creating the NiceHash object you have to pass your connection credential.
* api_url you have two choice:
https://api-test.nicehash.com for testing, in testing you probably will not have any mining rig.
https://api2.nicehash.com for production

* organisation_id
The organisation_id is the the id you can find in you page where you create you api key.

* api_key

* api_secret

![api_creation](assets/api_creation.png)
