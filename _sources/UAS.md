---
title: UAS

---



| P        | Q         | R         | S        | R->Q     | R->S     | (R->Q)->(R->S)   |
| -------- | --------  | --------  | -------- | -------- | -------- | ---------------- |
|T         |T          |T          |T         |T         |T         |T                 |
|T         |T          |T          |T         |T         |T         |T                 |
|T         |T          |F          |T         |T         |T         |T                 |
|F         |T          |F          |F         |T         |T         |T                 |
|F         |F          |F          |F         |T         |T         |T                 |
|T         |F          |T          |T         |T         |T         |T                 |
|F         |F          |F          |T         |T         |T         |T                 |
|F         |T          |T          |T         |T         |T         |T                 |

(R->Q)->(R->S)


![1](https://hackmd.io/_uploads/rkoudGVEyl.png)

# HITUNG CLOSNES CENTRALITY DARI G

| node |        a |        b |        c |        d |        e |        f |        g |
| -----| -------- | -------- | -----    | -------- | -------- | -----    | -------- |
| g    | 3        | 3        |2         | 1        | 1        |2         |0         |

$C_c(G) = \frac{7 - 1}{3 + 3 + 2 + 1 + 1 + 2 + 0} = \frac{6}{12}$
# HITUNG BETWEENNESS CENTRALITY CENTRALITY F

| node |        a |        b |        c |        d |        e |        f |        g |
| -----| -------- | -------- | -----    | -------- | -------- | -----    | -------- |
| f    | 4        | 4        |3         | 2        | 1        |0         |2         |

$C_B(F) = 1 + 1 + 1 + 1 + 1 + 1 + 1 = 7$