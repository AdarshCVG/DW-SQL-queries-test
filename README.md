SELECT 
date, sum(response), platform_id
from highlevelkpi.response where date >= 'date limit to check' group by date, platform_id order by date, platform_id
