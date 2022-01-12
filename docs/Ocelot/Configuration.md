# Configuration

```json
{
    //определяют URL-адрес, на который будет перенаправлен запрос
    "DownstreamPathTemplate": "/", 
    "DownstreamScheme": "http",
    "DownstreamHttpMethod": [ "Get" ],
    "DownstreamHttpVersion": "",
    //это коллекция, которая определяет хост и порт любых нижестоящих служб, которым вы хотите перенаправлять запросы.
    "DownstreamHostAndPorts": [
        {
            "Host": "localhost",
            "Port": 51876,
        }
    ],
    
    //это URL-адрес, который Ocelot будет использовать для определения того, какой DownstreamPathTemplate использовать для данного запроса.
    "UpstreamPathTemplate": "/",
    "UpstreamHttpMethod": [
        "Get"
    ],
    //Приведенный маршрут будет сопоставляться только в том случае, если значение заголовка хоста равно somedomain.com
    "UpstreamHost": "somedomain.com",
    
    "AddHeadersToRequest": {},
    "AddClaimsToRequest": {},
    "RouteClaimsRequirement": {},
    "AddQueriesToRequest": {},
    "RequestIdKey": "",
    "FileCacheOptions": {
        "TtlSeconds": 0,
        "Region": ""
    },
    "RouteIsCaseSensitive": false,
    "ServiceName": "",
    
    
    "QoSOptions": {
        "ExceptionsAllowedBeforeBreaking": 0,
        "DurationOfBreak": 0,
        "TimeoutValue": 0
    },
    "LoadBalancer": "",
    "RateLimitOptions": {
        "ClientWhitelist": [],
        "EnableRateLimiting": false,
        "Period": "",
        "PeriodTimespan": 0,
        "Limit": 0
    },
    "AuthenticationOptions": {
        "AuthenticationProviderKey": "",
        "AllowedScopes": []
    },
    "HttpHandlerOptions": {
        "AllowAutoRedirect": true,
        "UseCookieContainer": true,
        "UseTracing": true,
        "MaxConnectionsPerServer": 100
    },
    "DangerousAcceptAnyServerCertificateValidator": false
}
```