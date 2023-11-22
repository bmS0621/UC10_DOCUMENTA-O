```

import pandas as pd

df = pd.read_excel("base_notas.xlsx")

df['Média'] = df[['Nota1', 'Nota2', 'Nota3', 'Nota4']].mean(axis=1)
df.to_excel('nota_aluno.xlsx',index=False)

```
Na primeira linda deste codigo, estou importanto uma biblioteca do python,
e dando um nome a ela "**PD**", logo após criamos um df e fizemos a leitura do excel que tinhamos criado com as notas, na terceira linha estamos exibindo as notas.

