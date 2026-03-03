# FUTURE_CS-03
API Security Risk Analysis | Cyber Security Internship — Task 3
<br>
I recently completed a structured API Security Risk Analysis as part of my Cyber Security Internship, and I'm excited to share my key takeaways.
About the Assessment:
<br>
I conducted a read-only, non-exploitative security analysis on the JSONPlaceholder public API using Postman — inspecting endpoints, response headers, authentication mechanisms, and error handling behaviors.
<br>
Key Findings:
1. Unauthenticated Access to User Data (Medium Severity)<br>
The /users endpoint returned sensitive personal information — including names, emails, addresses, and phone numbers — with zero authentication required. In a production environment, this alone could trigger regulatory penalties and irreversible reputational damage.
2. Excessive Data Exposure (Medium Severity)<br>
Individual user profiles returned far more data than necessary — geographic coordinates, company metadata, and other fields with no practical client-side use. This violates the principle of data minimization, a core requirement under modern privacy regulations.
3. Unstructured Error Responses (Low Severity)<br>
While the API correctly returned 404 status codes for invalid resources, error responses lacked a standardized JSON format — an oversight that can complicate debugging and security monitoring at scale.
<br>
Core Recommendations:<br>
- Implement OAuth 2.0 or JWT-based authentication
- Apply strict response filtering — return only what's needed
- Standardize error responses with structured JSON formats
<br>
<br>
What this experience taught me:<br>
Security is not just about stopping attacks — it's about building systems that don't invite them in the first place. This hands-on task reinforced that authentication, authorization, and data minimization are non-negotiable pillars of any secure API architecture.
Grateful for the opportunity to apply real-world security thinking in a safe, ethical environment. Looking forward to growing further in this field.
<br>
Prepared using: Postman | API: JSONPlaceholder
<br>
<br>
Intern : Anusha Patil<br>
Date: Mrach 3, 2026
