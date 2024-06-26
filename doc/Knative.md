- Serverless 的主要特征：无需管理基础设施，按量计费，事件驱动，自动化部署
- 开发者只关心业务逻辑，不关心平台本身
- Knative 是谷歌发起的开源 Serverless解决方案
- 结合了云原生应用开发的三个领域：服务构建部署的自动化，服务编排的弹性化，事件驱动基础设施的标准化
- 以K8S扩展的形式提供了一整套中间件，可以运行任何无状态容器应用
- 容器是将操作系统层虚拟化，虚拟机是将硬件虚拟化
- 环境中通常通过部署sidecar来提供对Istio的支持
- minikube start + knative quick start 最后还是使用了这样的安装方式
- *knative serving 组件* 为k8s上的服务提供了自动缩扩容的功能，通过autoscaler的功能实现，监控pod的流量，并根据算法来控制pod的数量
- *knative eventing 组件* （作用待写）
- 可观察性组件：普罗米修斯，grafana，EFK，Jaeger
- 可以通过istio operator去安装istio
- k get ksvc
- cluster local gateway
- Learning guide：https://knative.dev/docs/getting-started/first-autoscale/#list-your-knative-service