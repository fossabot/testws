# test Websocket chat with bdd authentification

```bash
npm install --save ws
npm install --save mysql
```
<br>
db config : 
```
+----------------+
| Tables_in_test |
+----------------+
| chat           |
| user           |
+----------------+
```

table 'chat' :<br>
+---------+---------+------+-----+---------+----------------+<br>
| Field   | Type    | Null | Key | Default | Extra          |<br>
+---------+---------+------+-----+---------+----------------+<br>
| ID      | int(11) | NO   | PRI | NULL    | auto_increment |<br>
| user    | text    | YES  |     | NULL    |                |<br>
| Message | text    | NO   |     | NULL    |                |<br>
+---------+---------+------+-----+---------+----------------+<br>
<br>
table 'user' : <br>
+-------+---------+------+-----+---------+----------------+<br>
| Field | Type    | Null | Key | Default | Extra          |<br>
+-------+---------+------+-----+---------+----------------+<br>
| ID    | int(11) | NO   | PRI | NULL    | auto_increment |<br>
| user  | text    | NO   |     | NULL    |                |<br>
| pass  | text    | NO   |     | NULL    |                |<br>
+-------+---------+------+-----+---------+----------------+<br>
