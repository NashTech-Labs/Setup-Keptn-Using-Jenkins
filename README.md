# Setup-Keptn-Using-Jenkins
Setup keptn cli, helm and k3d using Jenkins pipeline.

## How to begin the Installation?
Just execute the main.sh file using this command using Jenkins pipeline on the host you want to deploy it on.
Rest script will handle everything :)
```
bash main.sh
```

The above command will do the following tasks:-
```mermaid
flowchart TD
    A[Main.sh executed] --> B{Are pre-requisites installed?};
    B -- Yes --> C[Begin Keptn Installation!];
    B -- No --> D[Install the pre-requisites!];
    C ----> E[Install K3d!];
    D ----> A[Main.sh executed];
    E ----> F[Download and Install Keptn CLI!];
    F ----> G[Install control-plane and execution-plane for continuous delivery use case using Helm!];
    G ----> I[Configure ingress and authenticate Keptn CLI!];
    I ----> J[Enjoy Keptn has been installed!];
```
## Congratulations you have intalled Keptn !!
### You can now access the Web UI at http://127.0.0.1.nip.io:8082/bridge.