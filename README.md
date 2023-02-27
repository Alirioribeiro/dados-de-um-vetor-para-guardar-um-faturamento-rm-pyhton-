# dados-de-um-vetor-para-guardar-um-faturamento-rm-pyhton-
# Define o faturamento mensal por estado
faturamento = {
    'SP': 67836.43,
    'RJ': 36678.66,
    'MG': 29229.88,
    'ES': 27165.48,
    'Outros': 19849.53
}

# Calcula o faturamento total
total = sum(faturamento.values())

# Calcula o percentual de representação de cada estado
percentuais = {estado: (valor / total) * 100 for estado, valor in faturamento.items()}

# Imprime os resultados
for estado, percentual in percentuais.items():
    print(f'{estado}: {percentual:.2f}%')
