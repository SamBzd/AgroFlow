# Interface Principale � AgroFlow

## Pr�sentation

L�**interface principale** d�AgroFlow est le point d�entr�e graphique de l�application, pens�e pour offrir une exp�rience fluide et efficace aux automaticiens et chefs de projet du groupe Agro Mousquetaires.  
Elle centralise l�acc�s aux fonctions critiques, facilite la gestion multi-utilisateur (avec distinction admin/utilisateur standard) et permet une navigation rapide entre les diff�rents modules m�tiers de l�outil.

## Fonctionnement global

- **Interface graphique Windows Forms** moderne et personnalis�e, adapt�e au standard Agro Mousquetaires.
- **Gestion de sessions utilisateur et administrateur** avec droits distincts et adaptation dynamique des fonctionnalit�s disponibles.
- **S�lection dynamique de la version TIA Portal**?: l�utilisateur choisit la version TIA install�e avec m�morisation du dernier choix.
- **Navigation modulaire** : chaque fonction (aide au diagnostic, r�ception de projet, etc.) s�ouvre sous forme de UserControl pour garantir rapidit� et clart�.
- **Gestion centralis�e des logs**?: toutes les actions importantes sont historis�es dans un module de log accessible � tout moment.
- **Menu principal r�tractable/�tirable** pour optimiser l�espace de travail ou acc�der � des fonctions avanc�es (admin, terminal, etc.).
- **Gestion avanc�e de la fen�tre**?: redimensionnement, maximisation, d�placement personnalis�, etc.

## Principales fonctionnalit�s accessibles depuis l�interface

- **Aide au diagnostic**?: g�n�ration automatis�e des variables BLKJump dans le FC d�aide au diagnostic (voir documentation fonction d�di�e).
- **R�ception de projet**?: int�gration facilit�e et v�rification de conformit� de nouveaux projets TIA Portal.
- **Fonctions administrateur**?: options et outils avanc�s pour la maintenance ou la configuration (visibles uniquement apr�s connexion admin).
- **Historique des actions/logs**?: affichage instantan� de toutes les op�rations r�alis�es via l�interface.

## Public vis�

- **Automaticiens**, chefs de projet, int�grateurs travaillant sur des projets TIA Portal Agro Mousquetaires.
- **Administrateurs**?: acc�s � des outils suppl�mentaires pour la maintenance et la configuration avanc�e.

## Pr�requis techniques

- Application **AgroFlow** install�e sur le poste de travail.
- Une ou plusieurs versions de **TIA Portal** (V17 minimum) install�es sur le poste.
- R�f�rences internes Agro Mousquetaires (biblioth�que LTU, standards de projet�).

## Parcours utilisateur type

1. **S�lection de la version TIA Portal** install�e (la s�lection est m�moris�e entre les sessions).
2. **Choix d�une fonction** selon le profil utilisateur (aide au diagnostic, r�ception de projet�).
3. **Connexion possible en mode admin** pour acc�der � des fonctionnalit�s suppl�mentaires.
4. **Utilisation des modules**?: chaque fonction s�ouvre dans l�interface principale, avec gestion des logs et navigation simplifi�e.
5. **Gestion ergonomique de la fen�tre** (maximisation, r�duction, d�placement, etc.).

## Extension et personnalisation

L�interface principale est con�ue pour �tre **�volutive**?:  
- De nouveaux modules (UserControls) peuvent �tre ajout�s facilement.
- Les droits et profils utilisateurs sont centralis�s pour une gestion simplifi�e.
- La personnalisation des couleurs, logos, et messages respecte la charte Agro Mousquetaires.

---

*Ce module d�interface graphique AgroFlow incarne la volont� du groupe Agro Mousquetaires de proposer des outils performants, ergonomiques et adapt�s aux besoins des �quipes d�automatisme industrielle.*