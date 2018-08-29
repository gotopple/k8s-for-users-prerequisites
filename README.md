# Kubernetes for Users Prerequisites

Good morning trainees,

In the week before our Kubernetes training you'll need to take a few simple steps to prepare. This course is a two-day offsite at Galvanize in Phoenix. You will need to prepare and bring your laptops. All work will be done locally.

##### 1. Install "Docker for Desktop" 18.06 on the laptop that you'll be bringing to class: https://www.docker.com/products/docker-desktop

This must be on your host operating system (Windows or MacOS) not on a virtual machine. Docker for Desktop will leverage your OS virutalization technology. For Windows users this means it requires that your system has HyperV (Windows 10 Pro). This course will not leverage proprietary Intel data or IP so if it is easier to use a personal laptop then you are welcome to do so.

##### 2. Enable Kubernetes

Kubernetes ships with Docker for Desktop on both Windows and Mac. Open the Docker for Desktop application window, navigate to the Kubernetes tab, and click the appropriate checkbox:

<p align="center">
<img alt="Enable Kubernetes in Docker for Desktop on Mac" src="https://github.com/gotopple/k8s-for-users-prerequisites/raw/master/images/enable-kube-d4m.png">
<img alt="Enable Kubernetes in Docker for Desktop on Windows" src="https://github.com/gotopple/k8s-for-users-prerequisites/raw/master/images/enable-kube-d4w.png">
</p>

##### 3. Verify installation and version

    kubectl version -o yaml

##### 4. Pre-pull several Docker images

You're going to be using several official sample programs. Download those Docker images now in order to speed things up during class. Run the following commands on your laptop:

    docker pull redis:alpine
    docker pull alpine:3.8
    docker pull dockersamples/visualizer:stable
    docker pull dockersamples/examplevotingapp_worker:latest
    docker pull dockersamples/examplevotingapp_result:before
    docker pull dockersamples/examplevotingapp_vote:before
    docker pull dockersamples/examplevotingapp_result:after
    docker pull dockersamples/examplevotingapp_vote:after
    docker pull postgres:9.4
    docker pull k8s.gcr.io/kubernetes-dashboard-amd64:v1.10.0

##### 5. Email me

When you've done these please respond to the email and let me know that you're ready to go.

## Class rules:

1. Please no work email during class
2. Lids down during lecture
3.

## Copyright

&copy; Topple 2018
