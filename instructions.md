# Hi-Score Tracker

## Important Resources
- [HiScore Tracker](./README.md)

## Time
- 4-6 hours

### Description
Hi-Score Tracker is a small REST API. You are tasked with building a REST API to track hi scores for a Pacman game. The REST API can store the scores in memory, for instance using a Map in Java or a dicitonary in Python. The REST API does not need to follow all 6 REST contraints. While REST APIs support can support various formats this application should use JSON. You will make your own app but should seek help from each other.

### Main Goals
- Get familiar interacting with RESTful endpoints
- Inernalize REST APIs as a way to track a resource
- Understand RESTful naming conventions
- Understand JSON as a format for transporting information
- Create a mental model seperating client and server

## Associate Instructions
1. You have recieved the link to the ScoreTracker Bounty (it's what is listed in the README.md)
2. Create your own project and attempt to implement the routes
3. Upload your code to Github

### Routes to Implement
```text

    POST /scores => creates a new score

    GET /scores => Returns all scores
    GET /scores?initials={AAA} => Returns all scores by that player
    GET /scores/{id} => Returns the score with that id 

    PUT /scores/{id} => Replaces the score with that ID

    DELETE /scores/{id} => Deletes the score with that ID

```

### Important Notes
- Since we are now working with data as Objects (i.e. the Score Object has properties: id, initials, and points), think about how you are going to store that information.
  - you may want to define a Score class in your application.

### Stretch Goals / Additional Features to add 
- Only after you've implemented the above routes!
  - Validate that all initials are 3 letters
    - return a 422 otherwise
  - Change all intials to uppercase when posted
  - Add the ability to sort by ascending and descending query params
  - Try using File IO to save the scores in a persistent way

```json
{"id":101, "initials":"AAA", "points":234900}
```


