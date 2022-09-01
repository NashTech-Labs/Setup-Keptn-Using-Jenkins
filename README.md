# Setup-Keptn-Using-Jenkins
Setup keptn cli, helm and k3d using Jenkins pipeline.

## How to begin the Installation?
Just execute the main.sh file using this command.
```
bash main.sh
```

The above command will do the following tasks:-
```mermaid
flowchart TD
    A[Main.sh executed] --> B{Are pre-requisites installed?};
    B -- Yes --> C[Begin Keptn Installation!];
    B -- No --> D[print Install the pre-requisites!];
    C ----> E[Enjoy Keptn has been installed!];
    D ----> A[Main.sh executed];
```