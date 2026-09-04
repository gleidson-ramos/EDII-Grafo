# 🌐 Grafo — Rede Social
O projeto simula uma rede social, na qual cada usuário é representado como uma ``vértice`` do ``grafo`` e cada amizade entre dois usuários é representada como uma ``aresta``.

Além do gerenciamento dos usuários e amizades, a aplicação utiliza algoritmos da **biblioteca NetworkX** para realizar consultas e análises sobre a rede.

Os dados dos usuários são persistidos em um arquivo CSV, permitindo que a rede social seja carregada novamente quando o programa for executado.

## 🎯 Objetivos
- Utilizar grafos para representar relacionamentos.
- Implementar operações de inserção e consulta.
- Trabalhar com grafos não direcionados.
- Analisar o grau de conexão dos usuários.
- Encontrar caminhos entre pessoas.
- Visualizar graficamente uma rede social.
- Praticar persistência de dados utilizando arquivos CSV.

## 🧠 Estrutura do Grafo
O projeto utiliza um grafo não direcionado, criado através de ``networkx.Graph()``. A representação pode ser entendida da seguinte maneira:
```bash
            Shuri
           /     \
        T'Challa  Peter
          /         \
       Natasha ---- Tony
```

- **Vértices (nós):** representam os usuários.
- **Arestas:** representam amizades.
- **Grau do vértice:** representa a quantidade de relacionamentos de uma pessoa.
- **Caminho:** representa uma sequência de relacionamentos entre duas pessoas.

Como as amizades são consideradas recíprocas, quando ``user1`` adiciona ``user2``, uma conexão é criada nos dois sentidos.

## 🛠️ Tecnologias utilizadas
- Python
- NetworkX: criação e análise de grafos.
- Matplotlib: visualização gráfica da rede.
- CSV: armazenamento e recuperação dos dados.


## ⚙️ Funcionalidades
A aplicação possui um menu interativo com as seguintes opções:

|  | Opção | Funcionalidade |
|---|---| --- |
|1	|Criar Perfil| Permite cadastrar um novo usuário |
|2	|Adicionar Amigos| Estabelece amizade entre dois usuários cadastrados.|
|3	|Exibir Rede Social| Cria e exibe graficamente o grafo utilizando NetworkX e Matplotlib. |
|4	|Buscar Pessoa| Permite pesquisar um usuário pelo nome. |
|5	|Pessoa(s) com Mais Relacionamentos| Utiliza o grau dos vértices para identificar as pessoas que possuem a maior quantidade de amigos. |
|6	|Pessoa(s) com Menos Relacionamentos| Realiza o processo inverso da funcionalidade anterior, identificando os usuários com a menor quantidade de conexões. |
|7	|Consultar Relacionamento| Permite verificar se duas pessoas possuem uma amizade direta , caso não exista uma ligação direta, o programa procura um caminho entre os dois usuários. |
|8	|Consultar por País| Permite consultar usuários pertencentes a determinado país. |
|9	|Salvar e Sair| Antes de encerrar o programa, os dados são armazenados no arquivo csv |





## 📈 Conceitos de Estrutura de Dados aplicados
- Grafos
- Vértices
- Arestas
- Grau de vértices
- Adjacência
- Caminhos
- Subgrafos
- Centralidade de grau
- Busca de menor caminho
- Representação de relacionamentos

## 📄 Sobre o Projeto
Projeto desenvolvido para a disciplina de Estrutura de Dados II (EDII), utilizando a estrutura de dados Grafo para representar uma rede social.

A aplicação permite cadastrar usuários, estabelecer amizades entre eles, consultar relacionamentos e visualizar graficamente a rede social.