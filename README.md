

---

# Comparação entre Algoritmos para Encontrar o Par de Pontos Mais Próximos em 2D

Este projeto compara dois algoritmos para o problema de encontrar o par de pontos mais próximos em um plano 2D. O objetivo é analisar o desempenho de ambos os algoritmos através de testes experimentais, medindo o tempo de execução para diferentes tamanhos de entrada.

## Algoritmos Comparados

1. **Força Bruta (O(n²))**  
   Este algoritmo calcula a distância entre cada par de pontos e retorna a menor distância.  
   **Complexidade**: O(n²)

2. **Divisão e Conquista (O(n log n))**  
   Algoritmo recursivo que divide os pontos em subgrupos e encontra o par mais próximo de maneira mais eficiente.  
   **Complexidade**: O(n log n)

## Objetivo

- Comparar o desempenho dos dois algoritmos para diferentes tamanhos de entrada.
- Medir o tempo de execução em função do tamanho da entrada.
- Garantir que ambos os algoritmos fornecem resultados consistentes para as mesmas entradas.

## Requisitos

- **Python 3.x**
- Bibliotecas:
  - `numpy`
  - `matplotlib`

### Instalação das Dependências

Certifique-se de que as dependências estão instaladas:

```bash
pip install numpy matplotlib
```

## Como Executar

1. **Configuração do Ambiente Virtual**  
   É recomendável usar um ambiente virtual para isolar as dependências do projeto. Para isso, crie e ative o ambiente virtual:

   - **Windows**:
     ```bash
     .venv\Scripts\activate
     ```
   - **Linux/macOS**:
     ```bash
     source .venv/bin/activate
     ```

2. **Executando o Código**  
   O código está contido nos notebooks Jupyter. Você pode rodá-los usando o Jupyter Notebook ou JupyterLab.

   Se o Jupyter não estiver instalado, instale-o com:

   ```bash
   pip install jupyter
   ```

   Após a instalação, execute o comando abaixo para iniciar o Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

   Isso abrirá o navegador e você poderá acessar o arquivo `comparacao_algoritmos_pontos_proximos.ipynb`.

3. **Execução dos Testes**  
   Dentro do notebook `comparacao_algoritmos_pontos_proximos.ipynb`, você encontrará o código que executa os testes de comparação entre os algoritmos. O notebook gerará gráficos comparando o tempo de execução de cada algoritmo para diferentes tamanhos de entrada.

## Detalhes dos Algoritmos

1. **Força Bruta**  
   - Para cada par de pontos, calcula-se a distância Euclidiana.
   - Complexidade: O(n²), onde `n` é o número de pontos.
   
2. **Divisão e Conquista**  
   - Divisão recursiva dos pontos, agrupando-os e tratando as sublistas.
   - Complexidade: O(n log n), onde `n` é o número de pontos.

## Testes e Resultados

Os testes são realizados para tamanhos de entrada que variam de 10 a 10.000 pontos. A cada tamanho `n`, o código executa os algoritmos `m` vezes, onde `m` é escolhido aleatoriamente entre 10 e 20 repetições para garantir consistência nos resultados.

- **Gráfico**: O código gera um gráfico comparando os tempos de execução de cada algoritmo.
- **Análise Esperada**:  
   - **Força Bruta** tende a ser mais lento conforme o número de pontos cresce, devido à sua complexidade quadrática.
   - **Divisão e Conquista** deve apresentar um crescimento mais suave no tempo de execução, com um desempenho significativamente melhor para entradas grandes.

## Estrutura do Projeto

```
.
├── .venv/                            # Ambiente Virtual
├── beta_test_pontos_proximos.ipynb     # Testes dos algoritmos
├── comparacao_algoritmos_pontos_proximos.ipynb # Comparação entre os algoritmos
└── README.md                          # Documentação do projeto
```

## Contribuidores

- **Alysson Sousa Silva**
- **Sara Ponte de Souza**

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

---

### Melhorias no README

- **Estrutura mais clara**: Organizei as seções para tornar o arquivo mais legível e acessível.
- **Explicações concisas**: O conteúdo foi reescrito para ser mais direto e fácil de entender.
- **Exemplo de execução**: Esclareci como rodar o projeto e gerar os resultados.

