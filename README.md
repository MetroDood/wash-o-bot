# **Wash-o-bot:** Aplicação do robô

Trabalho de Interação Humano-Robô (IHR) apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interação Humano-Robô (IHR) (CCR230) do curso de Engenharia de Robôs, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](https://github.com/fagnerpimentel).

## Componentes do Grupo

- Henrique Luisi Fernandes Pinto 11.221.068-7
- Francisco Ribeiro Silva Lima   11.120.479-8 
- Igor Croce Holanda             11.221.001-8

## Resumo
Wash-o-Bot é um robô doméstico autônomo capaz de coletar roupas, separá-las por tipo e cor, realizar o processo completo de lavagem e secagem, e organizar as peças ao final do ciclo.

## Introdução

A rotina doméstica demanda tempo e organização, sendo a lavagem de roupas uma tarefa recorrente e muitas vezes negligenciada por aqueles que possuem rotinas corridas. O Wash-o-Bot foi projetado para automatizar completamente o processo de cuidado com roupas, desde a coleta até a finalização.

Objetivo do robô: Automatizar integralmente o processo de lavagem de roupas de forma eficiente, intuitiva e confiável.
O robô deve proporcionar uma experiência prática, confiável e simples, exigindo mínima intervenção do usuário.

## Publico Alvo

Usuários domésticos que buscam otimizar tempo e reduzir esforço em tarefas domésticas.

Adultos com rotina intensa de trabalho

Idosos

Pessoas com mobilidade reduzida

### Personas

### Persona Primária: Adulto com rotina intensa

Idade: 25–45 anos

Trabalha em período integral

Mora sozinho ou com família pequena

Valoriza praticidade e tecnologia

### Informações necessárias:

Frequência de lavagem

Preferências de lavagem (tons escuros, pesado, cores separadas)

Horários para operação

### Persona Secundária: Pessoas com Mobilidade Reduzida

Pode possuir limitações motoras permanentes ou temporárias

Necessita minimizar esforço físico

### Informações necessárias:

Nível de autonomia desejado

Configuração de comandos por voz ou aplicativo

Horários para operação

Preferência de lavagem

### Persona Terciária: Pessoa idosa

Idade: 60+

Pode ter limitações físicas

Busca autonomia dentro de casa

### Informações necessárias:

Sensibilidade a ruídos

Complexidade da interface

Preferências de lavagem (tons escuros, pesado, cores separadas)

Horários para operação

### Mapa de empatia - Persona Primaria - Adulto de Rotina Intensa

![Mapa de empatia Primaria](empatia_primaria.png)

### Mapa de empatia - Persona Secundaria - Idosos

![Mapa de empatia Secundaria](empatia_secundaria.png)

## Contexto de uso

O Wash-o-Bot opera em ambientes domésticos, como casas e apartamentos, principalmente em quartos, banheiros e áreas de lavanderia.
O robô interage com o usuário durante tarefas rotineiras do dia a dia, em um ambiente onde roupas podem estar espalhadas ou acumuladas em cestos.

### Contexto social, econômico e cultural

Rotinas cada vez mais ocupadas, com pouco tempo para tarefas domésticas.
Crescente adoção de tecnologias de automação residencial.
Interesse por soluções que aumentem conforto e produtividade em casa.


### Informações que o robô precisa saber sobre o ambiente
- Localização da lavanderia ou máquina de lavar.
- Áreas da casa onde roupas podem estar (quarto, banheiro, cesto).
- Obstáculos no ambiente (móveis, escadas, objetos no chão).
- Tipos de superfície para navegação (piso, tapete).

## Jornada do usuário

Depois de um dia corrido, ao chegar em casa, o usuário percebe que há roupas acumuladas no quarto ou na lavanderia. Para evitar realizar a tarefa manualmente, ele ativa o Wash-o-Bot por comando de voz ou aplicativo no celular, solicitando o início da lavagem. O robô confirma o comando por meio de um sinal (sonoro ou visual).
Em seguida, o Wash-o-Bot se desloca pela casa utilizando seus sensores para localizar e coletar roupas no chão ou em cestos. Durante esse processo, o robô separa as peças de acordo com características como cor ou tipo de tecido. Depois de coletar as roupas, ele se dirige à lavanderia e inicia automaticamente o ciclo de lavagem. Após a lavagem, o robô realiza a secagem das roupas e organiza as peças em um local previamente definido pelo usuário. Ao final do processo, o Wash-o-Bot envia uma notificação informando que a tarefa foi concluída, encerrando a interação com o usuário.

# Análise de concorrência

## Samsung Bot Handy

### Pontos positivos

- Capacidade de manipular objetos domésticos.
  
- Uso de visão computacional.
  
- Integração com casa inteligente.
  
- Braço robótico com seis graus de liberdade

### Pontos negativos

- Ainda em desenvolvimento.

- Alto custo esperado.

## FoldiMate - Fora do Mercado em 2021

### Pontos positivos
- Automatiza a etapa de dobrar roupas.

- Reduz o tempo gasto após a lavagem.

### Pontos negativos

- Não coleta nem lava roupas.

- Muito manual em comparação ao Wash-o-Bot.

- Retirado do mercado por baixa lucratividade

## Laundroid - Seven Dreamers - Fora do Mercado em 2021

### Pontos positivos

- Uso de inteligência artificial para reconhecer roupas.

- Automatiza a organização das peças.

## Pontos negativos

- Equipamento grande e caro.

- Não realiza coleta ou lavagem completa.

- Requer manuseio humano

## Comparação com o Wash-o-Bot

Existem soluções que automatizam partes do processo de lavanderia, mas poucas realizam todo o fluxo de forma autônoma. O Wash-o-Bot se diferencia por integrar:

- coleta de roupas

- separação automática

- lavagem

- secagem

- organização final

## Design

O Wash-o-Bot foi projetado para possuir affordances claras, permitindo que o usuário compreenda facilmente como interagir com o robô. Entre essas características estão comandos simples por voz ou aplicativo, indicadores luminosos para mostrar o estado da tarefa e compartimentos de fácil acesso para manipulação de roupas, além do braço com seis graus de liberdade.

Em relação à acessibilidade, o robô deve considerar usuários com diferentes necessidades, incluindo pessoas idosas ou com mobilidade reduzida. Para isso, o sistema deve possuir interface simples, comandos intuitivos, feedback visual ou sonoro, além de minimizar a necessidade de esforço físico.

O Wash-o-Bot possui baixo nível de características antropomórficas, focando mais em funcionalidade do que em aparência humana, com a única característica similar sendo o braço.

Esse padrão tende a ser mais aceito em robôs domésticos voltados para tarefas utilitárias, pois transmite eficiência e evita expectativas irreais sobre comportamento humanoide.

<!-- ![Washobot](washobot.jpg) -->
<img alt="Washobot" src="washobot.jpg" height="300"/>

## Ações do robô

- Para cada ação:
  - Descreva a ação.
  - Determine os pré-requisitos para que a ação aconteça
  - Determine o que se espera que seja modificado no ambiente quando a ação é finalizada

## Interações do robô

### Espacial

- Para cada interação:
  - Descreva a interação.
  - Determine os pré-requisitos para que a interação aconteça
  - Determine espera de resposta emocional do usúario quando a interação é finalizada

### Verbal

- Para cada interação:
  - Descreva a interação.
  - Determine os pré-requisitos para que a interação aconteça
  - Determine espera de resposta emocional do usúario quando a interação é finalizada

### Não-verbal

- Para cada interação:
  - Descreva a interação.
  - Determine os pré-requisitos para que a interação aconteça
  - Determine espera de resposta emocional do usúario quando a interação é finalizada

[^1]: Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>

<!-- TODOs:
- Add exemplos
 -->
