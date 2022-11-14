# HiScoreTracker
You have been tasked with creating a REST API to track scores in Pacman. A score JSON looks like this. When you are finished you should push your project to Github.
```json
{"id":101, "initials":"AAA", "points":234900}
```
These are the routes to implement

### Routes to Implement
```text
    POST /scores => creates a new score

    GET /scores => Returns all scores
    GET /scores?initials={AAA} => Returns all scores by that player
    GET /scores/{id} => Returns the score with that id 
      => Returns 404 if score with ID not found

    PUT /scores/{id} => Replaces the score with that ID
      => Returns 404 if score with ID not found

    DELETE /scores/{id} => Deletes the score with that ID
      => Returns 404 if score with ID not found
```
