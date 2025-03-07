# Puertas lógicas práctica

### 1. Un sistema de seguretat bloqueja una porta si dues condicions es compleixen simultàniament. Un sistema de seguretat bloqueja una porta si la càmera detecta una cara desconeguda (A) i el sensor de moviment indica activitat (B).

#### **Expressió en Àlgebra de Boole:**
```
(T XOR B)
```

#### **Taula de la veritat:**
| T (Temperatura > 30) | B (Botó premut) | Ventilador (V) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

---
### 2. Un altaveu activa un so d’alerta només si ni el detector de fum ni el detector de monòxid de carboni han estat activats.

#### **Expressió en Àlgebra de Boole:**
```
NOT (F OR C)
```

#### **Taula de la veritat:**
| F (Fum) | C (Monòxid) | So d'alerta (S) |
|---|---|---|
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

---
### 4. Una reixa elèctrica s’activa només si una clau o una empremta digital són vàlides, però no ambdues alhora.

#### **Expressió en Àlgebra de Boole:**
```
K XOR E
```

#### **Taula de la veritat:**
| K (Clau vàlida) | E (Empremta vàlida) | Reixa activada (R) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

---
### 6. Un polsador d'emergència ha de ser premut per dues persones per activar una sirena.

#### **Expressió en Àlgebra de Boole:**
```
P1 AND P2
```

#### **Taula de la veritat:**
| P1 | P2 | Sirena (S) |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

---
