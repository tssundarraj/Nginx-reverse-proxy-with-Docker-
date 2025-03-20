# Reverse Proxy Overview

## [What is a Reverse Proxy?](#what-is-a-reverse-proxy)
A **reverse proxy** is a server that stands between client devices and one or more backend servers. It intercepts incoming client requests and forwards them to the appropriate backend server(s). Once the backend server processes the request, the reverse proxy sends the response back to the client. This setup helps shield the internal network details while providing additional features like load balancing, caching, and SSL termination.

## [Why is it Called a Reverse Proxy?](#why-is-it-called-a-reverse-proxy)
It is called a reverse proxy because it acts on behalf of the server rather than the client. In contrast to a forward proxy—where clients use the proxy to access external resources anonymously—a reverse proxy receives external requests and “reverses” the flow by routing them to internal servers. This effectively hides the details of the backend infrastructure from the clients.

## [Problems Solved by a Reverse Proxy](#problems-solved-by-a-reverse-proxy)
Reverse proxies address several critical issues:
- **Load Balancing:** Distributes incoming traffic evenly among multiple backend servers, preventing any single server from becoming overwhelmed.
- **Security and Anonymity:** Conceals the identities and IP addresses of backend servers, reducing the risk of direct attacks.
- **SSL Termination:** Offloads the SSL/TLS encryption and decryption processes from backend servers, simplifying certificate management and reducing server load.
- **Caching and Optimization:** Caches frequently requested content to reduce latency and speed up response times.
- **Centralized Access Control:** Provides a single point to implement security policies, manage authentication, and log requests before they reach the backend services.
