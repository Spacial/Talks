# Some toughts

Secure Coding 

👉SAST should be run early in the SDLC. The test reveals vulnerabilities in the code, specifically those in the OWASP Top 10 like SQL injection.
👉SCA with composition analysis scans software, and its dependencies display a list of known vulns and notes any deprecated dependencies.
👉Secure Code Review is a specialized task involving manual/auto review of an app source code to identify security-related code.

Build and Test

👉Container and Image Scan checks the build process of your containers and images for vulns. 
👉DAST for compiled code / a running app without knowledge of the environment, simulating an attack. 
👉Fuzzing the unexpected inputs. It should test if a non-date is entered in a date field or drop a binary file in a text field. 
👉An IAST tests the running apps for vulns during use, similar to a DAST. Can identify the line of code that is the source of a particular exposure.

Delivery and Deploy

👉Sign Verifies both the signature of the code and that the code has not been tampered with. 
👉Artifacts and Image Repository Scan all the artifacts created during development for vulnerabilities, and an image repository scan images when they are pushed to a repository. 

Run Defense

👉Monitoring systems, containers, and networks for known vulnerabilities with observability tools.
👉RASP works by adding sensors into the code so that execution points watch for exploits happening in real-time.
👉Attack simulation can be done either black box or white and on the apps, services, systems, networks, etc.

Credit:[PagerDuty](https://www.linkedin.com/posts/elishlomo_cybersecurity-cloudcomputing-activity-6851390002375471104-jQ_K/)
