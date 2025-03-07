# Puertas lógicas práctica

### 1. Un aspersor de riego se activa si la humedad del suelo es inferior al 20% o si el temporizador programado lo indica, pero no si ambas condiciones ocurren simultáneamente.
#### **Expressió en Àlgebra de Boole:**
```
H XOR T
```

#### **Taula de la veritat:**
| H (Humitat < 20%) | T (Temporitzador) | Aspersor (A) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

---
### 2. El semáforo peatonal se pone en verde si el botón de cruce es presionado y el semáforo de coches está en rojo.
#### **Expressió en Àlgebra de Boole:**
```
B AND R
```

#### **Taula de la veritat:**
| B (Botó premut) | R (Semàfor cotxes vermell) | Semàfor verd (S) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

---
### 3. Una máquina solo se enciende si el botón de encendido es presionado, el sensor de seguridad está activado, y la compuerta de emergencia NO está abierta.
#### **Expressió en Àlgebra de Boole:**
```
B AND S AND (NOT C)
```

#### **Taula de la veritat:**
| B (Botó premut) | S (Sensor activat) | C (Comporta oberta) | Màquina encès (M) |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

---
### 4. Un usuario puede acceder al sistema si introduce la contraseña correcta y además se cumple una de las siguientes condiciones: (1) Se encuentra dentro de la red segura O (2) Introduce un código temporal válido, pero no ambos.
#### **Expressió en Àlgebra de Boole:**
```
P AND (N XOR C)
```

#### **Taula de la veritat:**
| P (Contrasenya correcta) | N (Xarxa segura) | C (Codi vàlid) | Accés (A) |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

---

### 5. Una alarma se activa si el sensor de temperatura detecta sobrecalentamiento o si la presión del aceite es baja, pero solo si el motor está en funcionamiento.
#### **Condició:**
L’alarma s’activa si el sensor de temperatura detecta sobreescalfament (T) o si la pressió de l’oli és baixa (P), però només si el motor està en funcionament (M).

#### **Expressió en Àlgebra de Boole:**
```
(T OR P) AND M
```

#### **Taula de la veritat:**
| T (Sobreescalfament) | P (Pressió baixa) | M (Motor actiu) | Alarma (A) |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 0 |
| 1 | 1 | 1 | 1 |

---

### 6. El ventilador se activa si la temperatura supera los 28°C y además la humedad está por encima del 70% O el modo automático está activado.
#### **Condició:**
El ventilador s’activa si la temperatura supera els 28°C (T) i la humitat està per sobre del 70% (H) **O** el mode automàtic està activat (A).

#### **Expressió en Àlgebra de Boole:**
```
(T AND H) OR A
```

#### **Taula de la veritat:**
| T (Temp > 28°C) | H (Humitat > 70%) | A (Mode automàtic) | Ventilador (V) |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 |

---
