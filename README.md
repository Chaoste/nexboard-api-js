# nexboard-api-js

[![Greenkeeper badge](https://badges.greenkeeper.io/schul-cloud/nexboard-api-js.svg)](https://greenkeeper.io/)

## Useage

```javascript
Nexboard = require("nexboard-api-js");

nex = new Nexboard(ApiKey, UserID, Url);
```
### params 
- `ApiKey` = The identification key from account.
- `UserId` = The Id from user.
- `Url`= the URL of the API interface. If zero the value is set to [default](https://nexboard.nexenio.com/portal/api/v1/public/)

### functions
```javascript
nex.getProjectsIDs();
```
retun a list of IDs from all projects.


```javascript
nex.createProject(
    "Title of project" , 
    "description of project");
```
create an new project and return it. 

```javascript 
nex.createBoard(
    "Title of Board" , 
    "description of Board", 
    IdOfProjectFromThisBoard);
```
create an new board and return it. 
    
```javascript
nex.getBoardsByProject(ProjectId));
```
return all boards from Project.

```javascript
nex.getBoard(BoardId));
```
return the board object from ID.