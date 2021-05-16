---
title: "Getting started with Orleans"
date: "2021-05-16"
author:
  name: "Paramesh Gunasekaran"
aliases:
  - /talks/getting-started-with-orleans/
---

This article not only attempts to explain the complexities in developing distributed application using traditional approach but also provides Actor Model as an alternate approach, introducing a Microsoft implementation known as Orleans and backs with a working prototype using Orleans framework. The full source code of this working prototype is available in GitHub at [go.paramg.com/orleans/prototype](https://go.paramg.com/orleans/prototype "Building distributed high-scale computing applications using Orleans") with the presentation slides at [go.paramg.com/orleans/presentation](https://go.paramg.com/orleans/presentation "Building distributed high-scale computing applications using Orleans").

### Introduction

In today’s world, systems and applications are expected to serve with very high-throughput, respond in real-time, always available 24/7 without any downtime or reduced capacity, automatically scale up and down depending upon real-time customer volume. These attributes are no longer reserved for only high-end enterprise-level or research-oriented systems but also for every simple customer-facing day-to-day regular application. Indeed each one of these attributes pose an independent and complex problem landscape that has been under academic research for several years with multiple possible solutions depending on the use case.
High-throughput, real-time response, always-available and auto-scaling are the normal

Unfortunately, every application developer is forced to solve and implement solutions for these problems along with their actual business solutions. This results in the developer implementing these solutions in varying degrees of completeness and repeating it over for every application or business domain as there is no standardized way of solving these problems and reusing for developers. Orleans is an attempt from Microsoft to solve these problems using a well-known pattern called Actor-Model and abstract away the complexity of solving these core problems from developers and making it available for reuse for any application or business domains.

The full article text can be found in Medium at [go.paramg.com/orleans/article](https://go.paramg.com/orleans/article "Building distributed high-scale computing applications using Orleans").