- [Pipe](#pipe)
    - [Tarefas para casa](#tarefas-para-casa)
    - [Desafio](#desafio)
# Pipe
Nesta aula, vamos ver o conceito do caracter pipe (|). 
No linux, o pipe tem uma função importante: Direcionar a saída de um comando para a entrada do comando seguinte. Este comando simplificou muito a integração entre comandos/programas. Dessa forma podemos encadear comandos, sem aumentar muito a complexidade do código.

Veja, por exemplo, o comando abaixo:
```bash
cat arquivo.txt | grep "Busca" | cut -d',' -f2
```
Primeiramente o shell irá realizar o comando cat do arquivo.txt. Em seguida, o que seria mostrado na tela (conteúdo do arquivo) é passado para o comando grep, que filtra apenas as linhas que possuem o texto "Busca". em seguida, apenas estas linhas são direcionadas para o comando cut, que corta as linhas onde há vírgulas e seleciona apenas o segundo campo para mostrar na tela.

Para testarmos, baixe o arquivo lorem.txt e teste a execução de alguns comandos encadeados.

Ex:
```bash
cat lorem.txt | grep "Lorem" | cut -d',' -f2
```
Altere o comando e veja as diferenças nos resultados.

## Tarefas para casa
Nenhuma.

## Desafio
Nenhum.