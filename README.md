# Trabalho-Integrado
Aqui você irá ver um projeto integrado :D
## Integrantes:

João Pedro Silva Otoni
Ikaro Massafera Barros Amaral

Professores: Ana Leticia G. Gonçalves - José Andery Carneiro

## Sobre o projeto
Sistema embarcado interativo para controle de aulas em laboratório, desenvolvido com microcontrolador STM32F103 e display ST7789 via SPI. O professor opera o sistema por meio de 4 botões (PA9, PA10, PA11, PA12) e recebe feedback visual em tempo real no display.

## Funcionalidades

O sistema gera uma senha numérica aleatória de 4 dígitos (valores de 1 a 4) ao iniciar
O professor insere a senha usando os 4 botões
Senha errada: tela vermelha, nova senha gerada e tentativa reiniciada

## Configuração da turma

O professor define o número máximo de alunos antes de iniciar a aula
PA9 subtrai 1 - PA10 subtrai 5 - PA11 adiciona 1 - PA12 adiciona 5
PA11 + PA12 juntos confirmam o valor

## Menu principal (execução da aula)
Botão Ação

PA9 Registrar entrada de aluno
PA10 Registrar saída para banheiro/água
PA11 Registrar retorno do aluno
PA9 + PA10 Encerrar a aula

## Regras respeitadas

Não é possível registrar entrada acima do limite da turma
Máximo de 3 alunos fora da sala simultaneamente
Não é possível registrar saída se não houver alunos presentes

## Encerramento e relatório
Ao pressionar PA9 + PA10 simultaneamente, o sistema exibe:

Total de alunos da turma
Alunos presentes ao encerrar
Alunos ainda no banheiro
Total de saídas realizadas durante a aula
