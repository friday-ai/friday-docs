
# Variable

- [create](#create)
- [destroy](#destroy)
- [getValue](#getValue)

___


{% api-method method="post" host=" " path="/api/v1/variable" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create a variable</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %} 
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="key" type="String" required=true %}
<p>Key of the variable.</p>{% endapi-method-parameter %}


{% api-method-parameter name="value" type="String" required=true %}
<p>Value of the variable.</p>{% endapi-method-parameter %}


{% api-method-parameter name="owner" type="String" required=true %}
<p>Owner's id of the variable.</p>{% endapi-method-parameter %}


{% api-method-parameter name="ownerType" type="VariableOwner" required=true %}
<p>Owner type of the variable.</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: 'a2b9ba3a-72f1-4a24-b268-e3813c1e8f32',
  key: 'test_key0',
  value: 'test_value0',
  owner: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  ownerType: 'user'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host=" " path="/api/v1/variable/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete a variable</p>
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
  "success": "true",
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host=" " path="/api/v1/variable" %}{% api-method-summary %}getValue{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all variables</p>
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
  id: 'a2b9ba3a-72f1-4a24-b268-e3813c1e8f32',
  key: 'test_key0',
  value: 'test_value0',
  owner: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  ownerType: 'user'
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
