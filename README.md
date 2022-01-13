******GitOps Demo Repo - Shows how GitOps CD Pipelines Work******

Uses ArgoCD + ArgoCD ApplicationSet Controller - Shows how to hookup Git Directory Generator



Ensure ArgoCD is Installed:

**Follow ArgoCD Official Guide**  
https://argocd-applicationset.readthedocs.io/en/stable/Getting-Started/



****Installation Summary:****

1. **Create namespace**
   kubectl create namespace argocd
  
2. **Install ArgoCD & ArgoCD ApplicationSet Contoller**
   kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj-labs/applicationset/v0.3.0/manifests/install-with-argo-cd.yaml  

3. **Create ArgoCD Project** 
   kubectl apply -f argo-project.yaml

4. **Create ArgoCD Root Application** 
   kubectl apply -f argo-root-app.yaml
