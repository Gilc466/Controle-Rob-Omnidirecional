# Controle de Robô Omnidirecional com Três Rodas
![robocoppelia](https://github.com/user-attachments/assets/546f4a8f-7bef-4eb7-96cc-a3917f5342b2)

Este repositório contém o código para o controle cinemático de um robô omnidirecional de três rodas. O projeto foi desenvolvido como parte do meu Trabalho de Conclusão de Curso (TCC), focando na simulação em tempo real e controle do robô no CoppeliaSim, utilizando um controlador PID para o acompanhamento de trajetória.

## Funcionalidades
Implementa o controle cinemático de um robô omnidirecional de três rodas usando transformações matriciais.
Utiliza um controlador PID para seguir uma posição e orientação desejadas (x, y, theta).
Estabelece comunicação com o CoppeliaSim através da API remota para simulação em tempo real.
Inclui cálculos de cinemática inversa para controlar as velocidades das rodas.
Capaz de rastrear uma configuração de objetivo com feedback em tempo real sobre a posição e orientação do robô.

## Como Funciona
O algoritmo conecta-se ao CoppeliaSim via API remota e ajusta continuamente as velocidades das rodas para minimizar o erro entre as configurações atual e desejada. Os passos principais são:

Cinemática Direta: Calcula o movimento do robô com base nas velocidades das rodas.
Cinemática Inversa: Determina as velocidades das rodas necessárias para alcançar o movimento desejado (posição e orientação).
Controlador PID: Ajusta a velocidade do robô com base nos erros de posição e orientação.

## Configuração da Simulação
A simulação deve estar em execução no CoppeliaSim para que o script funcione corretamente.
O robô utilizado na simulação é nomeado como "robotino" e possui três rodas: wheel0_joint, wheel1_joint, e wheel2_joint.

## Requisitos
CoppeliaSim
Python 3.10.9

Como Executar
Certifique-se de que o CoppeliaSim esteja em execução e conectado via API remota.
Execute o script para controlar o robô em tempo real enquanto ele se move em direção à configuração de objetivo.


# Referências
MACHARET, D. G. dcc042-robotica-movel. 2024. Acesso em: 10 nov. 2023. Disponível
em: <https://github.com/verlab/dcc042-robotica-movel/blob/main/jupyter-notebooks/
aula09-controle-cinematico.ipynb>.
