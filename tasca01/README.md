# 🗂️ T01: DRP: Còpies de Seguretat  
### *Estudi de cas: Muntatges i Serveis Tècnics SL (Treball cooperatiu)*

Aquest repositori conté el desenvolupament complet de l’activitat **T01 de DRP (Disaster Recovery Plan)**, centrada en el disseny i planificació d’un sistema eficient de còpies de seguretat basat en un **cas pràctic realista** i treballat en diferents fases: individual, per parelles i en grup.

---

## 🏢 Cas d’estudi: “Muntatges i Serveis Tècnics SL”

L’empresa és una PIME dedicada a la instal·lació i manteniment d’equips industrials. La seva infraestructura tècnica inclou:

- **Servidor de fitxers (Ubuntu Server)** amb:
  - Documents de projectes (300 GB)
  - Bases de dades de comptabilitat i clients (20 GB)
  - Carpetes personals d’usuari (100 GB)
- **10 equips clients** Windows 10/11
- **Connexió a Internet:** fibra simètrica 600 Mbps  

### Requisits de recuperació
- **RTO:** < 4 hores per a dades de Comptabilitat/Clients  
- **RPO:**  
  - General: < 24 hores  
  - Comptabilitat/Clients: < 4 hores  
- **Retenció mínima:** 1 mes

---

## 🧩 Fases del Treball

### 🔸 Fase 1 — Treball individual
Cada alumne respon:
1. **Què copiar?** (dades crítiques i priorització)  
2. **Periodicitat i tipus de còpia** (completa/diferencial/incremental)  
3. **Mitjans i ubicació** seguint la regla **3-2-1**  

---

### 🔸 Fase 2 — Treball per parelles  
Les parelles:  
1. Comparen i discuteixen les respostes individuals  
2. Elaboren una **proposta consensuada d’esquema 3-2-1**

Inclou taula de:  
- Dades crítiques  
- Periodicitat  
- Tipus de còpia  
- Mitjà local  
- Mitjà extern  

---

### 🔸 Fase 3 — Treball en grup  
El grup:
1. Presenta i compara totes les propostes  
2. Debat pros i contres (cost, simplicitat, seguretat, RTO/RPO)  
3. Redacta la **Política Final de Còpies de Seguretat** per presentar a l’empresa

---

## 📂  Estructura de carpetes

Dins la carpeta `tasca01` es troben els següents arxius:

- `activitat.md`: Activitat centrada en el disseny i planificació d’un sistema eficient de còpies de seguretat.

---

## 📎  Documents
Podeu consultar tots els documents fent clic al document corresponent:
- Al arxiu [activitat](activitat.md) podeu trobar la activitat.
