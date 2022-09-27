SELECT 
date, platform_id, sum(intro_to_jesus)
FROM highlevelkpi.intro_to_jesus where date >='2022-09-04' and platform_id=4 AND data_source_id = 128 group by date, platform_id order by date, platform_id
