# API_Driven_Data_Enricher


<img width="913" alt="image" src="https://github.com/user-attachments/assets/f38fadfb-3bbd-4972-ae0c-efe4f447fd60" />



This integration flow includes:

🔹 HTTPS Sender Adapter – Triggered securely via Postman to simulate real-time data submission.
 🔹 XSLT Mapping – Transformed incoming XML to a required normalized structure.
 🔹 Content Modifier – Extracted key values from the payload and stored them as headers and properties.
 🔹 Local Integration Process – Performed field validation using Groovy; throws errors if essential data is missing.
 🔹 Content Enricher – Enriched the message by calling the Northwind OData API and merging external data into the main stream.
 🔹 Groovy Script – Logged the transformed payload for debugging and traceability.
 🔹 Data Store (Write) – Persisted the final output using the Data Store Operation for backup and audit purposes.
 🔹 Exception Subprocess – Handled exceptions gracefully and ensured error messages were stored properly.
