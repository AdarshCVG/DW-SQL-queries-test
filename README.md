SELECT 
date, platform_id, sum(reach)
FROM highlevelkpi.reach where date >= 'date limit to check' and platform_id=4 group by date, platform_id order by date, platform_id
