SELECT * 
FROM the_office;

# 1. In which season did the show have the most people watching, with the highest number of viewers tuning in?
SELECT season, 
	   SUM(us_viewers)
FROM the_office
GROUP BY season
ORDER BY season ASC;

# 2. Is there a particular director who brought more viewers throughout the life span of the show and if so, how many episodes did they direct?
SELECT directed_by AS director,
	   COUNT(*) AS episodes_directed,
       SUM(us_viewers) AS viewers,
       AVG(us_viewers) AS average_viewers
FROM the_office
GROUP BY director
ORDER BY episodes_directed DESC;

# 3. Did the number of episodes in each season correlate to the amount of viewers per season?
SELECT season,
	   COUNT(episode_num_in_season) AS episodes,
       SUM(us_viewers) as viewers
FROM the_office
GROUP BY season
ORDER BY viewers DESC;

# 4. What are the top 15 episodes with the highest viewers and what season was the episode
SELECT *
FROM the_office
ORDER BY us_viewers DESC
LIMIT 15;






