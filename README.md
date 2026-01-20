🍃 Mint Architect - Ultimate Setup (Mint 22.3 Edition)

Mint Architect est un script de post-installation tout-en-un conçu spécifiquement pour Linux Mint 22.x (basé sur Ubuntu 24.04 Noble).

Il permet de configurer en quelques minutes une machine prête pour le Gaming, le Développement et l'Intelligence Artificielle Locale, tout en respectant la philosophie et les dépôts de Linux Mint.

🚀 Fonctionnalités

Le script propose une interface graphique en terminal (TUI) fluide, modulaire et sécurisée :

🛠️ Système & Maintenance

Mise à jour Intelligente : Met à jour le système et nettoie les paquets orphelins sans casser les dépôts Mint (pas de remplacement risqué du sources.list).

Fastfetch : Installation automatique via PPA (remplace le Neofetch obsolète).

🖥️ Pilotes GPU & Optimisation

NVIDIA : Installation via le PPA officiel graphics-drivers + ubuntu-drivers.

AMD : Pilotes Mesa/Vulkan optimisés + bibliothèques 32-bit.

INTEL (Support Étendu) :

Legacy (Gen 4 Haswell / T440p) : Pilotes spécifiques i965 pour garantir l'accélération matérielle sur les anciens ThinkPads.

Moderne (Gen 8+ / Iris Xe) : Pilotes intel-media-driver récents.

🔋 Optimisation Laptop (ThinkPad Ready)

Module dédié pour prolonger la durée de vie de la batterie et réduire la chauffe :

TLP : Gestion avancée de l'énergie.

Intel Microcode : Correctifs de sécurité CPU.

Thermald : Régulation thermique intelligente.

🤖 AI Stack (Privée & Locale)

Déploiement automatique via Docker d'une stack complète pour l'IA générative :

Ollama : Pour tourner les LLM (Llama3, Phi-3, Mistral) en local.

OpenWebUI : Interface type ChatGPT complète.

SearXNG : Moteur de recherche privé.

Accélération Flexible :

🟢 NVIDIA : Support CUDA via Nvidia Container Toolkit.

🔴 AMD : Support ROCm natif.

🔵 CPU ONLY : Mode spécial pour les PC sans GPU dédié (ex: ThinkPad T440p/Intel HD), permettant de faire tourner des petits modèles (Phi-3, TinyLlama).

🎮 Gaming

Steam, Gamemode (Feral), et Flatpak à jour.

ProtonPlus pour gérer les versions de Proton-GE.

📦 Logiciels & Web

Navigateurs : Chrome, Firefox (Mint), Zen Browser, Tor.

Outils : VS Code, OBS Studio (Flatpak), Discord, Telegram, VLC.

📥 Installation

Prérequis

Une installation fraîche de Linux Mint 22 (ou compatible Ubuntu 24.04).

Une connexion Internet.

Commande Rapide (One-Liner)

Ouvrez un terminal et collez cette commande :

```wget -O mint_architect.sh https://raw.githubusercontent.com/MrTHP/mint_architect/main/mint_architect.sh && chmod +x mint_architect.sh && sudo ./mint_architect.sh``` 


Installation Manuelle

Ouvrez un terminal et collez cette commande :

git clone https://github.com/MrTHP/mint_architect.git

cd mint_architect/

chmod +x mint_architect.sh

sudo ./mint_architect.sh

🖼️ Utilisation

L'interface utilise whiptail pour une navigation simple au clavier :

Haut / Bas : Naviguer dans les menus.

Espace : Cocher ou décocher des options ([*]).

Entrée : Valider.

Tab : Basculer entre "Ok" et "Annuler".

🛠️ Dépannage AI Stack

Si OpenWebUI ne démarre pas immédiatement sur une vieille machine (ex: T440p) :

Soyez patient, la première initialisation de la base de données peut prendre 2 à 5 minutes sur un CPU ancien.

Vérifiez les logs : sudo docker logs ai-stack-open-webui-1.

Accès :

OpenWebUI : http://localhost:3000

SearXNG : http://localhost:8080

⚠️ Avertissement

Ce script est optimisé pour Linux Mint 22.3 (Base Ubuntu Noble). Bien qu'il soit conçu pour être sûr (pas d'écrasement de fichiers système critiques), l'utilisation de scripts de post-installation se fait toujours à vos propres risques.

🤝 Contribution

Projet open-source. Les Pull Requests pour ajouter de nouveaux logiciels ou améliorer le support matériel sont les bienvenues !

Développé pour simplifier la vie des utilisateurs Linux Mint & ThinkPad.
