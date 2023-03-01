k8s
===

![](https://miro.medium.com/v2/resize:fit:480/format:webp/0*X-_IGBEAB88amxNO.png)


## 簡介

Kubernetes 簡稱 K8s，是因為K和S之間有8個英文字母，為了方便而縮寫簡稱為「K8s」。

Kubernetes（K8S）是一個可以幫助我們管理微服務（microservices）的系統，他可以自動化地部署及管理多台機器上的多個容器（Container）。簡單來說，他可以做到：

* 同時部署多個容器到多台機器上（Deployment）
* 服務的乘載量有變化時，可以對容器做自動擴展（Scaling）
* 管理多個容器的狀態，自動偵測並重啟故障的容器（Management）


---

## 架構

* 容器（Container）<br>
Container 採用作業系統虛擬化的形式，將應用程式所需的程式碼、函式庫、執行檔和組態檔等內容進行封裝，在 Container 中不需再安裝作業系統，即可在各種容器平台中執行應用程式。而 K8s 則是用來管理 Container 的系統，能協調多個 Container 的運作，使其彼此協調一致。

* 最小部署單位（Pod）<br>
Pod 也就是可以在 K8s 建立並管理的最小部署運算單位，在 K8s 上會運行多個不同種類型的應用程式，而一個 Pod 即相當於一個應用程式。在一個 Pod 內部可以運行單一或多個 Container，而同一個 Pod 裡面的 Containers，則會共享相同的網路資源。

* 節點（Node）<br>
Node 分成2種：Worker Node 及 Master Node。<br>
  1. Worker Node：是作為主要執行的運行節點，一個 Node 會對應到一台實體或虛擬機器，每個 Node 中都還有3個組件：kubelet、kube-Proxy、Container Runtime。
  2. Master Node：則可稱為 K8s 的指揮中心，負責管理所有的 Node，一個 Master Node 中有4個組件：kube-apiserver、etcd、kube-scheduler、kube-controller-manager。


## 環境準備文件

### 下載項目

1. [Google Cloud SDK](https://cloud.google.com/sdk/docs/install)
2. [Kubectl](https://kubernetes.io/docs/tasks/tools/)
3. [K9S](https://k9scli.io/topics/install/)
4. [fish (linux or mac)](https://fishshell.com/)
5. [kubectx](https://github.com/ahmetb/kubectx)
6. [lens](https://k8slens.dev/)


---


## 
 



[Tags]
==

###### tags:  `k8s` `Kubernetes`