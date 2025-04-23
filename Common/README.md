# Gestion dynamique des versions TIA Portal � AgroFlow

## Pr�sentation

La gestion des versions TIA Portal dans AgroFlow est une **fonctionnalit� centrale et tr�s pratique** permettant de s�lectionner dynamiquement la version TIA Portal � utiliser, sans devoir installer ou lancer une application diff�rente pour chaque version.  
**Avant cette innovation, il existait une application distincte pour chaque version de TIA Portal** (V16, V17, etc.), ce qui compliquait la maintenance, la distribution et l�utilisation sur le terrain.  
Gr�ce � la gestion dynamique, un seul outil AgroFlow suffit d�sormais pour piloter l�ensemble des versions support�es de TIA Portal Openness?: un gain de temps, de praticit� et de robustesse pour tous les automaticiens et chefs de projet.

## Fonctionnement global

- **S�lection de la version TIA Portal**?: � l�ouverture ou depuis l�interface principale, l�utilisateur choisit la version install�e sur son poste.
- **V�rification automatique** de la disponibilit� des DLL Openness n�cessaires (Siemens.Engineering.dll, Siemens.Engineering.Hmi.dll...).
- **Chargement dynamique** des assemblies Openness via le gestionnaire d�assemblies .NET, sans red�marrage ni manipulation complexe.
- **Gestion des changements de version**?: lors d�un changement, les modules en cours sont d�charg�s proprement, �vitant tout conflit de version ou plantage.
- **Interop�rabilit� transparente**?: les outils, scripts et modules internes utilisent toujours la bonne version TIA Portal, adapt�e au projet en cours.

## Classes et modules principaux

- **TIAVersionManager**?:  
  Permet de d�finir, m�moriser, et surveiller la version courante de TIA Portal utilis�e.  
  Fournit �galement des m�thodes pour v�rifier la pr�sence des DLL n�cessaires, et signale tout changement de version � l�application.

- **TIAAssemblyLoader**?:  
  S�occupe du chargement dynamique des DLL Openness appropri�es et de la gestion des contr�les utilisateurs (.NET/WinForms) d�pendants de la version courante.
  G�re �galement le d�chargement propre des modules lors d�un changement de version.

## Avantages pour l�utilisateur

- **Un seul outil pour toutes les versions**?: fini les applications multiples, tout est centralis�.
- **Changement de version ultra simple**?: un simple choix dans l�interface, sans red�marrage complexe.
- **S�curit� et robustesse**?: impossible de charger une mauvaise DLL ou de provoquer des conflits de version.
- **Gain de temps majeur** pour la maintenance, la formation et le support?: un seul logiciel � installer et � ma�triser.

## Pr�requis

- TIA Portal install� (V17 minimum)
- Les DLL Openness Siemens correspondantes pr�sentes sur le poste
- Application AgroFlow (version r�cente)

## Pour aller plus loin

La documentation XML d�taill�e (dans le code source) d�crit chaque m�thode, propri�t� et �v�nement des modules `TIAVersionManager` et `TIAAssemblyLoader`.

---

*Cette gestion dynamique des versions TIA Portal est un atout majeur d�AgroFlow, pens�e pour la productivit� et la simplicit� d�usage sur tous les sites industriels Agro Mousquetaires.*