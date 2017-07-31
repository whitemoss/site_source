---
layout: page
title: Обратная связь
permalink: feedback.html
---

<form action="https://formspree.io/{{ site.email }}" method="POST">
  <p>
    Ваше имя:
    <input type="text" name="name" size="50"/>
  </p>
  <p>
    Ваш e-mail:
    <input type="email" name="_replyto" size="40" />
  </p>
  <p>
    Выберите интересующее вас изделие: <br />
    <select name="item" size="1">
      <option disabled="disabled" selected="selected">-</option>
      {% for collection in site.collections %}
        {% if collection.label != "posts" %}
          {% for item in collection.docs %}
            <option value="{{ item.title | escape }}">{{ item.title | escape }}</option>
          {% endfor %}
        {% endif %}
      {% endfor %}
      <option value="Другое">Другое / указать в сообщении</option>
    </select>
  </p>
  <p>
    Сообщение: <br />
    <textarea name="comment" cols="50" rows="10"></textarea>
  </p>
  <p>
    <input type="submit" value="Отправить" />
  </p>
</form>
