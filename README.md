# 🚀 Employee Management System Web API

A **.NET Core-based RESTful API** for managing employees and users with authentication, role-based access, and CRUD operations.  

---

## 📌 Features  
✅ JWT Authentication & Authorization  
✅ Role-based Access Control (Admin, HR, Employee)  
✅ Secure Password Hashing  
✅ Employee CRUD Operations  
✅ Entity Framework Core Integration  
✅ Exception Handling & Validation  

---

## 📂 Project Structure  

```
Employee_Management_System_API/
│── Controllers/
│   ├── AuthController.cs
│   ├── EmployeeController.cs
│── Data/
│   ├── ApplicationDbContext.cs
│── DTOs/
│   ├── UserLoginDTO.cs
│   ├── UserRegisterDTO.cs
│── Helpers/
│   ├── JwtHelper.cs
│── Models/
│   ├── Employee.cs
│   ├── User.cs
│── Repositories/
│   ├── EmployeeRepository.cs
│   ├── UserRepository.cs
│── Services/
│   ├── EmployeeService.cs
│   ├── UserService.cs
│── appsettings.json
│── Program.cs
```

---

## ⚙️ Setup & Installation  

### 🔹 1️⃣ Clone the Repository  
```sh
git clone https://github.com/YourUsername/Employee_Management_System_API.git
cd Employee_Management_System_API
```

### 🔹 2️⃣ Install Dependencies  
```sh
dotnet restore
```

### 🔹 3️⃣ Set Up Database  
```sh
dotnet ef migrations add InitialCreate  
dotnet ef database update  
```

### 🔹 4️⃣ Run the Application  
```sh
dotnet run  
```

---

## 🔑 API Endpoints  

### 🔹 Authentication  
| Method | Endpoint             | Description        |
|--------|----------------------|--------------------|
| POST   | `/api/auth/register` | Register a user   |
| POST   | `/api/auth/login`    | Login & get token |

### 🔹 Employees  
| Method | Endpoint              | Description         |
|--------|----------------------|---------------------|
| GET    | `/api/employees`      | Get all employees  |
| GET    | `/api/employees/{id}` | Get employee by ID |
| POST   | `/api/employees`      | Add a new employee |
| PUT    | `/api/employees/{id}` | Update employee    |
| DELETE | `/api/employees/{id}` | Delete employee    |

---

## 🎯 OOP Concepts Used  

✅ **Encapsulation** – Secure data in `Employee` & `User` models  
✅ **Abstraction** – Interfaces like `IEmployeeRepository`  
✅ **Inheritance** – Common properties in `BaseEntity` class  
✅ **Polymorphism** – Dependency injection for repositories  

---

## 💡 Contributing  

1. Fork the repository  
2. Create a new branch (`feature-xyz`)  
3. Commit your changes  
4. Push to the branch  
5. Create a pull request  

---

## 🚀 Happy Coding! 🎉


