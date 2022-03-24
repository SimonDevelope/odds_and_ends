2022.03.24

```sql
select a.mb_recommend, b.mb_name, count(*) from g5_member a
left outer join g5_member b on b.mb_id = a.mb_recommend
group by 1,2
having count(*) > 10
order by 1.2;
```

> 아래 10명 이상인 사람을 찾는 sql문
