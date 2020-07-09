# SQL-2-MINI

1-Create a new table called movie with a movie_id, title, and media_type_id.
Make media_type_id a foreign key to the media_type_id column on the media_type table.
Add a new entry into the movie table with a title and media_type_id.
Query the movie table to get your entry.

create table movie(
movie_id serial primary key,
title varchar(50),
media_type_id int references media_type(media_type_id)
);

insert into movie(
  media_type_id,
  title

)values(
  3,
  'Hot Rod'
);

select * from movie;


2-Add a new column called genre_id that references genre_id on the genre table.
Query the movie table to see your entry.

