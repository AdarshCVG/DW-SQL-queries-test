SELECT 
date, platform_id, sum(total_size), sum(size_of_the_community)
from highlevelkpi.mobilisation_community where date >= 'date' group by date, platform_id order by date, platform_id

SELECT
  date, platform_id, sum(reads_and_plays), sum(likes), sum(comments), sum(shares)
FROM
    highlevelkpi.engagements where date >= 'date' group by date, platform_id order by date, platform_id

SELECT 
date, count(church_name), sum(intro_to_jesus)
from highlevelkpi.cvoutreach_contributing_churches_itj where date >= 'date' group by date order by date

SELECT 
DATE, count(church_name)
from highlevelkpi.cvoutreach_contributing_churches where date >= 'date' group by date order by date

SELECT 
date, count(church_name), SUM(responses)
FROM highlevelkpi.cvoutreach_receiving_churches_responses where date >= 'date' group by date order by date

SELECT 
date, COUNT(church_name)
FROM highlevelkpi.cvoutreach_receiving_churches where date >= 'date' group by date order by date
