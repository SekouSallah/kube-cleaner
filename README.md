```markdown
# kube-cleaner 🧹 | Nettoyeur intelligent pour Kubernetes

🚀 **kube-cleaner** est un outil CLI écrit en Go qui aide à identifier et supprimer les ressources obsolètes dans votre cluster Kubernetes.  
Il nettoie automatiquement les Pods en échec, les Jobs terminés et les PersistentVolumeClaims (PVC) inutilisés.

## 📌 **Fonctionnalités principales**
- ✅ Suppression des Pods en échec (`CrashLoopBackOff`, `Evicted`).
- ✅ Nettoyage des Jobs terminés et échoués (`Completed`, `Failed`).
- ✅ Suppression des PersistentVolumeClaims (PVC) orphelins.
- ✅ **Mode dry-run** pour tester sans supprimer.
- ✅ Compatible avec tous les clusters Kubernetes.

## 🔧 **Installation**

### Installer via Go
```bash
go install github.com/SekouSallah/kube-cleaner@latest
```

### Installer depuis un binaire (Linux/macOS)
```bash
curl -L -o kube-cleaner https://github.com/SekouSallah/kube-cleaner/releases/latest/download/kube-cleaner-linux-amd64
chmod +x kube-cleaner
sudo mv kube-cleaner /usr/local/bin/
```

### Installer via Homebrew (Optionnel)
```bash
brew install SekouSallah/tap/kube-cleaner
```

## 🚀 **Utilisation**
```bash
kube-cleaner clean pods
kube-cleaner clean jobs --namespace=dev
kube-cleaner clean pvc --dry-run
```

## 🤝 **Contribuer**
Envie de contribuer ?  
Nous accueillons les contributions de la communauté ! Si vous êtes intéressé(e), n'hésitez pas à ouvrir une issue ou à soumettre une pull request.

### Étapes pour contribuer :
1. Fork ce dépôt.
2. Clonez votre fork :  
   `git clone https://github.com/votre-nom-d-utilisateur/kube-cleaner.git`
3. Créez une nouvelle branche :  
   `git checkout -b branche-nouvelle-fonctionnalité`
4. Apportez vos modifications et validez-les :  
   `git commit -am 'Ajout de nouvelle fonctionnalité'`
5. Poussez sur la branche :  
   `git push origin branche-nouvelle-fonctionnalité`
6. Ouvrez une pull request.

## 📝 **Licence**
Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

📢 **Envie de contribuer ?**  
Si vous êtes un(e) ingénieur(e) DevOps intéressé(e) par l'amélioration de kube-cleaner, ouvrez une issue ou une PR ! 🚀


---

# kube-cleaner 🧹 | Smart Kubernetes Cleaner

🚀 **kube-cleaner** is a CLI tool written in Go that helps identify and remove obsolete resources from your Kubernetes cluster.  
It automatically cleans up failed Pods, completed Jobs, and unused PersistentVolumeClaims (PVCs).

## 📌 **Key Features**
- ✅ Deletes failed Pods (`CrashLoopBackOff`, `Evicted`).
- ✅ Cleans up completed and failed Jobs (`Completed`, `Failed`).
- ✅ Removes orphaned PersistentVolumeClaims (PVCs).
- ✅ **Dry-run mode** to test without deleting.
- ✅ Compatible with all Kubernetes clusters.

## 🔧 **Installation**

### Install via Go
```bash
go install github.com/SekouSallah/kube-cleaner@latest
```

### Install from Binary (Linux/macOS)
```bash
curl -L -o kube-cleaner https://github.com/SekouSallah/kube-cleaner/releases/latest/download/kube-cleaner-linux-amd64
chmod +x kube-cleaner
sudo mv kube-cleaner /usr/local/bin/
```

### Install via Homebrew (Optional)
```bash
brew install SekouSallah/tap/kube-cleaner
```

## 🚀 **Usage**
```bash
kube-cleaner clean pods
kube-cleaner clean jobs --namespace=dev
kube-cleaner clean pvc --dry-run
```

## 🤝 **Contributing**
Want to contribute?  
We welcome contributions from the community! If you're interested, feel free to open an issue or submit a pull request.

### Steps to contribute:
1. Fork this repository.
2. Clone your fork:  
   `git clone https://github.com/your-username/kube-cleaner.git`
3. Create a new branch:  
   `git checkout -b feature-branch`
4. Make your changes and commit them:  
   `git commit -am 'Add new feature'`
5. Push to the branch:  
   `git push origin feature-branch`
6. Open a pull request.

## 📝 **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

📢 **Want to contribute?**  
If you're a DevOps engineer interested in improving kube-cleaner, open an issue or PR! 🚀
```
