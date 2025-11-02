[Postman] --(Login Request)--> [GitHub Login Page]
     ↑                               ↓
     ←--(Authorization Code)-- [GitHub]
     →--(Code + Secret)--> [GitHub Token URL]
     ←--(Access Token)-- [GitHub]
     →--(GET /user with token)--> [GitHub API]
     ←--(User Data)-- [GitHub]

🧠 Key learnings: -
Registered an OAuth client
*How to use Postman to test the complete OAuth 2.0 Authorization Code Flow
How to call a protected API using the Access Token
Exchanged a code for an access token
Client ID / Secret usage
Token-based authentication
Testing secured APIs using Postman

POSTMAN LINK: 
https://ankitkumar-2356106.postman.co/workspace/PYATB5X~6c73ff5a-90de-444d-a0c7-b5326cebbe4c/collection/44694445-2c780b0b-89ec-45f8-aba6-07f7dc7fc609?action=share&source=copy-link&creator=44694445

🧠 Key Testing Learnings
Concept	What to Test
Token Validity	Tokens expire; check expiry time
Scope Behavior	Try using token with less/more scopes
Unauthorized Access	Try API without token → should get 401 Unauthorized
Token Reuse	Use the same token again → should still work until expired
