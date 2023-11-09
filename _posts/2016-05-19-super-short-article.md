---
layout: post
title: "🐳 Setting up a Kubernetes Cluster with MicroK8s on Raspberry Pi"
categories: Kubernetes, Docker, CKA - Path
---

🐳 Setting up a Kubernetes Cluster with MicroK8s on Raspberry Pi 🥧

Kubernetes is all the rage these days! 😎 Let's set up our own little K8s cluster using MicroK8s on a couple of Raspberry Pis. 👍 This will allow us to get hands-on experience with Kubernetes right from our home lab. 🧑‍🔬
Prerequisites ✔️

    2 or more Raspberry Pi 4 devices
    MicroSD card (32 GB recommended) for each device
    Ethernet cables to connect the Pis together
    A router/switch to connect the Pis to

Step 1 - Flash the OS 💾

Let's start by flashing the Raspberry Pi OS (32-bit) onto the MicroSD cards. I'm using the Lite version to save space.

bash

Copy code
wget https://downloads.raspberrypi.org/raspios_lite_armhf/images/raspios_lite_armhf-2022-04-07/2022-04-04-raspios-bullseye-armhf-lite.img.xz
unxz 2022-04-04-raspios-bullseye-armhf-lite.img.xz

# Flash to MicroSD card
sudo dd bs=4M if=2022-04-04-raspios-bullseye-armhf-lite.img of=/dev/mmcblk0 conv=fsync

Repeat for each of your Pis.
Step 2 - Configure the Pis 🪛

Insert the MicroSD cards into the Pis and power them on. Log into each device:

Copy code
ssh pi@<ip address> 
# Default password is raspberry

Run the raspi-config tool to set hostname, password, locale, etc.

Copy code
sudo raspi-config

For example:

    Set hostname: k8s-master, k8s-worker1, k8s-worker2
    Change password
    Set locale
    Enable SSH

Reboot after making changes.
Step 3 - Install MicroK8s 📥

Let's now install MicroK8s on each device:

Copy code
sudo snap install microk8s --classic

Turn on the DNS add-on:

Copy code
sudo microk8s enable dns

Designate one node as the master:

Copy code
sudo microk8s add-node

Join the workers to the master:

Copy code
sudo microk8s join <master-ip>:25000/TOKEN

Verify the nodes are ready:

Copy code
sudo microk8s kubectl get nodes

🎉 Our little Raspberry Pi cluster is ready! Let's deploy some containers on it!
Step 4 - Deploy a Sample App 🚀

To test out the cluster, let's deploy a simple web app:

Copy code
sudo microk8s kubectl create deployment nginx --image=nginx
sudo microk8s kubectl expose deployment nginx --port=80 --type=NodePort

We can access this app using any node's IP and the NodePort:

Copy code
http://<node-ip>:<nodePort>

And that's it! We now have a Kubernetes cluster running on Raspberry Pis. 😄 Some next steps could be to add persistent storage, TLS certificates, etc. But this covers the basics of setting up the cluster. Have fun exploring Kubernetes! 👋
