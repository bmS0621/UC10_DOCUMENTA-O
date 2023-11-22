## Neste codigo fizemos um arquivo no excel com tabela de notas de alunos, e passamos para um codigo em python, usando bibiliotecas que a linguaguem nos disponibiliza
---

```

import pandas as pd

df = pd.read_excel("base_notas.xlsx")

df['Média'] = df[['Nota1', 'Nota2', 'Nota3', 'Nota4']].mean(axis=1)
df.to_excel('nota_aluno.xlsx',index=False)

```

---

>[!WARNING]
> Na primeira linda deste codigo (`Import pandas as pd`), estou importanto uma biblioteca do python,
e dando um nome a ela "**PD**", logo após criamos um df (`df = pd.read_execel("base_notas.xlsx`) e fizemos a leitura do excel que tinhamos criado com as notas, na terceira  (`df['Média'] = df[['Nota1', 'Nota2', 'Nota3', 'Nota4']].mean(axis=1)`) e quarta (`df.to_excel('nota_aluno.xlsx',index=False)`)linha basicamente estamos exibindo as notas.

