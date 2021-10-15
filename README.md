# Lambda_Clear_Cache
A simple lambda function to clear a cloudfront cache - to be ran in codepipeline. Make sure that the codepipeline service user has permissions to invokve lambda functions otherwise, it'll fail.
 
 ## Source/Maintainers ##
Python 3.8 lambda function 'borrowed' from the internet and edited for blinx usage. Written by @mtsouthworth (no longer maintained after November 2021).

## AWS Permissions ##
Permissions Needed:

Codepipeline service user:
- Privelleges to invoke lambda functions (if ran in codepipeline) 
- Trust relationship with Lambda service

Lambda User:
- Lambda execution role
- Codepipeline create clear cache privelleges.
