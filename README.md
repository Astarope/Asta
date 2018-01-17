# Asta
request.post({
    url: "https://api.kik.com/v1/config",
    auth: {
        user: "<username>",
        pass: "<api_key>"
    },
    json: {
        "webhook": "https://example.com/incoming", 
        "features": {
            "receiveReadReceipts": false, 
            "receiveIsTyping": false, 
            "manuallySendReadReceipts": false, 
            "receiveDeliveryReceipts": false
        }
    }
}, callback);
