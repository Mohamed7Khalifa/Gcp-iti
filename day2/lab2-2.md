# GCP
## Lab 1.2
--- 
### 1. Create a VM with public ip then:
– In two different ways, SSH into this VM.
```bash
gcloud compute ssh instance-public-1 --project=khalifa-iti-20233 --tunnel-through-iap
```

![image info](Screenshot/lab2-2-q1.png)

– Enforce SSH into this VM to be IAP protected.
![image info](Screenshot/lab2-2-q2.png)

![image info](Screenshot/lab2-2-q2-2.png)

### 2. Create a VM without public ip then:
– SSH into this vm.
```bash
gcloud compute ssh instance-private-1 --project=khalifa-iti-20233 --tunnel-through-iap
```
– update system packages (is it possible?)
    **answer is no**
---
### 3. Create a VM with public ip then:
– SSH into this vm
– Update system packages.
```bash
sudo apt update
```
– Setup Nginx Web Server and test your setup.
```bash
sudo apt install nginx
```
– Create a custom image from this VM named “custom-img-nginx”.
![image info](Screenshot/lab2-2-q3.png)
### 4. Create MIG (min 3 and max 5) of a template using the custom image “custom-img-nginx”.
![image info](Screenshot/lab2-2-q4.png)
![image info](Screenshot/lab2-2-q5.png)