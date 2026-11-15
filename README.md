# odoo19-modules

Addons personnalisés compatibles avec **Odoo 19**. Ce dépôt est la source des modules installables ciblant Odoo 19; l’index commun et la classification des autres dépôts se trouvent dans [odoo-modules](https://github.com/christiannoubisssi/odoo-modules).

## Structure

```text
oodo19-modules/
├── README.md
└── addons/
    ├── README.md
    └── module_template/
        ├── README.md
        ├── __init__.py
        ├── __manifest__.py
        ├── models/__init__.py
        ├── security/README.md
        ├── tests/__init__.py
        └── views/README.md
```

## Installation

Cloner le dépôt puis ajouter le chemin absolu vers `addons/` à l’option `addons_path` de la configuration Odoo 19. Redémarrer Odoo, mettre à jour la liste des applications et installer le module voulu.

```bash
git clone https://github.com/christiannoubisssi/odoo19-modules.git
```

## Ajouter un module

Copier `addons/module_template/` sous un nom technique unique, compléter le manifeste et le README, puis tester le module sur Odoo 19. Le champ `version` du manifeste doit commencer par `19.0.`. Ne pas ajouter ici de code destiné uniquement à Odoo 18.

Chaque addon doit documenter ses dépendances, sa configuration, son installation et les tests effectués. Ne déclarer comme compatible que le code effectivement vérifié sur Odoo 19.
