---
title: Document - Creating Test Certificates
description: Sometimes you need to create test certificates for unit tests.  In this post I share the steps I've used to accomplish this.
comments: true
---

You may come across a situation where you need to create test certificates for a unit test.  This can be accomplished with the following steps:

### Create KeyStore
    keytool -genkeypair -alias server-certificatekey -keyalg RSA -validity 36500 -keystore server-keystore.jks -ext SAN=DNS:localhost

* Validity specifies the number of days that the cert is valid
* the ext option specifies a hostname

### Check Entries
    keytool -list -v -keystore server-keystore.jks

### Export Certificate
    keytool -export -alias server-certificatekey -keystore server-keystore.jks -rfc -file server.cer

### Add to TrustStore
    keytool  -import -alias server-certificatekey -file server.cer -keystore trust-store.jks
