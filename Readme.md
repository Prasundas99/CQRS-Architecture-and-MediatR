CQRS (CQS)
CQRS is short for Command Query Responsibility Segregation, while CQS is short for (Command Query Segregation). CQS is a code pattern that segregates GET response into one flow (query flow) and writing or updating request (POST, PUT, PATCH, DELETE) into another flow (command flow). CQRS is an architectural pattern that requires a read database for query flow and write database for command flow.

Read database can be fully optimized for read (with all indexes that will increase read speed, etc.), while write database is optimized for data updates and insertions.

How do MediatR and CQRS fit together?

MediatR fits perfectly in the application layer of the CQRS schema, but don t just take my word for it. These two combined will give your application the best read-write performances, thin controllers, and handlers that will have a single responsibility.