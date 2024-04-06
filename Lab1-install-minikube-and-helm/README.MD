## Lab Exercise: Installing Minikube and Helm on Ubuntu

### Objective:
Install Minikube and Helm on an Ubuntu system.

### Steps:

1. **Install Required Dependencies**:
   Open a terminal and run the following commands to install the required dependencies:
   ```bash
   sudo apt update
   sudo apt install -y curl wget apt-transport-https

2. **Download and Install Minikube**:

Run the following commands to download and install Minikube:
```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```
3. **Start Minikube**:

Start Minikube by running the following command:
```
minikube start
```
4. **Verify Installation**:

Once Minikube has started successfully, you can verify the installation by checking the status:
```
minikube status
```
### Additional Notes:
- Minikube runs a single-node Kubernetes cluster locally, making it easy to get started with Kubernetes development and testing.
- Helm is a package manager for Kubernetes that helps you manage Kubernetes applications. It is used for installing and managing Kubernetes applications.
- For more detailed information on Minikube and Helm, refer to the [official documentation](https://minikube.sigs.k8s.io/docs/) and [Helm documentation](https://helm.sh/docs/).

### Clean up:
To remove Minikube and Helm from your system, delete the Minikube binary and Helm binary:
```
sudo rm /usr/local/bin/minikube
sudo rm /usr/local/bin/helm
```

