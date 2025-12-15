# 🗂️✨ T09: Servidor fitxers Linux. NFS (tasca individual)

En aquesta tasca implementarem un **servidor de fitxers centralitzat** amb NFS (Network File System) per a entorns Linux, seguint les necessitats del client.

---

## 🧭 Context

**Client:** DevOptimize Solutions  
- Startup de desenvolupament de programari que treballa exclusivament amb Linux.  
- Problema: els desenvolupadors tenen còpies locals del codi font i dels actius, causant errors de versió i pèrdua d’eficiència.  
- Requisit: centralitzar dades sense entorn d’autenticació centralitzada.  

La solució escollida: **NFSv3**, la més ràpida i eficient per entorns Linux sense LDAP o Kerberos.

---

## 🎯 Objectiu de la tasca

- Crear un **servidor NFS** i un **client Linux** que consumeixi els recursos compartits.  
- Simular usuaris i grups del client per provar el control d’accés.  
- Configurar opcions d’exportació en `/etc/exports` i permisos del sistema de fitxers (`chmod`, `chown`).  
- Fer una demostració de la solució i documentar-ne les limitacions i el funcionament.

---

## 📂  Estructura de carpetes

Dins la carpeta `tasca09` es troben els següents arxius:

- `activitat.md`: Documentació de la creació del servidor fitxers Linux.

---

## 📎 Documents

Podeu consultar tots els documents fent clic al document corresponent:
- Al arxiu [activitat](activitat.md) podeu trobar la activitat.