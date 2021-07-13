# Deployment Guide

This guide will walk you through using pipelines to build the Spring Pet Clinic app via [Tanzu Build Service]()

# Prep work

In order for the deployment to work - you'll need to create the image on Tanzu build service and point it to a previous commit sha:

```
kp image create spring-petclinic --tag harbor-demo.ryanbaker.io/demo-tbs/spring-petclinic --git https://github.com/ryan-a-baker/spring-petclinic.git --git-revision 0e6479b2373ce5ea63a39f27fced18c3a6ec8917
```