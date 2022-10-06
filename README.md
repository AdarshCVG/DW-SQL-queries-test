SELECT DISTINCT 
DATE, count(user_id)
FROM highlevelkpi.cvtraining_course_sign_ups where date >= 'date' group by date order by date

SELECT DISTINCT 
  "user join date", count(unique_user_id)
FROM
    highlevelkpi.imagen_cvresources_subscribers where "user join date" >= 'date' group by "user join date" order by "user join date"

SELECT 
date, count(*)
FROM highlevelkpi.imagen_cvresources_downloads where date >= 'date' group by date order by date

SELECT 
date_uploaded, COUNT(media_id), COUNT(record_id)
from highlevelkpi.imagen_cvresources_videos_library where date_uploaded >= 'date' group by date_uploaded order by date_uploaded

SELECT 
DATE, COUNT(user_id)
from highlevelkpi.cvtraining_lecture_completions where date >= 'date'group by date order by date

SELECT 
DATE, COUNT(user_id)
FROM highlevelkpi.cvtraining_course_completions where date >= 'date' group by date order by date;
