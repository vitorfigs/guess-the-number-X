# Projeto: Guess The Number XTREME
**Data:** 10/08/2026  
**Disciplina:** Circuitos Digitais | **UFCA** - Universidade Federal do Cariri | **Professor:** Ramon Nepomuceno |

## Sobre o projeto
Jogo interativo desenvolvido no **Logisim** onde dois jogadores competem para adivinhar um ponto no espaço (coordenadas x e y), representadas por números de 4 bits aleatórios. O sistema retorna um feedback sobre a precisão dos palpites através de um sistema de "temperatura" (LEDs RGB: azul para frio, vermelho para quente) e indicação de acertos parciais ou totais. Ganha o jogador que acertar 15 coordenadas primeiro ou, caso nenhum jogador tenha atingido esse objetivo, aquele que tiver acumulado mais pontos quando ambos os tempos dos jogadores se esgotarem.
 
---
## Visão Geral
<details>
  <summary><a href="#circuito-main">Clique para abrir a visão geral do circuito</a></summary>
  <br>
  <div align="center">
    <img src="./img/visao_geral.png" alt="Visão Geral do Sistema" width="65%">
  </div>
</details>

  ## 📅 Desenvolvimento
| Data | Atividade |
| :--- | :--- |
| 08/07/2026 | Definição das especificações e estrutura do projeto |
| 11/08 ~ 16/08 | Implementação do módulo dos Cronômetros |
| --/-- | Implementação do circuito CORE |
| --/-- | Implementação do circuito GTN X e subcircuitos auxiliares |
| --/--/-- | Finalização do projeto e documentação |


## * Circuitos principais:

### I. Cronômetros

* **Objetivo:** Realizar a contagem regressiva no turno do jogador.
   
* **Componentes:**
  * `4` Contadores de tempo.
  * `4` Multiplexadores (MUX).

* **Entradas (8 pinos):**
  * `Clk`: Sinal de clock do sistema.
  * `C jogando`: Pausa/ativa o cronômetro do jogador ativo (A ou B).
  * `s0` / `s1`: Ajustes de unidades (`s0`) e dezenas (`s1`) dos **segundos**.
  * `m0` / `m1`: Ajustes de unidades (`m0`) e dezenas (`m1`) dos **minutos**.
  * `reset`: Zera o cronômetro.
  * `cfg`: Alterna entre os modos de **Exibição** e **Configuração**.

* **Desafios:**
  * Noção de como funciona o contador
  * Controle dos limites de contagem de minutos e segundos.
  * Lógica e a estruturação do circuito

<details>
  <summary><a href="#cronometros">Clique para abrir a imagem do Circuito Cronômetros</a></summary>
  <br>
  
  ![Circuito Cronômetros](./img/cronometros.svg)
</details>

<br>
<br>

### II. Circuito "CORE" (...)

### III. Circuito "GTN X" (...)
