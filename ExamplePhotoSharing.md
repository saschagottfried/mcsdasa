Load Balancing

- DNS 
- Round robin
- HTTP (Layer7): Stickiness, SSL offloading


## Web Hosting Performance

- Asynchronous requests and response
  - ASP.NET thread pool can handle more requests
- Task Parallel Library (TPL) - await/async keywords
- Multi-core startup (JIT)
- Windows prefetcher for web application


## ASP.NET Session State

- InProc
- StateServer (WebFarms vs. WebGarden)
  - <sessionState mode="StateServer" stateConnnectionString=""/>
- SqlServer
  - <sessionState mode="SQLServer" stateConnectionString="Data Source=tcp:ServerName.database.windows.net,1433;Initial Catalog=DatabaseName;Integrated Security=False;UserId=username@servername;Password=password"/>
- Custom
  - <sessionstate mode="Custom" stateConnectionString="">
      <providers></providers>

Flexible options by Provider pattern
- [ASP.NET Session State Provider for Azure Redis Cache](https://github.com/Microsoft/azure-docs/blob/master/articles/redis-cache/cache-aspnet-session-state-provider.md#aspnet-session-state-options)


Refs
- http://www.alachisoft.com/ncache/session-index.html
  
