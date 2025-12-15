# 🖥️✨ T06: Accés Remot — Escriptori Remot (RDP) (tasca individual)

En la tasca anterior vam treballar l’administració remota via SSH, essencial per a servidors i sistemes sense entorn gràfic.  
Ara avancem cap al segon gran pilar del suport tècnic: **l’accés remot gràfic**.

Quan un client diu coses com:

- "No em funciona el programa X",  
- "Tinc un error estrany a la pantalla",  
- "No puc accedir a una opció",  

necessitem **veure exactament el que veu ell** i controlar el seu equip de forma remota. Aquí entra en joc la tecnologia RDP.

---

## 🧭 Context

**RDP (Remote Desktop Protocol)** és:

- L’estàndard de Microsoft per accedir a escriptoris Windows.  
- La tecnologia més utilitzada en entorns de suport tècnic.  
- Compatible avui en dia amb Linux (GNOME, Zorin OS), ampliant molt les opcions d’administració remota.

A la consultora EverPia donem suport a:

- Windows 10 / Windows 11  
- Windows Server  
- Zorin OS 18  

Per tant, és imprescindible dominar totes les combinacions possibles d’accés remot:

- Windows → Windows  
- Windows → Linux  
- Linux → Windows  
- Linux → Linux  

---

## 🎯 Objectiu de la PoC

Crear documentació interna clara, visual i completa perquè futurs becaris puguin establir connexions RDP de manera autònoma.

Les guies han d’explicar:

### 1️⃣ Connexió RDP des de Windows  
Amb *Remote Desktop Connection* o *Microsoft Remote Desktop*.

### 2️⃣ Connexió RDP des de Linux  
Mitjançant:

- Remmina  
- GNOME Connections  
- xfreerdp  

### 3️⃣ Configuració del servidor (Windows i Zorin OS)  
Incloent:

- Activació del servei RDP  
- Configuració d’usuaris i permisos  
- Ports i firewall  
- Bones pràctiques de seguretat  

---

## 📂 Estructura de carpetes

Dins la carpeta `tasca06` trobaràs:

- `activitat.md`: Guia per a fer connexions RDP des de Windows i Linux.

---

## 📎 Documents

Consulta cada guia aquí:

- Al arxiu [activitat.md](activitat.md) pots trobar la Guia d'Accés Remot RDP completa.
