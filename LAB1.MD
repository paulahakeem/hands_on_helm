### add bitnami helm chart in controlplane 
```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
```
- screenshot from terminal ![Screenshot_20230212_105656](https://user-images.githubusercontent.com/116673091/218307911-db3862d3-3398-44f2-912b-18d3c4490f10.png)
---
### Deploy the Apache application on the cluster using the apache from the bitnami repository. Set the release Name to: amaze-surf
```bash
helm install amaze-surf myrepo/apache
```
- screenshot from terminal ![ddddddddddddddddd212_105744](https://user-images.githubusercontent.com/116673091/218308002-89388f78-3577-4ecf-8bd7-be5465aeef60.png)
---
### Uninstall the apache chart release  from the cluster 
```bash
helm install amaze-surf
```
- screenshot from terminal ![Screenshot_20230212_105843](https://user-images.githubusercontent.com/116673091/218308244-38c7a12e-8b9b-4e83-b555-b0c7ad15ec00.png)

---
### install specfic version of nginx 1.22.0
### then update it to specfic 1.23.1 
### then rollback
``` bash
helm search repo nginx --versions
helm install my-release myrepo/nginx --version 12.0.6
helm upgrade my-release myrepo/nginx --version 13.2.10
helm list
helm history my-realease
helm rollback my-release 1
```
- screenshots from terminal 
![Screenshot_20230212_110354](https://user-images.githubusercontent.com/116673091/218308450-80be34e6-77a2-4ade-a0cb-5e4ef8578152.png)
![Screenshot_20230212_110552](https://user-images.githubusercontent.com/116673091/218308455-09852428-bcc2-4c09-8a6a-1c63d72f1f77.png)
![Screenshot_20230212_110941](https://user-images.githubusercontent.com/116673091/218308456-59ee0073-5533-4b52-8daf-c95be731e81c.png)
![Screenshot_20230212_111306](https://user-images.githubusercontent.com/116673091/218308459-4149c0b9-b9c7-45ab-aa9b-c9981d55a209.png)
