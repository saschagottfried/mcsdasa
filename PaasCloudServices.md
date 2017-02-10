# Cloud Services

Sizes
- [Sizes for Cloud Services](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-sizes-specs#sizes-for-web-and-worker-role-instances)



# Cloud Service Configuration 

Schema
- [Reference](https://msdn.microsoft.com/en-us/library/dd179398.aspx)

## Endpoints
- input endpoint
- Instance input endpoint
- Internal endpoint

## Network Traffic rules

- [Enable communication for role instances in azure](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-enable-communication-role-instances)

## Some communication scenarios
- [Network traffic rules to control role communication](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-enable-communication-role-instances#network-traffic-rules-to-control-role-communication)


## Role lifecycle


## Startup task
- [How to configure and run startup tasks for a cloud service](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-startup-tasks)
- [Common startup tasks](https://docs.microsoft.com/en-us/azure/cloud-services/cloud-services-startup-tasks)

startup tasks run again when roles restarts/recycles

## Local Storage


## Diagnostics
scheduledTransferLogLevelFilter
- Specifies the minimum severity level for log entries that are transferred

scheduledTransferPeriod
- Specifies the interval between scheduled transfers of data, rounded up to the nearest minute

# Deployment

3 components
- Service definition .csdef
- Service configuration .cscfg
- service package .cspkg
  -  zip file that contains all of the required binary-based dependencies.
  - You can use the CSPackcommand-line tool (installed with the Azure SDK) to create the package file as an alternative to Visual Studio


## Schema

<WebRole/>
  <Sites />
  <ConfigurationSettings>
  <Endpoints>
</WebRole>
<WorkerRole/>
  <InputEndpoints/>
  <InstanceInputEndpoints/>
  <InternalEndpoints/>
  <ConfigurationSettings/>
  <Certificates/>
  <LocalResources/>
  <Imports/>
  <Startup/>


