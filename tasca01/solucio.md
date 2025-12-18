# T01: DRP: còpies de seguretat  
## Estudi cas client (treball cooperatiu)

---

## Fase 1: Treball individual

### 1. Què copiar? (Priorització)

**Quines són les dades més crítiques del servidor? Cal fer còpia dels 10 equips clients? Justifica-ho.**

#### Què copiar?
Les dades més crítiques del servidor són:

- **Bases de Dades de Comptabilitat i Clients (20 GB)**  
  Són les més importants perquè tenen canvis constants i uns requisits estrictes de recuperació (**RTO i RPO de 4 hores**).

- **Documents de Projectes (300 GB)**  
  Contenen informació essencial per al funcionament i el treball diari de l’empresa.

- **Carpetes Personals dels usuaris (100 GB)**  
  Formen part de la feina quotidiana i cal garantir-ne la recuperació.

#### Cal fer còpia dels equips clients?
No és necessari fer una còpia completa dels **10 equips clients**, ja que la informació rellevant es troba centralitzada al servidor i la majoria d’usuaris hi treballen directament.  
Tot i això, es recomana protegir la carpeta **Documents dels tècnics**, ja que de manera puntual poden guardar-hi arxius importants.

---

### 2. Periodicitat i Tipus de Còpia

**Proposta de calendari bàsic (diari / setmanal / mensual) i tipus de còpia.**

Per complir els requisits de **RTO, RPO i retenció**, es proposa el següent calendari:

#### Bases de Dades de Comptabilitat i Clients (dades crítiques)
- **Còpia incremental cada 4 hores (diària)**  
  *Justificació:* dades amb canvis constants; només es poden perdre 4 hores de treball.
- **Còpia completa setmanal (diumenge)**.
- **Retenció mensual** amb una còpia completa guardada **1 cop al mes**.

#### Documents de Projectes i Carpetes Personals
- **Còpia incremental diària (1 cop al dia)**  
  *Justificació:* el RPO és de 24 hores.
- **Còpia completa setmanal (diumenge)**.
- **Còpia completa mensual** per mantenir l’historial del darrer mes.

---

### 3. Mitjans i Ubicació de la Còpia

**Quin tipus de mitjà de còpia utilitzar i on guardar-la (Regla 3-2-1).**

#### Mitjans de còpia proposats
- **NAS local**  
  Per fer les còpies diàries i setmanals amb rapidesa i permetre restauracions ràpides (important per complir l’RTO de 4 hores).

- **Còpia al núvol (Cloud Backup)**  
  Per disposar d’una còpia externa i protegida davant desastres físics.

- **Disc dur extern (opcional, còpia mensual)**  
  Com a suport addicional, desconnectat i útil per a còpies manuals.

#### Regla 3-2-1 aplicada
- **3 còpies de les dades:** dades originals + NAS + còpia al núvol.
- **2 tipus de mitjans diferents:** NAS local i servei Cloud.
- **1 còpia fora del lloc:** còpia al núvol.

#### Ubicació de la còpia més recent
La còpia més recent s’ha de guardar al **NAS local**, ja que és el sistema més ràpid per restaurar les dades crítiques i complir el **RTO de 4 hores**.



## Fase 2: Treball per Parelles

### Treballant per parelles

1. **Discussió i Consens**
   - Comparació de les respostes individuals (Fase 1).

2. **Elaboració d'una Proposta Unificada**
   - Disseny de l’Esquema 3-2-1 de Còpies (3 còpies, 2 mitjans, 1 fora de lloc) basat en els requisits del cas.

| Element              | Proposta de la Parella                                            | Justificació                                                                 |
|---------------------|------------------------------------------------------------------|----------------------------------------------------------------------------|
| **Dades Crítiques**  | Bases de dades de Comptabilitat/Clients, documents de Projectes i Carpetes Personals | Bases de dades amb canvis constants i RPO/RTO de 4 h; documents i carpetes essencials, no poden perdre’s més de 24 h. |
| **Periodicitat (BD)**| Còpies cada 4 hores (incrementals) + completa setmanal          | Complim RPO de 4 hores i mantenim una còpia estable setmanal.             |
| **Tipus de Còpia (BD)** | Incremental diària (cada 4 h) + Completa setmanal + Completa mensual | Incremental permet freqüència alta i poc espai; la completa garanteix punts de restauració fiables. |
| **Mitjà 1 (Local)**  | NAS dins l’empresa                                               | Restauració ràpida per complir RTO de 4 hores; alta velocitat i automatització. |
| **Mitjà 2 (Extern)** | Còpia al Núvol (Cloud Backup)                                   | Garanteix la còpia “off-site” de la regla 3-2-1, protegint davant robatori, incendi o fallada total del local. |

# T01: DRP: Còpies de Seguretat – Fase 3 (Treball en Grup)

## Política de Còpies de Seguretat – Muntatges i Serveis Tècnics SL

### 1) Dades Objecte de Còpia

#### Servidor

**Dades crítiques (còpia més freqüent):**
- Bases de dades de Comptabilitat i Clients (20 GB)  
  - Còpia incremental cada 4 hores  
  - Còpia completa setmanal

**Dades importants però no crítiques:**
- Documents de Projectes (300 GB)  
- Carpetes Personals dels usuaris (100 GB)  
  - Còpia incremental diària  
  - Còpia completa setmanal

#### Equips Clients
- No es fa còpia completa dels 10 PCs  
- Només es protegeix la carpeta **Documents** dels tècnics amb còpia diària (incremental)  
- La informació rellevant està centralitzada al servidor

---

### 2) Cronograma Setmanal Detallat

| Dia       | Dades                             | Tipus de còpia      | Mitjà                  |
|-----------|----------------------------------|------------------|-----------------------|
| Dilluns   | BD (cada 4 h), Documents, Carpetes | Incremental      | NAS                   |
| Dimarts   | BD (cada 4 h), Documents, Carpetes | Incremental      | NAS                   |
| Dimecres  | BD (cada 4 h), Documents, Carpetes | Incremental      | NAS                   |
| Dijous    | BD (cada 4 h), Documents, Carpetes | Incremental      | NAS                   |
| Divendres | BD (cada 4 h), Documents, Carpetes | Incremental      | NAS                   |
| Dissabte  | BD (cada 4 h), Documents, Carpetes | Incremental      | NAS                   |
| Diumenge  | Totes les dades del servidor       | Completa setmanal| NAS + núvol           |

**Còpia mensual:**  
- El primer diumenge de cada mes s’emmagatzema una còpia completa al núvol com a punt de retenció llarg.

---

### 3) Elecció de Mitjans i Ubicació (Regla 3-2-1)

**Mitjà 1 (Local):** NAS empresarial ubicat al rack de l’empresa.  
- Permet automatitzar totes les còpies incrementals i setmanals amb alta velocitat.

**Mitjà 2 (Extern):** Còpia al núvol utilitzant un servei com Azure Backup o Google Cloud Storage.  
- Garanteix còpia segura fora de l’empresa i protegeix davant incendis, robatoris o fallades totals.

**Ubicació fora de lloc:** La còpia externa es guarda al núvol (off-site lògic).  
- La gestió i verificació de restauracions és responsabilitat del tècnic de sistemes.  

**Compliment de la Regla 3-2-1:**  
- 3 còpies: dades originals + NAS + Cloud  
- 2 mitjans diferents: NAS i Cloud  
- 1 còpia fora de lloc: núvol

---

### 4) Estratègia de Recuperació (RTO/RPO)

**Per a les dades de Comptabilitat i Clients:**

- **RPO (4 hores)**  
  - Còpies incrementals cada 4 hores  
  - Assegura que mai es perd més que l’interval de treball

- **RTO (4 hores)**  
  - Restauració directa des del NAS local  
  - Còpia completa setmanal + incrementals permet reconstruir l’estat de la BD ràpidament

**En cas de desastre total:**  
- Restauració des del núvol, amb temps addicional però mantenint les dades intactes.
