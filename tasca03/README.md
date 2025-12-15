# 🗂️ T03: Pla de Recuperació davant Desastres  
### *Imatges del sistema – Prova de concepte amb Rescuezilla*

Aquesta tasca forma part del Pla de Contingència i Continuïtat del Negoci que el client està desenvolupant.  
Dins d’aquest pla, s’inclou el **DRP (Disaster Recovery Plan)**, que defineix les mesures necessàries per recuperar ràpidament l’activitat en cas d’avaria, robatori o desastre.

En aquesta activitat es treballa especialment un component crucial del DRP:  
👉 **La creació i restauració d’imatges completes del sistema** per reduir al mínim el temps de recuperació dels equips dels treballadors.

Els equips del client utilitzen **Zorin OS 18** amb configuracions i aplicacions específiques que cal preservar.

---

# 🔹 Fase 1 — Anàlisi i justificació de la solució tècnica

En aquesta fase cal investigar diverses eines capaces de crear imatges completes del disc (sistemes, configuracions i aplicacions).

La comparativa ha d’incloure:
- 2 eines **comercials**
- 2 eines **de comunitat**
- Característiques destacades
- Preu aproximat
- Punts forts i febles
- Valoració final i justificació de la solució recomanada

L’objectiu és triar l’eina que millor encaixa amb les necessitats de l’empresa.

---

# 🔹 Fase 2 — Guia tècnica amb Rescuezilla

Tot i que la comparativa pot recomanar un altre producte, **la prova de concepte i la guia tècnica s’han de fer amb Rescuezilla**, per evitar dependències comercials i facilitar l’avaluació.

La guia ha d’incloure:

### ✔️ 1. Creació d’una imatge completa del sistema
- Arrencada amb Rescuezilla Live  
- Selecció del disc d’origen  
- Elecció del destí (unitat externa, carpeta, etc.)  
- Configuració d’opcions d’imatge  
- Procés de validació  

### ✔️ 2. Restauració de la imatge en un equip “net”
Cal crear una màquina virtual idèntica a l’original:
- Mateixa RAM  
- Mateix processador  
- Mateixa interfície de xarxa  
- Mateix disc (mida i tipus)

Passos documentats:
- Arrencar Rescuezilla a la màquina neta  
- Seleccionar la imatge creada  
- Restaurar completament el disc  
- Validar que el sistema arrenca correctament  

La guia ha d’incorporar:
- Captures de pantalla
- Explicacions pas a pas
- Advertències i bones pràctiques  

---

# 📂 Estructura de carpetes

Dins la carpeta `tasca03` es troben els següents arxius:

- `comparativa.md`: Document amb la comparativa d'eines comercials i de comunitat i la justificació de la solució escollida.
- `rescuezilla.md`: Guia tècnica completa amb la creació i restauració d’imatges utilitzant Rescuezilla.

---

## 📎 Documents

Podeu consultar els documents fent clic al fitxer corresponent:

- A l’arxiu [comparativa.md](comparativa.md) podeu trobar la comparativa de solucions i la justificació final.
- A l’arxiu [rescuezilla.md](rescuezilla.md) podeu trobar la guia tècnica de creació i restauració d’imatges amb Rescuezilla.

