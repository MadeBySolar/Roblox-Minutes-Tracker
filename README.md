# Roblox Minutes Tracker

Este é um script Lua para o Roblox projetado para rastrear o tempo de jogo dos jogadores em minutos. Ele utiliza o `DataStoreService` para salvar e carregar os dados de tempo de jogo de cada jogador.

## Como Funciona:

-   **Entrada de Jogador:** Quando um jogador entra no jogo, o script cria um valor (`IntValue`) chamado "Minutos" dentro de uma pasta `leaderstats`, tornando-o visível na tabela de líderes.
-   **Carregamento de Dados:** Ele verifica se o jogador já tem dados salvos. Se sim, carrega o valor. Caso contrário, o contador começa em 0.
-   **Contagem de Tempo:** Uma rotina é iniciada para atualizar o valor de "Minutos" a cada 60 segundos (1 minuto).
-   **Saída de Jogador:** Quando o jogador sai do jogo, o script salva o valor atual de "Minutos" no `DataStore` usando o `UserId` do jogador como chave.
