# Fitxa tècnica: Instal·lació i configuració d'un servei SSH segur a Ubuntu Server

## Objectiu
Instal·lar, configurar i assegurar el servei OpenSSH en un sistema operatiu Ubuntu Server per permetre administració remota segura mitjançant claus xifrades.

## Materials
- Màquina virtual o física amb Ubuntu Server 22.04 LTS.
- Client amb terminal (Bash, PowerShell o PuTTY).
- Connexió a Internet i xarxa local activa.

## Procediment
1. Actualitzar els repositoris del sistema operatiu.
2. Instal·lar el paquet del servidor OpenSSH.
3. Verificar que el servei s'està executant correctament.
4. Editar el fitxer de configuració `/etc/ssh/sshd_config` per canviar el port per defecte i desactivar l'accés directe com a `root`.
5. Reiniciar el servei SSH per aplicar els canvis.

```bash
sudo apt update && sudo apt install openssh-server -y
sudo systemctl status ssh

4. Desat el fitxer prement **`Ctrl + S`**.
5. Per veure com queda el document dissenyat, prem **`Ctrl + Shift + V`** a VS Code (obrirà la previsualització).

---

### Pas 2: Fer els commits de Git pel terminal

A la part inferior de VS Code, obre el terminal integrat (**`Ctrl + ~`** o des del menú superior *Terminal > Nuevo terminal*) i executa aquestes comandes una per una per complir amb els requisits de versionat:

```bash
git add fitxa-tecnica.md
git commit -m "Crea estructura de fitxa tècnica"

git add fitxa-tecnica.md
git commit -m "Completa procediment i comprovacions"

git add fitxa-tecnica.md
git commit -m "Revisa format i recursos"

git add fitxa-tecnica.md
git commit -m "Afegeix explicació sobre el flux de treball amb Git"
git log --oneline
git push origin main
