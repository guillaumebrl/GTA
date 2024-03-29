### Rendement isentropique de groupe turbo-alternateur

### Généralités

La dérive dans le temps du rendement d'une turbine est caractéristique de l’état de ses internes (étanchéités des inter-étages et des périphéries des roues, état d'encrassement ou de déformation des ailettages mobiles et aubages fixes).

Le suivi de ce rendement permet de consolider un programme de maintenance, et participe, au même titre que les contrôles de suivi traditionnels (analyse vibratoire, analyse d’huile, analyse thermique...) à la maîtrise de l’état de la machine.

En s’appuyant sur les publications CEI 953-1 et 953-2, "Rules for steam turbine thermal acceptance tests", cette page propose un mode de mesure du rendement du GTA, et les modalités de mesure.

### Rendement GTA

Le rendement d'une installation est défini par le rapport de l'énergie sortante/énergie entrante.
La variation de ce rendement est significative d'une évolution de la différence entre l'énergie entrante et l'énergie sortante, soit les pertes.

Les GTA présents dans certaines usines (e.g. d'incinération) ne possèdent pas de mesure de couple sur les arbres de sortie turbine permettant un calcul direct de la puissance de sortie de la turbine. Le réducteur et l'alternateur seront donc inclus de fait dans la formule, la perte de rendement qui pourrait être mesurée ne permettra pas de distinguer l'origine de la perte entre la turbine et des autres éléments.

L'expression du rendement présentée dans la publication CEI 953-2 la mieux adaptée aux turbines industrielles simples est le rendement thermodynamique. Défini comme le rapport de la puissance de sortie à la puissance isentropique (produit du débit massique de vapeur et de la chute d'enthalpie isentropique entre la vapeur initiale et la pression d'échappement), la valeur numérique du rendement thermodynamique ne dépend pas des conditions initiales de vapeur et d'échappement, mais est l'indication de l'efficacité de la détente seulement (aux Rendements du réducteur et de l'alternateur près)

$$\eta_{th} = \frac{PE_b}{Q_a \times \Delta H_{S_{a:1}} + \Sigma_{i}^{n-1} (Q_a - \Sigma_{j}^{i-1} Q_j) \Delta H_{S_{i:i+1}} + (Q_a - \Sigma_{j}^{n} Q_j)\Delta H_{S_{n:e}}}$$

où :

- $PE_b$ : Puissance électrique en sortie de l'alternateur
- $Q$ : le débit de vapeur au point considéré
- $\Delta H_{S_{p:q}}$ : la chute d'enthalpie isentropique de la vapeur entre les points p et q.

Cette formule impose de connaître, en chaque point caractéristique de la turbine (admission, échappement, soutirages), la pression absolue, la température et le débit massique de la vapeur, ainsi que la puissance de sortie mesurée aux bornes de l'alternateur.

### Version
V1 - 10/02/2024

### Conception - réalisation

Vincent & Guillaume Bril

### Licence

[CC BY 4.0 DEED](http://creativecommons.org/licenses/by/4.0/legalcode)

Utilisation de la librairie [NativeDynamics](https://github.com/NativeDynamics/NeutriumJS.thermo.IAPWS97.git)
