# Contributor Covenant Code of Conduct

## STOP URGENCE :
```
service: veichi_ac.emergency_stop
```

## Vue OPÉRATEUR (commande) :
images/operator_view.png
```
type: entities
title: Variateur VEICHI – Commande
entities:
  - switch.marche_variateur
  - number.frequence
  - switch.sens_rotation
```

## Vue SUPERVISION :
images/supervision_view.png
```
type: entities
title: Supervision variateur
entities:
  - sensor.frequence_reelle
  - sensor.courant_moteur
  - sensor.puissance_moteur
  - sensor.temperature_variateur
  - binary_sensor.defaut_variateur
```

## Vue SÉCURITÉ :
images/safety_view.png
```
type: button
name: STOP URGENCE
icon: mdi:alert-octagon
tap_action:
  action: call-service
  service: veichi_ac.emergency_stop
```
