# Use Case Diagram

## Actors
- **Admin**: Has full access to the system, including user management and system settings.
- **Analyst**: Has access to view data, import CSV, view anomalies, and manage investigations.

## Use Cases

### Authentication & Authorization
- Login to the system
- Logout of the system

### Transaction Management
- View transaction list
- Search and filter transactions
- View transaction details
- Import transactions from CSV (Analyst, Admin)

### Analytics & Reporting
- View executive dashboard
- View revenue analytics charts
- View revenue leakage breakdown
- View AI business insights
- Generate and download reports

### Anomaly & Investigation Management
- View detected anomalies
- Dismiss anomalies
- Create an investigation from an anomaly
- View active investigations
- Update investigation status
- Add notes to an investigation

### System Administration
- View audit logs (Admin only)
- Manage system users (Admin only)

## Mermaid Use Case Diagram
```mermaid
usecaseDiagram
    actor Admin
    actor Analyst
    
    Analyst --> (Login)
    Admin --> (Login)
    
    Analyst --> (Import CSV Transactions)
    Admin --> (Import CSV Transactions)
    
    Analyst --> (View Dashboard)
    Admin --> (View Dashboard)
    
    Analyst --> (Manage Investigations)
    Admin --> (Manage Investigations)
    
    Analyst --> (View AI Insights)
    Admin --> (View AI Insights)
    
    Admin --> (Manage Users)
    Admin --> (View Audit Logs)
```
