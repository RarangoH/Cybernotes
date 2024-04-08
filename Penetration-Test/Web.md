# Web

### SQL Injection

    s


### Directory Traversal & Path Traversal
<p> Allows attacker to navigate through filesystem of running server</p>

    ../../../etc/passwd

### Local File Inclusion
<p>Allows attacker to insert and execute a file present in the target system</p>

    d
<code style="color : cyan">Note: the diference conceptually from directory traversal is that the application not only reads the file, but it includes the file in the application logic. 
<br>
<br>
If attacking webpage with a php file, when calling it by directory traversal it will only show the raw source code, while with file inclusion it will execute the php code.</code>

### Remote File Inclusion
    
    Note: difference between LFI and RFI, the resource that is inserted in the app logic is no taken from the file sistem of the server but can be taken from any webserver in the internet.

### OS Command Injection
<p>qpasa si hago esto </p>

    

### File Upload Vulnerability

    Allows attacker to upload files with malicious content
