# Tasks

## Prepare the pets DB

1. Open the pgAdmin Desktop client or the Web interface.
2. Connect to the database according to the `README.md`.
3. Right click to `Databases`, select `Create...`.
4. Give a name to the database in the `Database` field, e.g. `pets`.
5. Right click to the created database `pets` and select `Query Tools`.
6. In the opened editor paste the content of the `pets.sql`.
7. Execute the query with the Execute script (▶️ "play") button.

To check if the data is inserted properly:

- Open `pets` db, `Schemas`, `public`, `Tables`.
- Right click on a table, e.g. `pets`, select `View/Edit data`, `All Rows`.

On a given database anytime you can open the `Query Tools` to execute queries
on the database.

## Task 1: Insert, delete, update (Data manipulation)

Create queries to execute the following tasks.

Save the queries to the `task1.sql`.

- Add yourself to the database.
- Add your pet or your imaginary pet to the database.
- Your pet name is not respectful enough. Change it names by adding a "Mr." in front of it.
- Increase every pets' age if they are older than 5 years.
- Remove Simba from the database.

### Background material

- https://www.postgresql.org/docs/17/dml.html

## Task 2: Practice some basic queries (Data Query)

Create queries to execute the following tasks.

Save the queries to the `task2.sql`.

- Show only all pets' name, age and weight only.
- Order the previous list by pet age, the oldest pet should be the first.
- Order the list by age (oldest first), and if the two animal have the same age show the heaviest first.
- List 2nd, 3rd, 4th heaviest pet.
- Select only the pets if they are at least 5 years old and heavier than 5 kilos.
- Get all the unique owner IDs (use the pets table only for this).
- Find the pets who lives in the wild (does not have any owner). 


### Background material

- https://www.postgresql.org/docs/17/queries.html


## Task 3: Practice the joins (Data Query)

- Show the pet's kind's name next to the pet.
- Match made in heaven: Show the pet's owner's name next to the pet. Show only the pets who has an owner.
- Wild pets among us: Show the pet's owner's name next to the pet. Show those pets too who does not have an owner (but do not show the owners who does not have pets).
- Free/Lonely owners: Show the pet's owner's name next to the pet. Show those owners too who does not have a pet (but do not show the pets who does not have an owner).
- The matchmaking show: Show the pet's owner's name next to the pet. Show all the pets and owners even if they do not have owner/pet.

### Background material

- https://www.postgresql.org/docs/17/queries-table-expressions.html

## Task 4: Practice the grouping (Data query)

- Count how many pets we have.
- Count how many pets belongs to each kind. Show a counter and the kind name next to each other.
- Order the previous list by count, ascending.
- Measure the summarized weight of each kind. Show the sum of the weight and the kind's name next to each other.
- Show only the kinds from the previous list where the summarized weight is heavier than 10 kg.
- Find out the pet lady/lord! Find the owner who has the most pets. Show only their name, and the number of pets.
- Find out the *cat* lady/lord! Find the owner who has the most *cats.* Show only their name, and the number of *cats*.
- Count the average age by of the pet's grouped by owner.

### Background material

- https://www.postgresql.org/docs/17/queries-table-expressions.html#QUERIES-GROUP

