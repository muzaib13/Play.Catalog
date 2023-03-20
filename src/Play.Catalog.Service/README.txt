1. Setup the project. (Catalog Microservice)
	- dotnet new webapi -n 'Play.Catalog.Service' --framework net5.0

2. Build the project
	- dotnet build
3. Run the Project
	- dotnet run
4. Install dev trust certificate
	- dotnet dev-certs https --trust
5. Delete default template files from the project.

6. Create DTOs 

7. Create an Catalog Items Controller

8. Implement Get Methods

9. Create DTOs (record types)

10 Implement POST, PUT and Delete

11. Implement Repository Pattern --> MongoDB as Database
	- Why MongoDB ? 
	NoSQL solution is preferred for our microservice because: 
		- Won't need relationships across the data.
		- Don't need ACID (Atomicity, Consistency, Isolation and Durability ) guarantees.
		- Wouldn't have to write complex queries
		- Need low latency, high availability and high scalability.

12. Implement CRUD methods in the Repository class.

13. Install mongodb in Docker
	- docker run -d --rm --name mongo -p 27017:27017 -v mongodbdata:/data/db mongo (Docker can throw TLS handshake timeout error: It can be due to slow Internet Collection, Retry installing multiple times)

	