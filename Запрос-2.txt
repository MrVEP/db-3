CREATE TABLE IF NOT EXISTS Worker (
	id serial primary key,
	name varchar(40) unique not null,
	department_id integer,
	boss integer references Worker(id)
);