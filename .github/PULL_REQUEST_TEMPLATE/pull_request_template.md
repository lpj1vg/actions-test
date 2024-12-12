name: '🗒️ Kafka Connector PR' 
description: 'Crea/Cambia la configuración de un Connector de Kafka'
title: '🗒️ Connector PR: '
body:
- type: checkboxes
  id: connector-checks
  attributes:
    label: Debes validar **todas** esta comprobaciones
    description: Hasta que no estén todas no se podrá hacer PR
    options:
      - label: ¿Se ha verificado la exitencia del Namespace/Eventhub?
        required: true
      - label: ¿Se ha verificado el número de particiones del Eventhub sea igual al topic de onprem?
        required: true
      - label: ¿Se ha verificado la existencia del usuario en Cyberark?
        required: true
  validations:
    required: true  
  
