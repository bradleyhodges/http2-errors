# http2-errors (7XX Range)
Advena is a developer-oriented company, and as part of that, we believe that it's our responsibility to provide developers with tools that help them in the long run. There has not been a major revision to http status codes since 2014, and before then, it wasn't until 1997 that a major revision occured.

We've noticed this divide in http status codes, and have developed our own version of 7XX codes to help developers understand exactly what the problem is. These codes are primarily used internally, on Advena products and services, but you're welcome to use them under our Creative Commons Attribution Share Alike 4.0 license.

### 7XX Codes

  * 70X - Internal Errors
    - 701 - Internal Handling Exception
    - 702 - Expected Exception
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
    
  * 73X - Generalised Errors
    - 730 - Timeout Occurred
    - 731 - Content Not Found
    - 732 - Not Allowed
    - 733 - Content Not Allowed (See: 704)
    - 734 - User Not Authenticated
    - 735 - Access Denied
    - 738 - Syntax Error
    - 739 - Compiling Exception
    
    
    
### License
You can read more about the Creative Commons Attribution Share Alike 4.0 license here: https://choosealicense.com/licenses/cc-by-sa-4.0/.

![Creative Commons Attribution Share Alike 4.0](https://i.gyazo.com/554cbca59c9e31b027f042d766d5f3da.png)
