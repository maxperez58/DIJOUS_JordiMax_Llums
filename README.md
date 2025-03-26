View this project on [CADLAB.io](https://cadlab.io/project/28977). 

DIJOUS_JordiMax_Llums

## Autors
- Max Pérez (@maxperez58)
- Jordi Godàs (@Jordi_Godas)

## Versió - v1.0 ## Curs - Assignatura de Disseny de PCBs amb KiCad - [Curs 2024-2025]

## Objectiu Descripció breu de l'objectiu del projecte.

## Requisits i especificacions
- Llums curtes.
- Llums d'encreuament.
- Llums de circulacio dïurna.
- Intermitents.
- Motor escombreta neteja-fars.
- Sensor digital de llum, per activar les llums.

## Diagrama de blocs (Afegiu una imatge del diagrama de blocs)

## Taula de components
| Descripció | Manufacturer Number | Package | Datasheet | Proveïdor | Unitats |
|------------|--------------------|---------|----------|----------|---------|
| Díode | 1N1418 |DO-35| https://diotec.com/request/datasheet/1n4148.pdf| Mouser | 1 |
| Buck converter | LM2596T |TO-220| (http://www.ti.com/lit/ds/symlink/lm2596.pdf)| Texas Instruments | 1 |
| LDO | LM2596T |SMD| (https://www.mouser.es/datasheet/2/609/ADM7172-3121160.pdf)| Mouser | 1 |
| LDO | ADP7112ACBZ |SMD| (https://www.mouser.es/datasheet/2/609/ADM7172-3121160.pdf)| Mouser | 1 |
| Microcontrolador | PIC18F2580 |SMD| https://docs.rs-online.com/eeae/0900766b813831c4.pdf| Mouser | 1 |
| Transciever | MCP2551 |SMD| https://www.mouser.es/datasheet/2/268/20001667G-3441642.pdf| Mouser | 1 |
| NMOS | Si7336ADP |SMD| https://www.vishay.com/docs/73152/si7336adp.pdf| Mouser | 4 |
| NPN | ZXTN19020DFFTA | https://www.diodes.com/assets/Datasheets/ZXTN19020DFF.pdf| Mouser | 4 |
| Relay |  | |  | 1 |





## Funcionalitats
- [ ] Funció 1
- [ ] Funció 2
- [ ] Funció 3

## Historial de canvis 
| Data | Autor | Branch | Descripció |
|------|------|--------|------------| 
| 2025-03-17 | Max Pérez | `main` | Creació del projecte |
| 2025-03-17 | Max Pérez | `main` | LDO y output select stage |
| 2025-03-18 | Max Pérez | `main` | Conexiones básicas micro|
| 2025-03-18 | Max Pérez | `main` |Bloque transceiver, safe input y Clock|
| 2025-03-18 | Max Pérez |  `main` |Mejora estética|
| 2025-03-19 | Jordi Godàs | `main`|Acabar el diagrama de blocs 1.0|
| 2025-03-19 | Jordi Godàs |  `main` |Acabar el power point de la presentació|
| 2025-03-21 | Max Pérez | `main` |Creación esquemático 1.0|
| 2025-03-21 | Max Pérez | `main` |Bloques Clock, Communication, Digital Esquemático 1.0|
| 2025-03-21 | Max Pérez |  `main` |Bloques Input, Sensor, Power Esquemático 1.0|
| 2025-03-22 | Max Pérez |  `main` |Mejora etapa Power cambiando DC/DC + LDO por Buck|
| 2025-03-21 | Max Pérez | `main` |Capacidades desacoplo, comentar esquemático y bloque output|
| 2025-03-24 | Max Pérez |  `main` |Simulación Power stage (1 buck y 2 LDO). Exitosa|
| 2025-03-25 | Max Pérez |  `main` |Simulación Power stage (1 buck y 2 LDO) v2 y simulación Puente H|
