
# User

- [create](#create)
- [destroy](#destroy)
- [getAll](#getAll)
- [getById](#getById)

___



{% api-method method="post" host=" " path="/api/v1/user" %}{% api-method-summary %}create{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to create a user</p>
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-path-parameters %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% endapi-method-headers %}

{% api-method-query-parameters %}

{% api-method-parameter name="name" type="String" required=true %}
<p>Name of the user.</p>{% endapi-method-parameter %}


{% api-method-parameter name="firstName" type="String" required=true %}
<p>Firstname of the user.</p>{% endapi-method-parameter %}


{% api-method-parameter name="email" type="String" required=true %}
<p>Email of the user.</p>{% endapi-method-parameter %}


{% api-method-parameter name="password" type="String" required=true %}
<p>Password of the user.</p>{% endapi-method-parameter %}


{% api-method-parameter name="birthDate" type="Date" required=false %}
<p>Birth date of the user</p>{% endapi-method-parameter %}


{% api-method-parameter name="role" type="UserRole" required=false %}
<p>Role of the user</p>{% endapi-method-parameter %}


{% api-method-parameter name="language" type="AvailableLanguages" required=false %}
<p>Language of the user</p>{% endapi-method-parameter %}

{% endapi-method-query-parameters %}

{% endapi-method-request %}

{% api-method-response %}

{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success-Response
{% endapi-method-response-example-description %}

```javascript
{
  id: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  name: 'Pepperwood',
  firstName: 'John',
  email: 'john@pepperwood.com',
  birthDate: new Date(1996, 12, 20)
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="delete" host=" " path="/api/v1/user/:id" %}{% api-method-summary %}destroy{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to delete a user</p>
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


{% api-method method="get" host=" " path="/api/v1/satellite" %}{% api-method-summary %}getAll{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get all users</p>
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
[{
  id: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  name: 'Pepperwood',
  firstName: 'John',
  email: 'john@pepperwood.com',
  birthDate: new Date(1996, 12, 20)
}]
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}


{% api-method method="get" host=" " path="/api/v1/user/:id" %}{% api-method-summary %}getById{% endapi-method-summary %}

{% api-method-description %}
<p>This route allows you to get a user with his identifier</p>
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
  id: '0cd30aef-9c4e-4a23-81e3-3547971296e5',
  name: 'Pepperwood',
  firstName: 'John',
  email: 'john@pepperwood.com',
  birthDate: new Date(1996, 12, 20)
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}

{% endapi-method-spec %}
{% endapi-method %}
