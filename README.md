# k8s-stack

### kube-proxy

kube-proxy运行在每个node上，监听 service 和 endpoint 变化，并通过 iptables等来为服务配置负载均衡（仅支持TCP和UDP，不支持HTTP 流量需要 ingress controller 组件实现）。

kube-proxy 支持以下几种实现：
+ iptables
+ ipvs
