# Oi, what's the big idea here?

• Provides a web app accessible tool for creating parties, importing characters from D&D Beyond’s Character API, and then tracking the party’s gains for game management purposes. Uses a Django backend fed API to generate the React front end with user authentication and character imports.
It stems from this google sheet we use to track what stuff our adventure group has accrued, and I've always wanted to make it more useful than a spreadsheet. I figure the base goal of "do this excel sheet but better" is achievable, and then you can add some additional queries, like easily filtering by character, or non-magical items, etc.

CRUD: A party has characters (added manually or via API above) and items. Items can be associated to characters, but are a subset of the party.
### APIs:
APIs: D&DBeyond Character API (for pulling character data) and Auth0 (for log in/authentication)
D&D Beyond Character Service:  https://character-service.dndbeyond.com/character/v3/character/{CharacterId}
Auth0: React and Django APIs: https://manage.auth0.com/

