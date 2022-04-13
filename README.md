# study
#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
-------------------------------------------------
openssl genrsa -des3 -passout pass:<anypwd> -out server.pass.key 2048
openssl rsa -passin pass:<anypwd> -in server.pass.key -out server.key
openssl req -new -key server.key -out server.csr
openssl x509 -req -sha256 -days 365 -in server.csr -signkey server.key -out server.crt
----------------------------------------------------------------------------------------------
  CREATE access to Package Creator-
------------------------------------

Step 1: Login to the Post Refresh Automated Salesforce Org.
Step 2: Under -> Setup -> Profiles -> System Administrator. Click on edit Profile.
Step 3: In Custom Tab Setting adjust the tab named "Package Creator" drop down from Tab Hidden to Default On.
