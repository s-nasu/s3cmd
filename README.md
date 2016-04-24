s3cmd role
=============

Installs the s3cmd tool.This role will let you s3cmd and configure it for ES.By setting the url and signature_v2 variables, you can also use it in S3-compatibility mode.

GMO cloud configuration has been left commented out as a configuration example.

Requirements
------------

None

Usage
-----

The role is supposed to be used this way from a playbook:

   - { role: s-nasu.s3cmd }

Role Variables
--------------

```
s3cmd:
  access_key: S3 access key
  secret_key: S3 secret key
  bucket_location: US
  url: s3.amazonaws.com
  signature_v2: False
  # url: inter-st.gmocloud.com
  # signature_v2: True
```

Dependencies
------------

No

License
-------

Unlicense (Public Domain)
