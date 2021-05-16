---
title: "Istio Service Mesh for Kubernetes"
date: "2018-09-03"
author:
  name: "Paramesh Gunasekaran"
aliases:
  - /talks/istio-service-mesh-for-kubernetes/
---

### Introduction

About few months ago, while I was working on designing infrastructure platform and developing ASP.NET Core based microservices application, I was introduced to the world of service mesh and Istio by a coworker. Since then, I was intrigued by service mesh as an architectural concept and fascinated how Istio enables developers to roll out large, complex, enterprise-scale microservices applications and to manage the challenges of microservices. This article will detail out my progress in learning and deploying Istio on Kubernetes using Azure Kubernetes Cluster (AKS), a managed Kubernetes service provided by Microsoft. I hope this will provide anyone who is interested in developing and managing the complexities of microservices to consider service mesh/Istio as a good starting point.

In order to demonstrate the use of Istio service mesh on Kubernetes, we would require an application modeled in a microservices way. For this reason, I have developed a prototype using C# and ASP.NET Core containing few REST services, few externally accessible and few accessible internal only (downstream services). This prototype might be oversimplified ecommerce application allowing users to browse products and order them with ridiculously simple address and payment validation. But, the objective here is not this application, but to demonstrate few important features of Istio using same. The full source code of the working prototype is avaialble at GitHub at [go.paramg.com/istio/prototype](https://go.paramg.com/istio/prototype "Implementing Service Mesh using Istio on Kubernetes") and full text of the article in Medium at [go.paramg.com/istio/article](https://go.paramg.com/istio/article "Implementing Service Mesh using Istio on Kubernetes").