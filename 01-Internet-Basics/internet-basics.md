# Internet Basics

## Why Learn Internet Basics?

Before learning Node.js or Express.js, it is important to understand how applications communicate over the internet. Every backend application receives requests from clients, processes them, interacts with a database if required, and sends responses back to the client.

---

# 1. What is Backend?

Backend is the part of an application responsible for processing requests, implementing business logic, communicating with databases, and returning responses to the client.

### Example

When you log in to Instagram:

- You enter your username and password.
- The browser sends a request to the backend.
- The backend verifies your credentials using the database.
- A response is sent back indicating whether the login was successful.

---

# 2. Client and Server

### Client

A client is any application or device that sends a request.

Examples:

- Web Browser
- Mobile Application
- Desktop Application

### Server

A server is a computer that is always connected to the internet. It receives client requests, processes them, and returns the appropriate response.

---

# 3. Request and Response

Communication between a client and a server happens in two steps:

1. The client sends a **Request**.
2. The server processes the request and sends a **Response**.

Example:

Browser → "Show me the YouTube homepage."

Server → Returns the YouTube homepage.

---

# 4. What Happens When You Open google.com?

```text
You
 │
 ▼
Type google.com
 │
 ▼
Browser
 │
 ▼
DNS
 │
 ▼
IP Address
 │
 ▼
Server
 │
 ▼
Backend
 │
 ▼
Database
 │
 ▼
Response
 │
 ▼
Browser
```

---

# 5. DNS (Domain Name System)

DNS converts a domain name into its corresponding IP address.

Example:

```
google.com
      ↓
142.xxx.xxx.xxx
```

Think of DNS as the **phonebook of the Internet**.

---

# 6. IP Address

An IP Address is the unique address of a device or server on a network.

Example:

```
142.250.xxx.xxx
```

Computers communicate using IP addresses instead of domain names.

---

# 7. HTTP vs HTTPS

| HTTP | HTTPS |
|------|-------|
| HyperText Transfer Protocol | HyperText Transfer Protocol Secure |
| Data is sent in plain text | Data is encrypted |
| Less secure | More secure |
| Uses Port 80 | Uses Port 443 |

---

# 8. HTTP Methods

| Method | Purpose |
|---------|---------|
| GET | Retrieve data |
| POST | Create new data |
| PUT | Update existing data completely |
| PATCH | Update part of existing data |
| DELETE | Remove data |

---

# 9. HTTP Status Codes

| Code | Meaning |
|------|---------|
| 200 | OK |
| 201 | Created |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Server Error |

---

# 10. Why Do We Need a Database?

A database stores and manages application data efficiently.

Instead of storing users, posts, products, or comments inside the server code, applications store them in a database. The backend retrieves and updates this data whenever required.

---

# 11. Backend Flow

```text
Client (Browser)
        │
        │ Request
        ▼
Backend Server
        │
        ▼
Database
        │
        │ Response
        ▼
Client (Browser)
```

---

# Key Takeaways

- The browser always sends the first request.
- Servers process requests and return responses.
- DNS converts domain names into IP addresses.
- The backend communicates with databases.
- Clients never communicate directly with the database.

---

# My Understanding

I learned that backend acts as the bridge between the client and the database. The browser sends a request to the backend, the backend processes the request, retrieves or updates data if needed, and returns the appropriate response to the client.
