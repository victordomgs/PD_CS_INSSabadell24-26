# Puertas lógicas práctica

1. Un ventilador se activa si la temperatura supera los 30 grados o si el botón de encendido manual está presionado, pero no si ambos criterios se cumplen al mismo tiempo.
#### **Condición:**
El ventilador se activa si la temperatura supera los 30 grados (T) o si el botón de encendido manual está presionado (B), pero no si ambos criterios se cumplen al mismo tiempo.

#### **Expresión en Álgebra de Boole:**
```
(T XOR B)
```

#### **Tabla de la verdad:**
| T (Temperatura > 30) | B (Botón presionado) | Ventilador (V) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

---
2. Una puerta automática se cierra si los sensores no detectan movimiento y el botón de cierre está activado.
#### **Condición:**
La puerta se cierra si los sensores no detectan movimiento (M) y el botón de cierre está activado (B).

#### **Expresión en Álgebra de Boole:**
```
(NOT M) AND B
```

#### **Tabla de la verdad:**
| M (Movimiento) | B (Botón activado) | Puerta (P) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

---
3. Una alarma se dispara si la ventana está abierta y la alarma está habilitada, pero no si la puerta también está abierta.
#### **Condición:**
La alarma se dispara si la ventana está abierta (W) y la alarma está habilitada (A), pero no si la puerta también está abierta (D).

#### **Expresión en Álgebra de Boole:**
```
(W AND A) AND (NOT D)
```

#### **Tabla de la verdad:**
| W (Ventana abierta) | A (Alarma habilitada) | D (Puerta abierta) | Alarma (S) |
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
4. Un sistema de iluminación exterior se enciende si detecta movimiento o si es de noche, pero no si la luz está configurada en modo manual.
#### **Condición:**
El sistema de iluminación exterior se enciende si detecta movimiento (M) o si es de noche (N), pero no si la luz está configurada en modo manual (L).

#### **Expresión en Álgebra de Boole:**
```
(M OR N) AND (NOT L)
```

#### **Tabla de la verdad:**
| M (Movimiento) | N (Noche) | L (Modo Manual) | Luz (Luz encendida) |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 0 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

---
5. Una cafetera comienza a preparar café si el depósito de agua está lleno y se ha programado la hora de inicio, o si el botón de inicio rápido está presionado.  
#### **Condición:**
La cafetera comienza a preparar café si el depósito de agua está lleno (W) y se ha programado la hora de inicio (H), o si el botón de inicio rápido está presionado (B).

#### **Expresión en Álgebra de Boole:**
```
(W AND H) OR B
```

#### **Tabla de la verdad:**
| W (Agua llena) | H (Hora programada) | B (Botón rápido) | Cafetera (Café preparado) |
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
