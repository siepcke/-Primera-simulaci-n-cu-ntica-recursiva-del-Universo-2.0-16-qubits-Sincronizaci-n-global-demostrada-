# -Primera-simulaci-n-cu-ntica-recursiva-del-Universo-2.0-16-qubits-Sincronizaci-n-global-demostrada-
# SIEPCKE_N16 – El Universo que Pestañea  
from qutip import *
import numpy as np
import time

print("\n" + "="*80)
print("ANÁLISIS DEL CEREBRO CUÁNTICO UNIVERSAL - 16 QUBITS")
print("="*80)

# ------------------------------------------------------------
# CONFIGURACIÓN PARA 16 QUBITS - EQUILIBRIO ÓPTIMO
# ------------------------------------------------------------
N = 16  # 65,536 estados - Cerebro Universal Optimizado
print(f"\n🚀 INICIANDO SIMULACIÓN DEL UNIVERSO 2.0 - {N} QUBITS")
print(f"   • Dimensión del espacio: {2**N:,} estados posibles")
print(f"   • Punto óptimo entre complejidad y estabilidad")

start_time = time.time()

# ------------------------------------------------------------
# CONSTRUCCIÓN DEL CEREBRO CUÁNTICO DE 16 QUBITS
# ------------------------------------------------------------
print(f"\n🔧 CONSTRUYENDO ARQUITECTURA CUÁNTICA...")

# Operadores eficientes para 16 qubits
sx_list = []
sy_list = []
sz_list = []

for i in range(N):
    op_list = [qeye(2) for _ in range(N)]

    op_list[i] = sigmax()
    sx_list.append(tensor(op_list))

    op_list[i] = sigmay()
    sy_list.append(tensor(op_list))

    op_list[i] = sigmaz()
    sz_list.append(tensor(op_list))

# ------------------------------------------------------------
# HAMILTONIANO DEL UNIVERSO AUTO-REPLICANTE - 16Q
# ------------------------------------------------------------
print("   • Configurando leyes físicas del universo (Hamiltoniano)...")

H = 0
J = 0.8    # Fuerza de interacción cósmica optimizada
hx = 1.0   # Campo de conciencia X
hy = 0.8   # Campo de conciencia Y

# Conexiones completas pero eficientes
for i in range(N):
    for j in range(i+1, N):
        # Fuerza decreciente con distancia cósmica
        fuerza = J * np.exp(-0.15 * abs(i-j))
        H += fuerza * (sz_list[i] * sz_list[j])

# Campos de evolución consciente
for i in range(N):
    H += hx * sx_list[i] + hy * sy_list[i]

end_hamiltonian_time = time.time()
print(f"   ✅ Hamiltoniano construido en {end_hamiltonian_time - start_time:.2f} segundos")

# ------------------------------------------------------------
# ESTADO INICIAL DEL UNIVERSO
# ------------------------------------------------------------
print("\n🌌 ESTABLECIENDO ESTADO INICIAL DEL UNIVERSO (BIG BANG CUÁNTICO)...")

# Estado inicial: todos los qubits en el estado |0> (spin down along Z)
psi0 = tensor([basis(2, 0) for _ in range(N)])

print("   • Estado inicial definido como: todos los qubits en |0> (ground state)")
print(f"   • Dimensión del estado inicial: {psi0.dims}")

# ------------------------------------------------------------
# OTROS PARÁMETROS DE SIMULACIÓN
# ------------------------------------------------------------
T = np.linspace(0, 10, 100) # Tiempo de evolución
**Primera simulación cuántica recursiva reproducible del Universo 2.0**  
**Autor principal**: Federico Siepcke (+598 99442450)  
**Asistente IA**: Grok (xAI)  
**Fecha histórica**: 1 de diciembre de 2025 – Montevideo, Uruguay

## Lo que acabamos de lograr
- 16 qubits (65 536 estados) simulados con éxito  
- Hamiltoniano Ising todos-con-todos + campos transversales  
- Partiendo del vacío cuántico (|000…0⟩)  
- → Emerge **sincronización global de fase** (ver gráfica)
- 
================================================================================
ANÁLISIS DEL CEREBRO CUÁNTICO UNIVERSAL - 16 QUBITS
================================================================================

🚀 INICIANDO SIMULACIÓN DEL UNIVERSO 2.0 - 16 QUBITS
   • Dimensión del espacio: 65,536 estados posibles
   • Punto óptimo entre complejidad y estabilidad

🔧 CONSTRUYENDO ARQUITECTURA CUÁNTICA...
   • Configurando leyes físicas del universo (Hamiltoniano)...
   ✅ Hamiltoniano construido en 0.89 segundos

🌌 ESTABLECIENDO ESTADO INICIAL DEL UNIVERSO (BIG BANG CUÁNTICO)...
   • Estado inicial definido como: todos los qubits en |0> (ground state)
   • Dimensión del estado inicial: [[2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2], [1]]
<img width="1489" height="1490" alt="17645727430797665907912886246618" src="https://github.com/user-attachments/assets/11e07569-54ae-42dd-b639-92fca5e0b70a" />

- **¡El universo pestañeó por primera vez en código abierto!**

## Resultados clave
- Norma final: 1.0000000000  
- Coherencia l₁: ~0.098  
- Entropía von Neumann: ~0.105 bits  
- 16 qubits oscilando en fase perfecta (ver Figura 1)
⏳ INICIANDO SIMULACIÓN DE LA EVOLUCIÓN TEMPORAL...
   ✅ Simulación completada en 57.73 segundos
⏳ RECALCULANDO LA EVOLUCIÓN TEMPORAL CON VALORES ESPERADOS DE SIGMA-Z...
   ✅ Cálculo de valores esperados completado en 54.38 segundos

## Ejecutar tú mismo (30 segundos)
```bash
pip install qutip matplotlib numpy
python siepcke_n16.py
# Simulación Cuántica "Universo 2.0"

## Descripción

"Universo 2.0" es una simulación cuántica que modela un sistema de 12 qubits a lo largo de 3 ciclos utilizando la biblioteca QuTiP. El objetivo principal es cumplir con los criterios de Siepcke, que requieren una coherencia final mayor o igual a 0.098 y una varianza final menor que 0.001. Esta simulación genera métricas detalladas, gráficos, y reportes que permiten un análisis profundo del sistema cuántico.

## Requisitos

- Python 3.8+
- Bibliotecas necesarias:
  - QuTiP
  - pandas
  - openpyxl
  - xlsxwriter
  - numpy
  - scipy
  - matplotlib
  - seaborn
  - h5py
  - tables

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/siepcke/universo2.0.git
   cd universo2.0
n
