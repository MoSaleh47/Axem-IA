# AXEM IA × Bellanger Construction

Proposition commerciale interactive destinée au comité de direction de Bellanger Construction. La page permet de choisir les premiers usages de l’IA à tester en 2027, d’estimer le temps qu’ils pourraient libérer et de comparer deux budgets d’accompagnement.

## Ouvrir la proposition

Téléchargez `index.html` et ouvrez-le dans un navigateur. Le fichier contient l’application, le logo AXEM IA et le dessin de chantier. Les filtres, les curseurs et le comparatif fonctionnent aussi hors connexion.

## Utiliser la page en comité de direction

1. **Choisir les priorités.** Filtrez les huit besoins par vague. La première réunit la sécurité des données et trois pilotes métier : la pré-imputation des factures, les comptes rendus de chantier et les mémoires techniques.
2. **Tester les volumes.** Dans le simulateur, ajustez le nombre de factures par mois, le nombre de comptes rendus par semaine et le coût horaire chargé. Les résultats se mettent à jour à chaque mouvement de curseur.
3. **Comparer les offres.** L’option essentielle couvre deux pilotes pour **11 500 € HT sur 10 jours**. L’option recommandée ajoute le pilote Études et la feuille de route pour environ 50 licences, pour **15 500 € HT sur 14 jours**. Le calendrier prévoit un bilan des pilotes en avril 2027.

## Comprendre le calcul du ROI

| Hypothèse par défaut | Calcul annuel | Temps libéré |
| --- | --- | ---: |
| 2 500 factures par mois | 2 500 × 12 mois × 3 min | 1 500 h |
| 15 comptes rendus par semaine | 15 × 52 semaines × 45 min | 585 h |
| **Total** | | **2 085 h** |

À **42 €/h**, ces heures représentent **87 570 € de temps valorisé par an**, soit **1,30 équivalent temps plein** sur une base de 1 607 h/an. L’économie de trésorerie dépend de l’utilisation effective des heures libérées.

Le délai d’amortissement prend toujours pour référence **l’option recommandée à 15 500 € HT**, y compris lorsque l’option essentielle est affichée dans le comparatif. À plein régime, le calcul donne **15 500 ÷ (87 570 ÷ 12) ≈ 2,1 mois**. La projection exclut la montée en charge, les licences, la consommation des services, les gains commerciaux et toute aide éventuelle de Constructys.

## Déployer sur Vercel

1. Placez `index.html` à la racine du dépôt GitHub et importez le dépôt dans Vercel.
2. Dans **Framework Preset**, choisissez **Other**. Activez **Override** pour **Build Command** et laissez la commande vide.
3. Utilisez `.` comme **Output Directory**, puis lancez **Deploy**.

Le projet utilise HTML, CSS et JavaScript natif. En ligne, la page charge Tailwind CSS, les icônes Lucide et la police Inter. Les calculs s’exécutent dans le navigateur, sans clé API.

[Documentation Vercel sur les projets statiques](https://vercel.com/docs/builds/configure-a-build#skip-build-step)
