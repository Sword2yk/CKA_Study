# CKA! Here are some tips and tricks

## Study tips
- Certified Kubernetes Administrator (CKA) with Practice Tests by Mumshad Mannambeth.
- CKA-StudyGuide by David-VTUK: [LabGuide](https://github.com/David-VTUK/CKA-StudyGuide/tree/master/LabGuide).
- Killer.sh (You get 2 free sessions of killer.sh with your exam voucher. The sessions last 36 hours each and the questions are MUCH harder than the real CKA exam. Killer.sh was actually useless in terms of the questions they asked BUT the environment/ layout of the terminal is very similar to the real exam so it helped me become comfortable with how the real exam would look.)

## WHAT TO STUDY:
- Create roles, services, and role bindings
- Unschedule a node and reschedule the pods
- Backup and restore ETCD
- Upgrade a cluster to a specific version
- NETWORK POLICY
- Scale deployments
- NodeSchedulers
- Pod logs
- Pod resource usage
- Persistent Volumes
- Assigning PVC to pods
- Sidecar containers
- Ingress
- Exposing deployments/ pods
- Troubleshooting nodes, pods, or networks (practice all)

## TIPS FOR THE EXAM
As soon as you enter the terminal run these commands
- alias k=kubectl Lets you type "k" in place of "kubectl"
export do="--dry-run=client -o yaml" This will let you create yaml files when you use the "kubectl run" command [ex: kubectl run nginx --image=nginx $do > nginx.yaml]. Then you can vim into the yaml you created. NEVER create a yaml file from scratch. It takes away too much valuable time. You can copy and paste almost any yaml configuration you will need from Kubernetes.io
- sudo -i Gives you root privileges. Run this immediately because the user they give you on the exam doesn't seem to have permission to do anything...
- USE THE RIGHT CONTEXT FOR EACH QUESTION. You will be instructed to use a specific context for each question. They give you the command to switch to the right context so all you have to do is copy and paste it into the terminal before you do anything. I cannot stress how important this step is. If you forget this step and use the wrong context you will most likely get the question wrong.
- Be VERY familiar with the kubectl cheat sheet and the reference docs. There are a lot of commands on both that will help you out tremendously if you know where to look.

## Links
[kubernetes Home](https://kubernetes.io/docs/home/)

[kubectl-commands](https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands)

[cheatsheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)

[Persistent-volumes](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistent-volumes)

[Network Policies](https://kubernetes.io/docs/concepts/services-networking/network-policies/)

[Backing-up-an-etcd-Cluster](https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd/#backing-up-an-etcd-cluster)
