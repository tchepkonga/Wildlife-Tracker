# wildlife_tracker


## Description

- This is an app where you get to add animals and also animals that are endangered.
- Once an animal is sighted, a ranger can go ahead and record the sighting.
- One can then view all the available animals, endangered animals and sightings.


## Author

titus chepkonga (https://github.com/tchepkonga)

## Built with
- [Java](http://www.oracle.com/technetwork/java/index.html)
    * [Spark framework](http://sparkjava.com/)
- Postgresql Database

## Setup
- Clone or download repo from (https://github.com/tchepkonga/Wildlife-Tracker.git)
- Download latest version of `java` and `gradle`.
- from the parent directory, run `$ gradle build` then `gradle run`.
- Launch the program from your local server `http://localhost:4567` in your browser.
- In PSQL:

CREATE DATABASE wildlife_tracker;
\c wildlife_tracker;
CREATE TABLE animals (id INT PRIMARY KEY, name VARCHAR);
CREATE TABLE endangeredAnimals (id INT PRIMARY KEY, name VARCHAR, health VARCHAR, age VARCHAR);
CREATE TABLE sightings (id INT PRIMARY KEY, location VARCHAR, ranger name VARCHAR, sighting time VARCHAR );
CREATE DATABASE wildlife_tracker_test WITH TEMPLATE wildlife_tracker;

## KNOWN errors
functionality of viewing animals an endangered animals produces error 500 Internal Server Error sometimes

## Licensing
All the work included has been dedicated to the public domain by waiving all of my rights to the work, under
copyright law, including all related and neighboring rights, to the extent allowed by law.
You can copy, modify, distribute and perform the work, even for commercial
purposes, all without asking permission.
