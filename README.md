var body = $response.body;
var obj = JSON.parse(body);

obj.subscription = {
    "status": "Canva Pro",
    "expires_at": "2099-12-31T23:59:59Z",
    "features": {
        "premium_templates": true,
        "no_watermark": true,
        "hd_export": true,
        "background_remover": true,
        "brand_kit": true
    }
};

body = JSON.stringify(obj);
$done({body});
