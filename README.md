# splunk-apache-recon
## Project: Web Reconnaissance Detection with Splunk

### Objective
Analyze Apache web access logs to identify suspicious reconnaissance activity.

### Data Source
- Apache access logs
- Ingested into Splunk (access_combined sourcetype)

### Detection Logic
- Queried HTTP status codes 401, 403, and 404
- Reviewed requests to restricted paths such as /admin and /login
- Identified unauthenticated and automated access attempts

### Findings
- Multiple source IPs probed restricted endpoints
- Observed failed authentication and forbidden responses
- Activity consistent with web reconnaissance
- Activity assessed as web reconnaissance rather than successful compromise

### Tools Used
- Splunk Enterprise
- Apache access logs
