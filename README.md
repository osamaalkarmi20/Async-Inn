# Async-Inn
this is a simple api project that we will make on a several labs and it starts on the with the first lab 11 which will include the ERD(Entity Relationship Diagram:
## Digram:
![diagram](dirgram.png)
and here isthe link to it for more clearer view.
[diagram](dirgram.png)
## Explanation:

1. Location entity: Represents a hotel location.
   - `location_id`: Unique identifier for each hotel location.
   - `name`: Name of the hotel location.
   - `city`: City where the hotel is located.
   - `state`: State where the hotel is located.
   - `address`: Street address of the hotel.
   - `phone_number`: Contact phone number for the hotel location.

2. Room entity: Represents a hotel room.
   - `room_id`: Unique identifier for each hotel room.
   - `location_id`: Foreign key referencing the corresponding hotel location.
   - `room_number`: Room number of the hotel room.
   - `nickname`: Nickname given to the room for better differentiation.
   - `room_type`: Type of the room (e.g., one-bedroom, two-bedroom, studio).
   - `price`: Price of the room.
   - `pet_friendly`: Indicates whether the room is pet-friendly.

3. Amenity entity: Represents the amenities available in a room.
   - `amenity_id`: Unique identifier for each amenity.
   - `name`: Name of the amenity.

## Relationships:

- One location can have multiple rooms (one-to-many relationship): The `location_id` attribute in the Room entity is a foreign key referencing the primary key `location_id` in the Location entity.
- Each room can have multiple amenities (many-to-many relationship): The Amenity entity is related to the Room entity through an associative table that is not explicitly shown in the diagram.
## pure join Tables:
the Room_Amenity table serves as a pure join table, only consisting of foreign keys that reference the primary keys of the Room and Amenity tables. It does not include any additional attributes or payload information.


