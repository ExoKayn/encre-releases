# Encre : installateurs

Encre est un éditeur de bureau pour écrire un livre : chapitres et scènes, versions gardées automatiquement.

Ce dépôt ne contient que les installateurs. Dernière version : onglet **Releases**, ou directement
https://github.com/ExoKayn/encre-releases/releases/latest

| Système | Fichier |
| --- | --- |
| Windows | `Encre-<version>-win-x64.exe` |
| macOS, puce Apple (M1 et suivantes) | `Encre-<version>-mac-arm64.zip` |
| macOS, processeur Intel | `Encre-<version>-mac-x64.zip` |
| Linux | `Encre-<version>-linux-x86_64.AppImage` |

Encre signale elle-même les nouvelles versions au démarrage. Chaque Release contient un fichier `SHA256SUMS` pour
vérifier le téléchargement (Linux : `sha256sum -c SHA256SUMS --ignore-missing`).

Les fichiers ne sont pas signés : au premier lancement, Windows et macOS avertissent. Windows : « Informations
complémentaires » puis « Exécuter quand même ». macOS : décompresser le `.zip`, glisser Encre dans Applications, puis
Réglages Système, Confidentialité et sécurité, « Ouvrir quand même » (si l'application est dite « endommagée » :
`xattr -cr /Applications/Encre.app` dans le Terminal). Linux : rendre l'AppImage exécutable puis l'ouvrir.
