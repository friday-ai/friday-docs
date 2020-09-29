
# Session

- [getAll](#getAll)
- [revoke](#revoke)

___


{% api-method method="get" host=" " path="/api/v1/session" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all sessions</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %} 
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host=" " path="/api/v1/session/revoke/:id" %}{% api-method-summary %}revoke{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to revoke an session</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %} 
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% endapi-method-spec %}
{% endapi-method %}
