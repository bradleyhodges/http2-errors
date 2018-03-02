# http2-errors (7XX Class Errors)
### A set of standard http error codes in the 7XX range
Advena is a developer-oriented company, and as part of that, we believe that it's our responsibility to provide developers with tools that help them in the long run. There has not been a major revision to http status codes since 2014, and before then, it wasn't until 1997 that a major revision occured.

We've noticed this divide in http status codes, and have developed our own version of 7XX codes to help developers understand exactly what the problem is. These codes are primarily used internally, on Advena products and services, but you're welcome to use them under our Creative Commons Attribution Share Alike 4.0 license.

---

# 7XX Codes

  * 70X - Internal Errors
    - 701 - Internal Handling Exception
    - 702 - Expected Exception
    - 703 - Failed to Update
    - 704 - Content Not Acceptable
    - 705 - Internal Allocation Exception
    - 706 - Execution Error
    - 707 - Storage Allocation Error
    - 708 - Documented, Undisclosed Internal Exception
    - 709 - Undocumented Exception
    
  * 71X - External Errors
    - 710 - External Service Returned Error
    - 711 - External Service Returned Unexpected Response
    - 712 - External Content Unreachable
    - 715 - External Service Unreachable
    - 719 - External Content Redirected Unexpectedly
    
  * 72X - Edge Cases
    - 720 - Timed Out
    - 721 - Not possible
    - 722 - Edge Cache Failure
    - 723 - Undocumented Infrastructure Failure
    - 725 - Unexpected Infrastructure Failure
    - 726 - Expected Infrastructure Failure
    - 727 - Not Responding
    - 728 - Server Failed to Complete the Request
    - 729 - Example Content
    
  * 73X - Generalised Errors
    - 730 - Timeout Occurred
    - 731 - Content Not Found
    - 732 - Not Allowed
    - 733 - Content Not Allowed (See: 704)
    - 734 - User Not Authenticated
    - 735 - Access Denied
    - 736 - Parameters Returned 0 Results
    - 737 - Forbidden
    - 738 - Syntax Error
    - 739 - Compiling Exception
    
  * 74X - Caching Exceptions
    - 740 - Cache Expired
    - 741 - Cache Expected
    - 742 - Edge Cache Not Responding
    
  * 75X - Binary Responses
    - 750 - Okay
    - 751 - No
    - 752 - Yes
    
  * 76X - Security Responses
    - 760 - Violated Policy
    - 761 - Request Rejected for Security
    - 762 - Refused to Fulfill Request
    - 763 - Client is Blocked
    
  * 77X - DNS Errors
    - 770 - DNS Format Error
    - 771 - DNS Query Error
    - 772 - Server Failed to Complete the DNS Request
    - 773 - Domain Name Does Not Exist
    - 774 - Server Refused to Connect
    - 775 - Server Not Authoritative for the DNS Zone
    - 776 - Timed out
    - 777 - Unexpected Result (DNS)
    - 778 - Server Unreachable
    - 779 - Client Unreachable
    
  * 78X - Content Errors
    - 780 - Content Ended Unexpectedly
    - 781 - Expected Character(s) Missing
    - 782 - Content Incorrectly Encoded
    - 785 - Unexpected Content
    - 788 - Content Length is Invalid
    
  * 79X - API Errors
    - 790 - API Not Available
    - 791 - Invalid Scope
    - 795 - API Service Error
    - 796 - Invalid/Missing Parameter

---

# License
You can read more about the Creative Commons Attribution Share Alike 4.0 license here: https://choosealicense.com/licenses/cc-by-sa-4.0/.

![Creative Commons Attribution Share Alike 4.0](https://i.gyazo.com/554cbca59c9e31b027f042d766d5f3da.png)

---

# Implementation
To properly indicate the results of the error, use these code examples.

### PHP 7(>?)
```php
@http_response_code(729);
@header("X-Advena-Error: 729");
die("729 - Example Content. Explain error here"); // Not required - will end code execution.
```

### Apache 2(.2+)
```apache
Redirect 729 /
```

### Node.JS
```nodejs
res.status(729);
res.send('Example Content');
```
