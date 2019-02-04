# Channels

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/channels/:channel" %} {% api-method-summary %} Get channel information {% endapi-method-summary %}

{% api-method-description %} Retrieve information for the specified channel. {% endapi-method-description %}

{% api-method-spec %} {% api-method-request %} {% api-method-path-parameters %} {% api-method-parameter name="channel" type="string" required=true %} Channel ID {% endapi-method-parameter %} {% endapi-method-path-parameters %} {% endapi-method-request %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authorization Bearer token
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-response %} {% api-method-response-example httpCode=200 %} {% api-method-response-example-description %}

{% endapi-method-response-example-description %}
```javascript
{
    "profile": {
        "headerImage": "https://cdn.streamelements.com/static/user/profile_header_default.png"
    },
    "provider": "twitch",
    "_id": "1234567890",
    "isPartner": false,
    "broadcasterType": "affiliate",
    "providerId": "568709",
    "displayName": "TwitchUser",
    "username": "twitchuser",
    "avatar": "https://static-cdn.jtvnw.net/jtv_user_pictures/twitchuser-profile_image-8a9fbe3c190447ce-300x300.jpeg",
    "alias": "twitchuser",
    "inactive": false
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a user matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "statusCode": 404,
    "error": "Not Found",
    "message": "channel invalidid was not found"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



