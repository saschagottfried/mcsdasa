# Azure App Services

- Web Apps
- Mobile Apps
- Logic Apps
- API Apps


App Service Plans
- specific for a region



Traffic Manager
- DNS load-balancing for Web Apps in multiple regions



## Basics

App Service Plan Tiers

- Free
  - 1 GB Storage
- Shared
  - Custom domains
- Basic
  - manual auto scale
  - SSL
- Standard
  - Daily Backup
  - SSL
  - 5 Deployments Slots
  - auto scale
  - traffic manager
  
- Premium
  - 20 deployment slots
  
- App Service Environment
  - [Introduction to App Service Environment](https://docs.microsoft.com/en-us/azure/app-service/app-service-app-service-environments-readme)
  
  
App Services
- Logic Apps (connect with IFTTT)
- API Apps (needs Swagger)
   

Comparison
- [Azure App Service, Virtual Machines, Service Fabric, and Cloud Services comparison](https://docs.microsoft.com/en-us/azure/app-service-web/choose-web-site-cloud-service-vm)



## Logic apps

Logic apps integrate your apps with cloud-based apps by using connectors

Core connectors
- 



## App Deployment methods in App Service


Example
- [ToDoApp](https://docs.microsoft.com/en-us/azure/app-service-web/app-service-deploy-complex-application-predictably)

Publish profile


Deploy to Azure (Kudu)


Deploy with Visual Studio



## Lesson 7 - Traffic Manager



## App Service on Linux

Customers can create web apps on Linux only within a Linux enabled App Service Plan and this App Service Plan can only host Linux-based web apps

- [Overview](https://docs.microsoft.com/en-us/azure/app-service/app-service-linux-readme)


