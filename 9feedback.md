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
    Сообщение: <br />
    <textarea name="comment" cols="50" rows="10"></textarea>
  </p>
  <p>
    <input type="submit" value="Отправить" />
  </p>
</form>
