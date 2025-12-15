# 🖨️✨ T10: Servidor impressió Linux. CUPS (tasca individual)

A la consultora EverPia, un dels punts més caòtics en qualsevol oficina és la gestió d’impressores: drivers incompatibles, costos de tòner descontrolats i equips que no saben a quina impressora enviar la feina.  
La solució professional és implementar un **Servidor d’Impressió Centralitzat**.

---

## 🧭 Context

**Client:** DevOptimize Solutions  
- Vol centralitzar la impressió en tots els seus departaments amb clients Linux (Zorin OS) i servidors Ubuntu.  
- Requisit: demostrar que un servidor Linux pot gestionar i compartir impressores de manera transparent.

Per a la prova, s’utilitzarà **cups-pdf**, una impressora virtual que genera un fitxer PDF en lloc d’imprimir en paper.

---

## 🎯 Objectiu de la PoC

- Configurar un servidor Ubuntu amb **CUPS** i una impressora virtual cups-pdf.  
- Configurar el client Zorin OS perquè pugui enviar treballs d’impressió al servidor.  
- Verificar que els fitxers PDF s’han generat correctament al servidor.  
- Documentar totes les comandes i passos, amb captures de pantalla, per demostrar el funcionament de la prova.

---

## 🖥️ Escenari de treball

- **Màquina 1 (Servidor):** Ubuntu Server amb interfície NAT i segona interfície Host-Only  
- **Màquina 2 (Client):** Zorin OS amb mateixa configuració de xarxa que el servidor  

### Passos de la PoC
1. Instal·lació de CUPS al servidor  
2. Instal·lació de la impressora virtual cups-pdf  
3. Configuració de CUPS per escoltar per totes les interfícies  
4. Compartició de la impressora via el frontal web de CUPS  
5. Afegir la impressora al client Zorin OS  
6. Provar la impressió de diversos documents  
7. Comprovar al servidor els PDFs generats corresponents als treballs impresos

---

## 📂 Estructura de carpetes

Dins la carpeta `tasca10` trobaràs:

- `server/` → Configuració i scripts del servidor CUPS  
- `client/` → Configuració del client Zorin per enviar treballs d’impressió  
- `README.md` → Guia de la tasca (aquest document)  

---

## 📎 Documents

- La documentació amb totes les comandes, passos i captures es troba dins la mateixa carpeta `tasca10` en els fitxers del servidor i client.
