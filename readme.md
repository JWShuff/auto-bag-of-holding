# Oi, what's the big idea here?

- Provides a web app accessible tool for creating parties, importing characters from D&D Beyond’s Character API, and then tracking the party’s gains for game management purposes. Uses a Django backend fed API to generate the React front end with user authentication and character imports.

- It stems from this google sheet we use to track what stuff our adventure group has accrued, and I've always wanted to make it more useful than a spreadsheet. I figure the base goal of "do this excel sheet but better" is achievable, and then you can add some additional queries, like easily filtering by character, or non-magical items, etc.

### ___The To Do List___
1. [ ] Spin up Django
   - [ ] Models for: Items, Characters, Parties and keyed correctly related
   - [ ] Viewsets for Models
   - [ ] API Endpoints
   - [ ] Rough Auth?
1. [ ] Spin up React
1. [ ] Django serves API of Parties and Items to Front End
1. [ ] Prepare the whole mess for deployment on Heroku
1. [ ] React consumes API and displays party and item
1. [ ] CRUD Parties, Items, Characters from React
1. [ ] React Auth0 implemented for perms
1. [ ] Django API Auth0 implemented for perms
1. [ ] React DDB Character Service API Consumption and CRUD Characters in backend
1. [ ] Make it pretty

### CRUD:
A party has characters (added manually or via API above) and items. Items can be associated to characters, but are a subset of the party.

### APIs:
- D&D Beyond Character Service:  [D&DBeyond](https://character-service.dndbeyond.com/character/v3/character/{CharacterId})
- Auth0: React and Django APIs: [auth0](https://manage.auth0.com/)

### Resources:
Data used from [5e.tools](https://github.com/TheGiddyLimit/TheGiddyLimit.github.io) to populate item database.