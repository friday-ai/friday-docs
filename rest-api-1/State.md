
# State

- [getByOwner](#getByOwner)
- [set](#set)

___


{% api-method method="get" host=" " path="/api/v1/state/:id" %}{% api-method-summary %}getByOwner{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get a state with his owner's identifier</p>
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

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '17ea7282-507b-496b-b496-a6d8ce7fac17',
  owner: 'c6f6ed8a-80d0-4a90-8c3f-470b9ca3696a',
  ownerType: 'user',
  value: 'user.at.home'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host=" " path="/api/v1/state" %}{% api-method-summary %}set{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to set a state</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %} 
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="owner" type="String" required=true %}
<p>Owner of the state.</p>{% endapi-method-parameter %}


{% api-method-parameter name="value" type="AvailableState" required=true %}
<p>Value of the state.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '17ea7282-507b-496b-b496-a6d8ce7fac17',
  owner: 'c6f6ed8a-80d0-4a90-8c3f-470b9ca3696a',
  ownerType: 'user',
  value: 'user.at.home'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
