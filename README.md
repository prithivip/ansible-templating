# ansible-templating

Steps to template a playbook. Same is applicable for complex tasks and roles.

1) Create jinja2 template file
2) Create manifests file
3) Define variables in a separate file
4) Define inventory files

ansible-playbook manifests/kubernetes-manifest.yaml -i /root/ansible/inventory/kube_inventory

git init
git add *
git commit -m "Template commit"
git branch -M main
git remote add origin git@github.com:prithivip/ansible-templating.git
git push -u origin main

Once deployment.yaml gets generated and pushed successfully to github, ArgoCD will get triggered to pull deployment.yaml files and deploy to kubernetes cluster
