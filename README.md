- It includes postman collection, file name: postman.json
- Role managament is based on pathing: prefix client requires role client, that must be included on any request as header.
- If no permissions, 401 is thrown.
- I used mock data as "repository services".
- Exceptions are captured so no 500 err should be expected as data-errors via controllers.
- Cors and CSRF are disabled just for speeding-up purposes.
- Project is ready to deploy with dev/test/prod envs.
- Used Spring Boot with initializer.
- Repo url is: https://github.com/d3sd1/prueba-23-09-spring
- Feel free to ask permissions for repo.
- Commented with JavaDoc.
- Ticket ID is not handled by repository as we expect SQL to manage it on the future...
- Used user_id header when there's JWT login needed as tmp solution to handle firewall.
- Operator should only comment their tickets, but we can't handle that constraint that easy yet.
- Constraints @NotNull, etc not implemented due to time... and no javax hibernate validation package.
- Tickets are not differenciated between clients and operators intentionally. We can make it easy scaling system ;))
- /admin/tickets should be paginated, I KNOW RIGHT!!
- IKR id's should not be duplicated but a relational system will handle this in the future. system is scalable and MVC prepared!!