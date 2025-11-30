# projeto-arvores-binarias

# Projeto Árvores de Dados

Este projeto implementa e visualiza duas estruturas de dados fundamentais: Árvore 2-3-4 e Árvore Rubro-Negra. Ambas são árvores balanceadas que garantem operações eficientes de busca, inserção e remoção.

## Objetivo

O objetivo deste projeto é demonstrar o funcionamento, balanceamento e propriedades de duas importantes estruturas de dados de árvores balanceadas:

- **Árvore 2-3-4**: Árvore de busca onde cada nó pode conter de 1 a 3 chaves e ter de 2 a 4 filhos
- **Árvore Rubro-Negra**: Árvore binária de busca com propriedades de coloração que garantem balanceamento

## Estrutura do Projeto

```
projeto_arvores/
├── arvore_234.ipynb          # Implementação da Árvore 2-3-4
├── arvore_rubro_negra.ipynb  # Implementação da Árvore Rubro-Negra
└── README.md                 # Este arquivo
```

## Pré-requisitos

### Software Necessário
- Python 3.7 ou superior
- Jupyter Notebook ou Jupyter Lab
- Graphviz (software de renderização de grafos)

### Bibliotecas Python
```bash
pip install graphviz
pip install ipython
```

### Instalação do Graphviz
- **Windows**: Baixar e instalar de https://graphviz.org/download/
- **macOS**: `brew install graphviz`
- **Ubuntu/Debian**: `sudo apt-get install graphviz`

## Instruções de Execução

### 1. Configuração do Ambiente

1. Clone ou baixe este projeto
2. Navegue até o diretório do projeto
3. Instale as dependências necessárias
4. Inicie o Jupyter Notebook:
```bash
jupyter notebook
```

### 2. Executando a Árvore 2-3-4

1. Abra o arquivo `arvore_234.ipynb`
2. Execute as células na ordem:
   - **Célula 1**: Importações das bibliotecas
   - **Célula 2**: Classes Node234 e Arvore234 com implementação completa
   - **Célula 3**: Demonstração interativa com visualização passo a passo

### 3. Executando a Árvore Rubro-Negra

1. Abra o arquivo `arvore_rubro_negra.ipynb`
2. Execute as células na ordem:
   - **Célula 1**: Importações das bibliotecas
   - **Célula 2**: Classes RBNode e ArvoreRubroNegra com implementação completa
   - **Célula 3**: Demonstração interativa com visualização passo a passo

## Funcionalidades Implementadas

### Árvore 2-3-4
- **Inserção**: Inserção com divisão automática de nós cheios
- **Busca**: Busca iterativa eficiente
- **Remoção**: Remoção com ajuste da estrutura
- **Balanceamento**: Automático através de divisões
- **Visualização**: Gráficos dos nós com múltiplas chaves

### Árvore Rubro-Negra
- **Inserção**: Inserção com rebalanceamento por rotações e recoloração
- **Busca**: Busca recursiva/iterativa
- **Remoção**: Remoção com correção das propriedades rubro-negra
- **Balanceamento**: Rotações e mudanças de cor
- **Visualização**: Nós coloridos (vermelho/preto)

## Saída Esperada

Ambos os notebooks produzem:
1. **Animação passo a passo** da construção da árvore
2. **Visualizações gráficas** em cada etapa
3. **Estatísticas** (altura, número de nós)
4. **Demonstrações** de busca e remoção
5. **Arquivos PNG** das visualizações geradas

## Detalhes Técnicos

### Complexidade das Operações
- **Busca**: O(log n)
- **Inserção**: O(log n)
- **Remoção**: O(log n)
- **Altura**: Balanceada automaticamente

### Propriedades da Árvore 2-3-4
- Cada nó tem 1, 2 ou 3 chaves
- Nó com k chaves tem k+1 filhos
- Todas as folhas no mesmo nível
- Chaves ordenadas em cada nó

### Propriedades da Árvore Rubro-Negra
- Todo nó é vermelho ou preto
- Raiz é sempre preta
- Folhas (NIL) são pretas
- Nós vermelhos têm filhos pretos
- Caminhos da raiz às folhas têm mesmo número de nós pretos

## Solução de Problemas

### Erro de Renderização Graphviz
- Verifique se o Graphviz está instalado no sistema
- Confirme se está no PATH do sistema
- Reinicie o kernel do Jupyter após a instalação

### Visualizações Não Aparecem
- Execute todas as células em ordem
- Verifique se as imagens estão sendo geradas no diretório
- Limpe o output e execute novamente

### Performance
- Para árvores muito grandes, ajuste o `time.sleep()` para acelerar a animação
- Reduza o número de valores para demonstrações mais rápidas

## Estrutura dos Comentários

O código está comentado para fins de aprendizado:
- **Comentários de função**: Explicam o propósito de cada método
- **Comentários de algoritmo**: Detalham passos importantes
- **Comentários de casos**: Explicam diferentes cenários tratados
- **Comentários de complexidade**: Indicam características de performance
