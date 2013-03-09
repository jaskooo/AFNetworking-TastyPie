AFNetworking-TastyPie
=====================

AFNetworking-TastyPie adds additional authentication headers to talk to TastyPie endpoints. AFNetworking is used by RestKit to communicate with TastyPie REST APIs.

Example:

    #import "AFNetworking+ApiKeyAuthentication.h"

    // ...

    RKObjectManager* sharedMgr = [ RKObjectManager sharedManager];
    [sharedMgr.HTTPClient setAuthorizationHeaderWithTastyPieUsername:@"username" andToken:@"token-key-provided-by-TastyPie"];

    // ...

