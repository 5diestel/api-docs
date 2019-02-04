# Overlays

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/overlays/:channel" %} {% api-method-summary %} Get channel overlays {% endapi-method-summary %}

{% api-method-description %} Retrieve overlays of the specified channel. {% endapi-method-description %}

{% api-method-spec %} {% api-method-request %} {% api-method-path-parameters %} {% api-method-parameter name="channel" type="string" required=true %} Channel ID {% endapi-method-parameter %} {% endapi-method-path-parameters %} {% endapi-method-request %}

{% api-method-headers %} {% api-method-parameter name="Authorization" type="string" required=true %} Authorization Bearer token {% endapi-method-parameter %} {% endapi-method-headers %}

{% api-method-response %} {% api-method-response-example httpCode=200 %} {% api-method-response-example-description %}

{% endapi-method-response-example-description %}
```javascript
{
    "total": 2,
    "docs": [
        {
            "settings": {
                "width": 1920,
                "height": 1080,
                "name": "1080p"
            },
            "type": "mobile",
            "preview": "https://cdn.streamelements.com/uploads/e4e348a6-5cc1-417e-966c-a9d75051da28.jpg",
            "mobile": false,
            "_id": "12345678901234567890",
            "channel": "1234567890",
            "theme": "PURPLE WAVE STATIC ALERTS",
            "themeId": "5bc59b880ffc75008af892b0",
            "game": null,
            "name": "Mobile - MOBILE ALERTS - PURPLE WAVE ALERTS STATIC",
            "createdAt": "2019-02-02T17:33:39.446Z",
            "updatedAt": "2019-02-02T17:33:39.446Z"
        },
        {
            "settings": {
                "width": 1920,
                "height": 1080,
                "name": "1080p"
            },
            "type": "regular",
            "preview": "https://static-cdn.jtvnw.net/ttv-boxart/Talk%20Shows-272x380.jpg",
            "mobile": false,
            "_id": "1234567890987654321",
            "updatedAt": "2017-11-15T12:03:26.202Z",
            "createdAt": "2017-08-16T18:28:42.617Z",
            "game": null,
            "name": "Followers",
            "theme": "false",
            "channel": "1234567890"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}
