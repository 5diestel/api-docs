# Giveaways

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/giveaways/:channel" %} {% api-method-summary %} Get channel giveaways {% endapi-method-summary %}

{% api-method-description %} Retrieve giveaways for the specified channel. {% endapi-method-description %}

{% api-method-spec %} {% api-method-request %} {% api-method-path-parameters %} {% api-method-parameter name="channel" type="string" required=true %} Channel ID {% endapi-method-parameter %} {% endapi-method-path-parameters %} {% endapi-method-request %}

{% api-method-response %} {% api-method-response-example httpCode=200 %} {% api-method-response-example-description %}

{% endapi-method-response-example-description %}
{
    "active": null,
    "giveaways": []
}
{% endapi-method-response-example %} {% endapi-method-response %} {% endapi-method-spec %} {% endapi-method %}
