1)actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.<br><code>
  (select first_name from actor)
union 
(select first_name from customer);</code><br>
2)actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.<br><code>
  (select first_name from actor)
intersect
(select first_name from customer);</code><br>
3)actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.<br><code>
  (select first_name from actor)
except
(select first_name from customer);</code><br>
4)İlk 3 sorguyu tekrar eden veriler için de yapalım.
<br><code>
  (select first_name from actor)
union all 
(select first_name from customer);</code><br>

  
