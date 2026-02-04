
# 🔍 Scapy-Network — Escaneo de red con Scapy

Este repositorio contiene un conjunto de scripts escritos en **Python** utilizando la librería **Scapy**, una potente herramienta para manipulación de paquetes, escaneo, análisis y descubrimiento de red. citeturn16search120

Los scripts incluidos permiten realizar **escaneos de puertos**, análisis de respuesta TCP y otras técnicas esenciales para reconocimiento de red.

---
## 🚀 Funcionalidades principales
- Escaneo de puertos TCP mediante creación de paquetes personalizados. (Script `Scan_tcp.py`) citeturn16search119
- Escaneo general de red (`scan_all.py`). citeturn16search119
- Uso directo de la librería Scapy para enviar, recibir y analizar paquetes.
- Ideal para pruebas de conectividad, pentesting controlado y análisis educativo.

---
## 📁 Contenido del repositorio
```
Scapy-Network/
├── Scan_tcp.py       # Escaneo TCP de puertos
├── scan_all.py       # Escaneo general de red
└── README.md         # Este archivo
```
citeturn16search119

---
## ▶️ Cómo usar los scripts
### 1. Clona el repositorio
```bash
git clone https://github.com/Victor-AFT/Scapy-Network
cd Scapy-Network
```

### 2. Instala Scapy
```bash
pip install scapy
```
*(Scapy es una librería de manipulación de paquetes altamente flexible) citeturn16search122*

### 3. Ejecuta un escaneo TCP
```bash
python Scan_tcp.py
```

### 4. Escaneo completo de red
```bash
python scan_all.py
```

---
## 📊 Ejemplo conceptual de uso de Scapy
```python
from scapy.all import IP, TCP, sr1

packet = IP(dst="192.168.1.10")/TCP(dport=80, flags="S")
response = sr1(packet, timeout=1)
if response:
    print("Puerto 80 responde")
```
*(Ejemplo basado en documentación oficial de Scapy) citeturn16search120*

---
## 📚 Recursos recomendados
- Documentación oficial Scapy: citeturn16search121
- PyPI Scapy (instalación, guía rápida): citeturn16search122
- Tutoriales de manipulación de paquetes y escaneo con Scapy.

---
## 🔧 Mejoras futuras sugeridas
- Añadir escaneo UDP.
- Implementar detección de SO (fingerprinting).
- Exportar resultados en JSON.
- Añadir modo interactivo.

---
## 🤝 Contribuciones
Las contribuciones son bienvenidas. Puedes crear **issues** o enviar **pull requests**.

---
## 📜 Licencia
Uso libre para fines personales, educativos y de investigación.

