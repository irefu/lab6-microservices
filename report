**_Irene Fumanal Lacoma 758325_**

#### 1. The two microservices are running and registered (two terminals, logs screenshots).

- Accounts (port 2222)
![Accounts running](images/accounts.png)


- Web
![web running](images/web.png)


#### 2. The service registration service has these two microservices registered (a third terminal, dashboard screenshots)
- Third terminal
![third terminal registration](images/registration_terminal.png)


- Dashboard screenshoot
![dashboard screenshot](images/dashboard.png)

#### 3. A second accounts microservice instance is started and will use the port 4444. This second accounts (4444) is also registered (a fourth terminal, log screenshots).

I have copied accounts service and I have called it _accounts2._ Then, I have modified _application.yml_ :

![accounts2 aplication.yml](images/accounts2.png)

I added a line in settings.gradle. 

![accounts2 gradle_settings](images/accounts2_gradle_added.png)

- The new service accounts2 is running in a forth terminal in the port 4444:
![accounts2 running](images/accounts2_running.png)

- We can see the new instance registered:
![accounts2 dashboard](images/dashboard2.png)

#### 4. What happens when you kill the microservice accounts (2222) and do requests to web? Can the web service provide information about the accounts again? Why?

We can see if we kill the microservice with port 2222 now it doesn't appear in Eureka dashboard:
![accounts killed dashboard](images/dashboard3.png)

The web service can provide information abour accounts as we can see:
![accounts service is ok](images/service_is_ok.png)

Accounts service in port 2222 was killed, but accounts service in port 4444 is alive so the web service provides information about accounts using that service.
It is working because I had a replica running and registered in eureka.