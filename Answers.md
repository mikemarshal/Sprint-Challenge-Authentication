<!-- Answers to the Short Answer Essay Questions go here -->

# 1.  Describe Middleware, Sessions (as we know them in express), bcrypt and JWT.
# 2.  What does bcrypt do in order to prevent attacks?
# 3.  What are the three parts of the JSON Web Token?

# 1) Middleware are functions that are used to offload some word from the express routes.. you can change the req/res objects before they reach the route with middleware. Sessions are log-in instances that are created and do not go away if you refresh the page (also can be used for authentication). Bcrypt encrypts/hashes your passwords. Json web tokens are used to send secure information between two computers.
# 2) Bcrypt salts passwords and creates a hashed password. This is a one way process, if someone was able to obtain your hashed password and tried logging in with it, it would simply get hashed into a new password (hash of a hash) instead of allowing access to your account.
# 3) Header - has the token type and hashing algorithm, Payload - info about requestor and type of entity, Signature - ensures authentication is true from origin to destination.
