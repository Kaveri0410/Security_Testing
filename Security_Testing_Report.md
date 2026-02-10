SECURITY TESTING REPORT

1. SQL Injection

Test Location:
Login Page

Payload Used:
' OR '1'='1

Result:
Login was bypassed and admin access was granted.

Status:
Vulnerable


2. Cross Site Scripting (XSS)

Test Location:
Feedback Form

Payload Used:
<script>alert('XSS')</script>

Expected Result:
Alert popup should appear.

Actual Result:
Form was submitted successfully but script execution was blocked.
No alert popup was displayed.

Conclusion:
The application is not vulnerable to XSS at this point.
