import pandas as pd
import matplotlib.pyplot as plt

dados = {
    "amostra": [1, 2, 3, 4, 5],
    "expressao_genica": [2.3, 3.1, 4.7, 3.9, 5.2]
}

df = pd.DataFrame(dados)

print("Dados do projeto:")
print(df)

print("\nResumo estatístico:")
print(df.describe())

plt.plot(df["amostra"], df["expressao_genica"])
plt.title("Expressão gênica por amostra")
plt.xlabel("Amostra")
plt.ylabel("Expressão gênica")
plt.show()
