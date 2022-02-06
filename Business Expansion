select ua.id, ua.first_name, ua.last_name, cu.id, cu.customer_name,count(cu.id)
from customer cu, user_account ua, contact c
where cu.id = c.customer_id and c.user_account_id = ua.id
group by ua.id, ua.first_name, ua.last_name, cu.id, cu.customer_name
having count(cu.id) > 1
