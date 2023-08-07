# Administration
Endpoints for instance administration.

## GET /admin
Returns admin dashboard information.
### Response
```json
{
    "instance_stats": {
        "wallet_balance": 10000000,
        "total_profits": 5000000000,
        "total_merchants": 12
    },
    "recent_withdrawals": [
        {
            "id": "009c1085-3988-4426-b655-fdf8add5a0d1",
            "merchant_name": "siren",
            "amount": 10000000,
            "date": "2023-04-08T19:19:05Z"
        },
        {
            "id": "658bfae2-8669-4639-8c6b-c2d8aa75a0c8",
            "merchant_name": "stnby",
            "amount": 10000000,
            "date": "2023-03-29T12:01:40Z"
        }
    ]
}
```

## GET /admin/withdrawal
Returns withdrawals from all merchants on this instance.

## GET /admin/payment
Returns payments from all merchants on this instance.
### Response

## GET /admin/merchant
Returns a list of all merchants on this instance.
### Response

## GET /admin/merchant/{account_id}
Returns information about a merchant.
### Response

## POST /admin/merchant/{account_id}
Modifies settings for a merchant.
### Response

## DELETE /admin/merchant/{account_id}
Deletes a merchant account.
### Response

## GET /admin/instance
Returns current instance settings.
### Response
```json
{
    "version": "0.0.1",
    "default_commission": 1000,
    "custodial_mode": true,
    "registrations_allowed": true,
    "withdrawal_times": "weekly"
}
```

## POST /admin/instance
Modifies instance settings.
### Request
### Response
