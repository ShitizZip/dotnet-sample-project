# Order API — Interview Exercise

## Getting Started

This is a pre-configured ASP.NET Core 10 Web API project. The boilerplate is done — you just need to implement the API.

**What's already wired up:**

- EF Core **InMemory** database provider (registered in `Program.cs` as `AppDbContext`)
- **Swagger UI** at `/swagger` when running in Development mode
- An `Order` model in `Models/Order.cs`
- An empty `AppDbContext` in `Data/AppDbContext.cs`
- An empty `OrdersController` in `Controllers/OrdersController.cs`

### Prerequisites

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)

### Run

```bash
cd OrderApi
dotnet run
```

The API will start on `http://localhost:5050`. Open `http://localhost:5050/swagger` to explore your endpoints.

---

## Task

Build a simple **Order Management API** with the following endpoints:

### `POST /orders`

Accepts an order in the following JSON format:

```json
{
  "item": "Widget",
  "qty": 3,
  "price": 9.99
}
```

Stores the order and returns an appropriate response.

### `GET /orders/{id}`

Retrieves a previously created order by its identifier.

---

## Verify Your Work

An integration test suite is included. Run it to check your implementation:

```bash
dotnet test
```

---

**Time limit:** 30 minutes. Focus on correctness and good API design practices.
