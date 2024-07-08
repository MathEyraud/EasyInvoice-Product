# Project EasyInvoice
## EasyInvoice Product (product)
### Description:
The 'product' microservice is responsible for managing product-related information. It provides APIs for creating, retrieving, updating, and deleting products. This service communicates with the 'invoice' microservice to provide product data required for invoice creation.

### Key Features:
- RESTful APIs for product management.
- Inter-service communication with invoice service using WebClient.
- Integration with invoice-core for entity definitions.

## Integration Overview
EasyInvoice is designed as a microservices architecture where each service has a distinct responsibility. The invoice-core module provides the shared entity definitions, while the customer, invoice, and product services handle their respective domains. The service-discovery module facilitates dynamic discovery and communication among these services.
- Customer Service: Provides customer data to the Invoice service. https://github.com/MathEyraud/EasyInvoice-Customer
- Invoice Service: Manages invoices and retrieves necessary customer and product data from respective services. https://github.com/MathEyraud/EasyInvoice-Invoice
- Product Service: Supplies product information to the Invoice service. https://github.com/MathEyraud/EasyInvoice-Product
- Service Discovery: Ensures all services can discover and communicate with each other. https://github.com/MathEyraud/EasyInvoice-ServiceDiscovery
- Invoice Core: https://github.com/MathEyraud/Java-Learn-Spring-Data-Core/tree/Microservices
This architecture ensures scalability, modularity, and ease of maintenance, making EasyInvoice a robust and flexible invoicing solution.
