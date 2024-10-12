---
title: Kubernetes를 통한 Prometheus,Grafana,Opensearch 아키텍쳐
date: YYYY-MM-DD HH:MM:SS +09:00
categories: [Kuberenetes, Prometheus, Grafana, Opensearch]
tags:
  [
    Kuberenetes,
    Prometheus,
    클라우드,
    Grafana,
    Opensearch
  ]
---

Samsung DS에서의 K8S 고도화 프로젝트를 진행 후 Local PC에서 직접 시스템을 구축해보았습니다.
목적은 Kubernetes로 Wordpress를 직접 서비스화시키는 것이었습니다. (현재는 접속이 되지 않습니다. / 전기비가 많이 들어서)

![k8s architecture](https://github.com/Sosimina/sosimina.github.io/blob/main/k8s_architecture.png)


1. Local PC를 가지고 Proxmox라는 Opensource를 통하여 논리적으로 3개의 PC로 나누었습니다.
2. Kube-spray와 Ansible을 통하여 동일한 쿠버네티스 환경을 각각 배포하였습니다.
3. Master, worker1, worker2에 각각 Control node / wordpress / Promethues & Grafana를 설치하였습니다.
4. 해당사항은 
![k8s 링크](./https://github.com/Sosimina/k8s_local/blob/main/K8s_Project/Kubernetes_local_sangwon.docx)

파일에서 자세히 볼 수 있습니다.

