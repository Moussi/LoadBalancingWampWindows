# LoadBalancingWampWindows

```xml
<Proxy balancer://pfs>
            BalancerMember http://localhost:8080/dashboards-web
            BalancerMember http://localhost:8088/dashboards-web
 </Proxy>
    ProxyPass /dashboard balancer://pfs
    ProxyPassReverse /dashboard balancer://pfs
```

