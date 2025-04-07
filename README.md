View this project on [CADLAB.io](https://cadlab.io/project/28977). 

DIJOUS_JordiMax_Llums

## Autors
- Max Pérez (@maxperez58)
- Jordi Godàs (@Jordi_Godas)

## Versió - v1.0 ## Curs - Assignatura de Disseny de PCBs amb KiCad - [Curs 2024-2025]

## Objectiu Descripció breu de l'objectiu del projecte.

L'objectiu d'aquest projecte és la realització d'un sistema de control per els diferents tipus de llums d'un vehícle automòvil. A més a més, s'ha incorporat un motor per al control de l'escombreta neteja-fars.

## Requisits i especificacions
- Llums curtes.
- Llums d'encreuament.
- Llums de circulacio dïurna.
- Intermitents.
- Motor escombreta neteja-fars.
- Sensor digital de llum, per activar les llums.

## Diagrama de blocs (Afegiu una imatge del diagrama de blocs)
![image](Diagrama%20Bloques/diagramadeblocs.png)

_Figura 1.1: Diagrama de Blocs del nostre projecte_



## Taula de components
| Descripció | Manufacturer Number | Package | Datasheet | Proveïdor | Unitats |
|------------|--------------------|---------|----------|----------|---------|
| LDO-5V | ADM7172ACPZ-5.0-R7 |SMD| [ADM7172ACPZ-5.0-R7](https://www.mouser.es/datasheet/2/609/ADM7172-3121160.pdf)| Mouser | 1 |
| LDO-3.3V | ADP7112ACBZ-3.3-R7 |SMD| [ADP7112ACBZ-3.3-R7 ](https://www.mouser.es/datasheet/2/609/ADP7112-3121706.pdf)| Mouser | 1 |
| Sensor de llum | BH1750FVI-TR |SMD| [BH1750FVI-TR](https://www.mouser.com/catalog/specsheets/Rohm_11162017_ROHMS34826-1.pdf)| Mouser | 1 |
| Relé | G5LE-1 DC12 |TO-220| [G5LE-1 DC12](https://www.mouser.es/datasheet/2/307/en_g5le-3447037.pdf)| Mouser | 2 |
| Buck converter | LM2596T-ADJ |SMD| [LM2596T-ADJ](https://www.ti.com/lit/ds/symlink/lm2596.pdf)| Texas Instruments | 1 |
| Transciever| MCP2551-I-SN |SMD| [MCP2551-I-SN](https://ww1.microchip.com/downloads/en/devicedoc/21667d.pdf) | Texas Instruments | 1 |
| Microcontrolador | PIC18F2580-I/SO |SMD| [PIC18F2580-I/SO](https://www.mouser.es/datasheet/2/268/39637d-3443674.pdf) | Mouser | 1 |
| Transistor NMOS | Si7336ADP |SMD| [Si7336ADP](https://www.vishay.com/docs/73152/si7336adp.pdf)| Mouser | 4 |
| Transistor BJT | ZXTN19020DFFTA |SMD| [ZXTN19020DFFTA](https://www.diodes.com/assets/Datasheets/ZXTN19020DFF.pdf) | Mouser | 5 |
| Traductor (3.3V-5V) | PCA9306D |SMD|[PCA9306D](https://www.ti.com/lit/ds/symlink/pca9306.pdf?ts=1743021004009&ref_url=https%253A%252F%252Fwww.ti.com%252Fproduct%252FPCA9306) | Mouser | 1 |
| Sensor hall | TMAG5124G1CEDBZRQ1 |SMD| [TMAG5124G1CEDBZRQ1](https://www.ti.com/lit/ds/symlink/tmag5124-q1.pdf?ts=1743694512003&ref_url=https%253A%252F%252Fwww.mouser.es%252F) | Mouser | 1 |
| OPAMP's | LT6202CS5 |SMD| [LT6202CS5](https://www.mouser.es/datasheet/2/609/620234fd-2955338.pdf) | Mouser | 1 |
| Voltage Regulator | TLV1117-33 |SMD| [TLV1117-33](http://www.ti.com/lit/ds/symlink/tlv1117.pdf) | Mouser | 1 |
| Cristall | XT9M20ANA8M |SMD| [XT9M20ANA8M](https://datasheet.octopart.com/XT9M20ANA8M-Vishay-datasheet-41303490.pdf) | Mouser | 1 |
| Inductance | Ms 42 / 47 µH |SMD| [Ms 42 / 47 µH](https://neosid.de/import-data/product-pdf/neoFestind_Ms42.pdf) | Mouser | 1 |
| Diode | 1N4002 |THT| [1N4002](https://diotec.com/request/datasheet/1n4001.pdf) | Mouser | 1 |
| Diode | 1N5817 |THT| [1N5817](http://www.vishay.com/docs/88525/1n5817.pdf) | Mouser | 4 |
| LED | APTR3216PGW |SMD| [APTR3216PGW](https://www.mouser.es/datasheet/2/216/kingbright_kngbd00006-5-1736195.pdf) | Mouser | 2 |
| Zener diode | BZX84C39 |SMD| [BZX84C39](https://diotec.com/request/datasheet/bzx84c2v4.pdf) | Mouser | 1 |
| Diode | 1N4148 |THT| [1N4148](https://assets.nexperia.com/documents/data-sheet/1N4148_1N4448.pdf) | Mouser | 1 |
| Diode Schottky | SS3P5HM3/84A |SMD| [SS3P5HM3/84A](https://www.vishay.com/docs/88944/ss3p3.pdf) | Mouser | 1 |

## Funcionalitats de les diverses seccions del nostre circuit
- [ ] Secció 1: secció de Power que converteix els 12 volts de VBAT a 5 volts per +Vcc i els 3.3 volts pel sensor.
- [ ] Secció 2: resistències pull-down a l'input per evitar una entrada descontrolada en cas de no connexió.
- [ ] Secció 3: secció del sensor amb traductor de nivell per garantir la bona comunicació entre sensor i microcontrolador.
- [ ] Secció 4: Etapa d'entrada del sensor Hall, el qual està destinat a comptar les voltes del motor.
- [ ] Secció 5: Etapa de comunicacions basada en un transciever el qual serveix per connectar el micro a un bus CAN.
- [ ] Secció 6: Etapa digital, formada pel micro i els seus I/0 + ICSP + Clock
- [ ] Secció 7: Pont-H + resistència Shunt, que controlen el sentit de gir del motor i detecten possibles pics de tensió
- [ ] Secció 8: etapa de selecció, on segons el corrent de base dels transistors i el voltatge aplicat al relé, s'escull un tipus d'iluminació o un altre.
- [ ] Secció 9: etapa reservada pels outputs i el connector DB-9 del bus CAN

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
| 2025-03-27 | Jordi Godàs |  `main` | Actualizar presentacion |
| 2025-03-27 | Jordi Godàs |  `main` | Actualizar el diagrama de bloques y el esquematico con lo dicho en clase por el profesor |
| 2025-03-29 | Max Pérez |  `main` |simulación Puente H v2|
| 2025-03-31 | Max Pérez |  `main` |Placement algunos componentes, separación planos masa y potencia. Routing Transciever, puente H y algun Input Output|
| 2025-04-02 | Jordi Godàs |  `main` | Acabar el layout de la pcb |
| 2025-04-02 | Jordi Godàs |  `main` | Actualizar presentacion |
| 2025-04-02 | Max Pérez |  `main` |GND de SMD + algun ruteo puntual. DRC sin errores|
| 2025-04-03 | Jordi Godàs |  `main` | Cambio del LDO-3.3V y placement en el esquematico |
| 2025-04-03 | Jordi Godàs |  `main` | Update readme |
| 2025-04-06 | Jordi Godàs |  `main` | Update pcb, bigger paths and better organitzation |
| 2025-04-06 | Jordi Godàs |  `main` | Update schemetatic, minor changes |
| 2025-04-07 | Jordi Godàs |  `main` | Finished layout, ERC passed |
| 2025-04-07 | Max Pérez |  `main` | Update readme |



