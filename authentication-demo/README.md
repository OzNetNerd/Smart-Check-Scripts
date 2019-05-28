# Authentication Demo

Demonstrates how to authenticate against Smart Check and make API calls, e.g `/api/sessions` (as documented [here](https://automation.deepsecurity.trendmicro.com/article/11_1/smart-check-api-reference?platform=on-premise#operation/listSessions)).

## Usage

Help menu:

```
$ python3 authentication-demo.py  -h
usage: authentication-demo.py [-h] -u USERNAME -p PASSWORD -b BASE_URL

Smart Check API Wrapper

optional arguments:
  -h, --help            show this help message and exit
  -u USERNAME, --username USERNAME
                        Smart Check username
  -p PASSWORD, --password PASSWORD
                        Smart Check password
  -b BASE_URL, --base-url BASE_URL
                        Smart Check URL

```

Example command & output:

```
python3 authentication-demo.py -u administrator -p password -b https://a1db48ed280ef11e9b9fd022fbd87295-7482937192.ap-southeast-2.elb.amazonaws.com

{
    "sessions": [
        {
            "created": "2019-05-28T02:22:06Z",
            "expires": "2019-05-28T03:22:06Z",
            "href": "/api/sessions/fe6c4e8a-15f5-4179-b82e-d07fa7df8b92",
            "id": "fe6c4e8a-15f5-4179-b82e-d07fa7df8b92",
            "updated": "2019-05-28T02:22:06Z",
            "user": {
                "created": "2019-05-28T02:21:31Z",
                "href": "/api/users/afb92212-6e67-494a-b34a-26b0c30d1491",
                "id": "afb92212-6e67-494a-b34a-26b0c30d1491",
                "passwordChangeRequired": false,
                "role": "8e3b6f3d-1c0b-4635-a1ad-8a2b545eeb41",
                "updated": "2019-05-28T02:22:18Z",
                "userID": "administrator"
            }
        },
        {
            "created": "2019-05-28T02:23:36Z",
            "expires": "2019-05-28T03:23:36Z",
            "href": "/api/sessions/aaa1836c-b13f-4339-8510-804449944581",
            "id": "aaa1836c-b13f-4339-8510-804449944581",
            "updated": "2019-05-28T02:23:36Z",
            "user": {
                "created": "2019-05-28T02:21:31Z",
                "href": "/api/users/afb92212-6e67-494a-b34a-26b0c30d1491",
                "id": "afb92212-6e67-494a-b34a-26b0c30d1491",
                "passwordChangeRequired": false,
                "role": "8e3b6f3d-1c0b-4635-a1ad-8a2b545eeb41",
                "updated": "2019-05-28T02:22:18Z",
                "userID": "administrator"
            }
        },
        {
            "created": "2019-05-28T02:23:54Z",
            "expires": "2019-05-28T03:23:54Z",
            "href": "/api/sessions/3a63db65-d887-4bee-956c-0790bdd56952",
            "id": "3a63db65-d887-4bee-956c-0790bdd56952",
            "updated": "2019-05-28T02:23:54Z",
            "user": {
                "created": "2019-05-28T02:21:31Z",
                "href": "/api/users/afb92212-6e67-494a-b34a-26b0c30d1491",
                "id": "afb92212-6e67-494a-b34a-26b0c30d1491",
                "passwordChangeRequired": false,
                "role": "8e3b6f3d-1c0b-4635-a1ad-8a2b545eeb41",
                "updated": "2019-05-28T02:22:18Z",
                "userID": "administrator"
            }
        },
        {
            "created": "2019-05-28T02:30:03Z",
            "expires": "2019-05-28T03:30:03Z",
            "href": "/api/sessions/edc23e82-ee62-4cc2-8bb9-cbb686a7dd74",
            "id": "edc23e82-ee62-4cc2-8bb9-cbb686a7dd74",
            "updated": "2019-05-28T02:30:03Z",
            "user": {
                "created": "2019-05-28T02:21:31Z",
                "href": "/api/users/afb92212-6e67-494a-b34a-26b0c30d1491",
                "id": "afb92212-6e67-494a-b34a-26b0c30d1491",
                "passwordChangeRequired": false,
                "role": "8e3b6f3d-1c0b-4635-a1ad-8a2b545eeb41",
                "updated": "2019-05-28T02:22:18Z",
                "userID": "administrator"
            }
        }
    ]
}

```

