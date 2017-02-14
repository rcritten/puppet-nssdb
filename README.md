# nssdb puppet module

very simple puppet module to create an NSS database and add a certificate
and key via PEM files.

This module can do two things:

1. Create a new NSS database with an optional password
2. Import a cert and key in the form of PEM files by using openssl
   to create a PKCS#12 file and then calling the NSS pk12util to load
   it into the target NSS database.
