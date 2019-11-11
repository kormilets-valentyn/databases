# 12_MySQL_data_CRUD
select title, year, fullname, age from films inner join actor_id on films.id = actor_id.film_id INNER JOIN actors on actors.id = actor_id.actor where actors.fullname= 'Leonardo DiCaprio' order by title;<br/>
SELECT fullname from films inner join actor_id on films.id = actor_id.film_id INNER JOIN actors on actor_id.actor = actors.id where title = 'Titanic';
select title, actors.fullname, directors.fullname from films inner join actor_id on films.id = actor_id.film_id inner JOIN actors on actors.id=actor_id.actor inner join directors on directors.film_id=films.id order by title;
select concat (title, ' year ', year) as 'Film and Year', actors.fullname as 'actors fullname', directors.fullname as 'Directors fullname' from films inner join actor_id on films.id = actor_id.film_id inner join actors on actors.id = actor_id.actor inner join directors on directors.film_id = films.id where dues > 200000000 order by actors.fullname limit 2,3;
