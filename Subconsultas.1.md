
```
SELECT r.code, (SELECT m.age
FROM member m
WHERE m.id = r.member_id ) AS age
FROM register r;
```
![[Pasted image 20240701103014.png]]

``` 
SELECT r.code, (SELECT COUNT(total_attendees)
FROM conference c
WHERE c.id = r.id_conference ) AS nro_attendees
FROM register r;
```
![[Pasted image 20240701103220.png]]