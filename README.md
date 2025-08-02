# 🧰 SmartBox-Control - Valise Domotique

## 📌 Description
Valise domotique autonome permettant le contrôle :
- ✅ **Manuel** via boutons physiques
- 💻 **Logiciel** via Loxone Config sur PC
- 📱 **Mobile** via application Android dédiée

## 🎯 Fonctionnalités
### Contrôles Globaux
- 🚀 **ON/OFF total** de toutes les lampes
- 🌞 **Montée/descente simultanée** des stores

### Contrôles Individuels
- 💡 **Lampe par lampe** (allumage/extinction)
- 🪟 **Store par store** (positionnement précis)

## 🛠️ Configuration Technique
| Composant | Modèle | Qty |
|-----------|--------|-----|
| Module Loxone | Miniserver Gen2 | 1 |
| Relais | KNX 8x230V | 1 |
| Alimentation | MeanWell 24V/5A | 1 |
| Lampes | LED 12W 2700K | 4 |
| Stores | Somfy Sonesse 30 | 2 |

```mermaid
graph TB
    A[Interface Manuelle] -->|Fils| B[Loxone Miniserver]
    C[PC Loxone Config] -->|Ethernet| B
    D[App Android] -->|WiFi| B
    B --> E[Relais KNX]
    E --> F[Lampes]
    E --> G[Stores]
