# Prometheus.Client.AspNetCore

[![MyGet](https://img.shields.io/myget/phnx47-beta/vpre/Prometheus.Client.AspNetCore.svg)](https://www.myget.org/feed/phnx47-beta/package/nuget/Prometheus.Client.AspNetCore)
[![NuGet](https://img.shields.io/nuget/v/Prometheus.Client.AspNetCore.svg)](https://www.nuget.org/packages/Prometheus.Client.AspNetCore)
[![NuGet](https://img.shields.io/nuget/dt/Prometheus.Client.AspNetCore.svg)](https://www.nuget.org/packages/Prometheus.Client.AspNetCore)

[![Build status](https://ci.appveyor.com/api/projects/status/d5pdqedoxogmiun4/branch/master?svg=true)](https://ci.appveyor.com/project/PrometheusClientNet/prometheus-client-aspnetcore/branch/master)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/73abdf76e71f42dfb6887a15eafb250a)](https://www.codacy.com/app/phnx47/Prometheus.Client.AspNetCore?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=PrometheusClientNet/Prometheus.Client.AspNetCore&amp;utm_campaign=Badge_Grade)
[![License MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)



Extension for [Prometheus.Client](https://github.com/PrometheusClientNet/Prometheus.Client)


#### Installation:

     dotnet add package Prometheus.Client.AspNetCore

#### Quik start:

There are [Examples](https://github.com/PrometheusClientNet/Prometheus.Client.Examples/tree/master/Middleware/WebAspNetCore_2.0)

```csharp

public void Configure(IApplicationBuilder app, IHostingEnvironment env, ILoggerFactory loggerFactory, IApplicationLifetime appLifetime)
{
    app.UsePrometheusServer();
}

```

```csharp

public void Configure(IApplicationBuilder app, IHostingEnvironment env, ILoggerFactory loggerFactory, IApplicationLifetime appLifetime)
{
    app.UsePrometheusServer(q =>
    {
        q.MapPath = "/metrics1";
    });
}

```


