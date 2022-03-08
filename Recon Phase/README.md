# Web-Application-Penetration-Testing
In This Repository I M Gonna Tell You About How To Penetrate Web-Application Test Step By Step.
#  Starting With Recon Phase(Unauthorized Access).
    
      1:- Resolve Dns Records Name Using dig Command.
      2:- IP To Location.
      3:- Nmap Don't Ping Scan.
      4:- Nmap Service Version, Detection.
      5:- Enumerate Supported HTTP Methods Using Nmap.
      6:- Checking SSL And TLS Versions Using Nmap.
      7:- Host Header Injection.
      8:- Waybackurls.
      9:- Whatweb.
     10:- Find Hidden Web Directories With Dirsearch.

 1- Resolve DNS Records name using dir.
                                                                                                                                                                   
    # dig (doamin name)+Mx
    # dig (doamin name)+SOA
    # dig (doamin name)+ANY
    # dig (doamin name)+noall 
    # dig (doamin name)+noall+answer
    # dig (doamin name)+short
                           
 2- IP To Location.

   https://www.iplocation.net/
    
   https://iplocation.com/
    
   https://tools.keycdn.com/geo
    
   https://ipinfo.io/
    

 3- Nmap Don’t Ping Scan.

    # nmap -Pn <Target IP ADDRESS>
    
![image](https://user-images.githubusercontent.com/80889609/157229641-d0f5221b-665c-45e0-9a9d-ad57ab20aeba.png)


 4- Nmap Service Version Detection.

     # nmap -sV <Target IP ADDRESS>

![image](https://linuxhint.com/wp-content/uploads/2020/02/2-14.png)

 5- Enumerate Supported HTTP Methods Using Namp.
    
    # nmap --script http-methods <Target IP ADDRESS> 
 ![image](https://user-images.githubusercontent.com/80889609/157235359-21cfe1d2-82fb-4fda-a73f-f4136121cdb7.png)
 
    # nmap --script http-methods --script-args http-methods.url-path='/website' <Target IP ADDRESS>
    
       
 6- Checking SSL And TLS Versions Using Nmap

    # nmap --script ssl-cert -p 443 <Target IP ADDRESS>
 ![image](https://user-images.githubusercontent.com/80889609/157234643-b2c056ce-79bd-4e38-8414-b8215d083963.png)
   
     # nmap --script ssl-enum-ciphers -p 443 <Target IP ADDRESS>
  ![image](https://user-images.githubusercontent.com/80889609/157234248-ef99de4f-afc3-4bde-929a-50286c7744f9.png)

 7- Host Header Injection.
 
      # nmap -sV --script=http-headers <Target IP ADDRESS>
 ![image](https://user-images.githubusercontent.com/80889609/157235255-ea91f2aa-093a-4c2d-8383-60d5fdf6f8fb.png)

    
 8- Waybackurls.

     # waybackurls <Target Website URL>

 9- Whatweb.

     # whatweb <Target Website URL>

 10- Find Hidden Web Directories with Dirsearch.
        
     # dirsearch -u <Target Website URL>
 
 
     
