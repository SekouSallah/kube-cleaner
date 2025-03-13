# kube-cleaner 🧹 | Nettoyeur intelligent pour Kubernetes

kube-cleaner est un outil CLI écrit en Go qui identifie et supprime les ressources obsolètes dans votre cluster Kubernetes.  
Il permet de nettoyer automatiquement les Pods en échec, les Jobs terminés et les PersistentVolumeClaims inutilisés.  

## Fonctionnalités principales :
✅ Suppression des Pods en échec (`CrashLoopBackOff`, `Evicted`).  
✅ Nettoyage des Jobs terminés (`Completed`, `Failed`).  
✅ Suppression des PersistentVolumeClaims (PVC) orphelins.  
✅ Mode **dry-run** pour tester sans supprimer.  
✅ Compatible avec tous les clusters Kubernetes.  

## Installation & Utilisation :
```bash
kube-cleaner clean pods
kube-cleaner clean jobs --namespace=dev
kube-cleaner clean pvc --dry-run
