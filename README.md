# Authentication-
today lesson a form in 2min

1/from django.contrib.auth.forms import UserCreationForm

2/ add this to the html 
{%extends 'base.html'%}
{%block content%}
<h1>Welcome this is the signup</h1>
<form method="post">
    {%csrf_token%}
    {{ form.as_p }}
    <button type="submit">Sign Up</button>
</form>
{%endblock%}
# python3 manage.py shell 


In [1]: from django.contrib.auth.models import User

In [2]: User.objects.count()
Out[2]: 5

In [3]: User.objects.first()
Out[3]: <User: yassine>

