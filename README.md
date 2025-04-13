# 🔍 Modelamiento de Amplificadores Operacionales (Op-Amps)

Los **amplificadores operacionales (Op-Amps)** son componentes clave en la electrónica analógica. Son utilizados para amplificar señales, operar matemáticamente sobre ellas (suma, resta, integración, derivación), y como bloques fundamentales en filtros, osciladores, reguladores y sistemas de control.

El modelamiento de Op-Amps facilita el análisis y diseño de circuitos electrónicos, partiendo de un enfoque ideal y extendiéndose al comportamiento real.

---

## 📘 Conceptos Clave

- **Op-Amp (Amplificador Operacional):** Dispositivo electrónico de ganancia muy alta que amplifica la diferencia entre dos entradas.
- **Entradas:**
  - \( V^+ \): Entrada no inversora
  - \( V^- \): Entrada inversora
- **Salida:** \( V_{out} \): Salida amplificada
- **Modo ideal:** Supuestos más comunes:
  - Ganancia infinita (\( A 	o \infty \))
  - Impedancia de entrada infinita
  - Corriente de entrada nula
  - Voltaje en las entradas igual: \( V^+ = V^- \) (con realimentación negativa)
- **Modo real:** Considera limitaciones como ganancia finita, impedancia de salida no nula, offset, etc.

---

## 🛠️ Aplicaciones

- Amplificadores de señal para sensores
- Filtros activos (pasa bajos, pasa altos, pasa banda)
- Comparadores de voltaje
- Circuitos de integración y derivación
- Sumadores/restadores analógicos
- Controladores en lazo cerrado

---

## 🧪 Ejemplo 1: Amplificador Inversor

### 🎯 Enunciado

Diseñar un amplificador inversor con una ganancia de -10. Se tiene una resistencia de entrada \( R_1 = 1\,k\Omega \). Hallar \( R_f \) y la salida para \( V_{in} = 0.5\,V \).

### ⚙️ Solución

La fórmula para la ganancia de un amplificador inversor es:

```math
V_{out} = -\frac{R_f}{R_1} V_{in}
```

Dado que la ganancia deseada es -10:

```math
\frac{R_f}{R_1} = 10 \Rightarrow R_f = 10 \times R_1 = 10\,k\Omega
```

Para una entrada de \( 0.5\,V \):

```math
V_{out} = -\frac{10k\Omega}{1k\Omega} \cdot 0.5 = -5\,V
```

### 🔧 Resultado:

- \( R_f = 10\,k\Omega \)
- \( V_{out} = -5\,V \)

![Amplificador Inversor](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Op-Amp_Inverting_Amplifier.svg/320px-Op-Amp_Inverting_Amplifier.svg.png)

---

## 🧪 Ejemplo 2: Amplificador No Inversor

### 🎯 Enunciado

Diseñar un amplificador no inversor con una ganancia de 6. Se fija \( R_1 = 1\,k\Omega \). Hallar \( R_f \) y calcular la salida para \( V_{in} = 2\,V \).

### ⚙️ Solución

La fórmula de ganancia es:

```math
V_{out} = \left(1 + \frac{R_f}{R_1}\right) V_{in}
```

Resolviendo para \( R_f \):

```math
1 + \frac{R_f}{R_1} = 6 \Rightarrow \frac{R_f}{R_1} = 5 \Rightarrow R_f = 5 \times R_1 = 5\,k\Omega
```

Salida para \( V_{in} = 2\,V \):

```math
V_{out} = 6 \cdot 2 = 12\,V
```

### 🔧 Resultado:

- \( R_f = 5\,k\Omega \)
- \( V_{out} = 12\,V \)

![Amplificador No Inversor](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Op-Amp_Non-Inverting_Amplifier.svg/320px-Op-Amp_Non-Inverting_Amplifier.svg.png)

---

## 🧩 Conclusión

El modelamiento de amplificadores operacionales permite comprender, diseñar y optimizar una amplia gama de circuitos analógicos. Estos dispositivos, al ser configurables para diversas funciones, son herramientas indispensables en sistemas electrónicos, automatización, procesamiento de señales y control. Su estudio teórico y práctico es fundamental para cualquier ingeniero en electrónica o mecatrónica.

