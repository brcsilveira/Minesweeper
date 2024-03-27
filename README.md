# Minesweeper em Elixir

Este é um projeto simples do jogo Minesweeper implementado em Elixir. O jogo é jogado em um tabuleiro de tamanho N x N, onde os jogadores devem abrir todas as células sem abrir uma única mina.

## Funcionalidades

### 1. Manipulação de Matrizes

- `get_arr/2`: Retorna o elemento em uma posição específica de um vetor.
- `update_arr/3`: Atualiza o valor em uma posição específica de um vetor.
- `get_pos/3`: Retorna o valor em uma posição específica de uma matriz.
- `update_pos/4`: Atualiza o valor em uma posição específica de uma matriz.

### 2. Lógica do Jogo

- `is_mine/3`: Verifica se uma posição em um tabuleiro contém uma mina.
- `is_valid_pos/3`: Verifica se uma posição é válida no tabuleiro.
- `valid_moves/3`: Retorna uma lista de posições adjacentes válidas.
- `conta_minas_adj/3`: Conta o número de minas adjacentes a uma posição específica.
- `abre_jogada/4`: Função principal do jogo para abrir uma posição e suas adjacências.
- `abre_posicao/4`: Verifica e abre uma posição no tabuleiro.
- `abre_tabuleiro/2`: Abre todo o tabuleiro após a conclusão do jogo.
- `board_to_string/1`: Converte o tabuleiro para uma representação em string para exibição.
- `gera_lista/2`: Gera uma lista contendo N vezes um valor específico.
- `gera_tabuleiro/1`: Gera um novo tabuleiro todo fechado.
- `gera_mapa_de_minas/1`: Gera um novo mapa de minas todo falso.
- `conta_fechadas/1`: Conta as posições fechadas no tabuleiro.
- `conta_minas/1`: Conta o número de minas no tabuleiro.
- `end_game?/2`: Verifica se o jogo acabou.

## Como Jogar

Para jogar, siga os passos abaixo:

1. Clone o repositório:

   ```
   git clone https://github.com/brcsilveira/minesweeper-elixir.git
   ```

2. Navegue até o diretório do projeto:

   ```
   cd minesweeper-elixir
   ```

3. Execute o jogo:

   ```
   iex -S mix
   ```

4. Siga as instruções na tela para jogar.

## Motor do Jogo

O motor do jogo pode ser executado descomentando as linhas no final do módulo `Minesweeper`:

```elixir
# defmodule Motor do
#   ...
# end
#
# Motor.main()
```

## Autor

Bruno Chim Silveira

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter mais detalhes.
