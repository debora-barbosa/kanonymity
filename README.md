# Implementação de k-Anonymity para dados escolares

Este é um projeto que aplica a técnica de **k-Anonymity** em um DataSet fictício e aleatório de alunos, desenvolvido como parte do meu Trabalho de Conclusão de Curso da minha pós-graduação em Ciência de Dados.

## 🛠️ Tecnologias e Bibliotecas

- **Python**
- Jupyter Notebook (Anaconda)
- Pandas
- Faker
- Numpy
- Random

## 📊 Sobre o DataSet

É um DataSet aleatório com registro de 1000 alunos gerado automaticamente com as seguintes informações:
- Nome (identificador)
- Matrícula (identificador)
- Endereço (identificador)
- Idade (quase-identificador)
- Ano escolar (quase-identificador)
- Turma (quase-identificador)
- Médias (quase-identificadores)

## 🛡️ Anonimização
1. Remoção dos dados identificadores.
2. Generalização de quase-identificadores:
    * Idade: Segmentada em intervalos (14-16 e 17-19 anos).
    * Ano escolar: Generelizado para "Ensino Médio".
    * Turma: Ocultação com "*".
    * Médias: Agrupadas em intervalos (0-5 e 5-10).
  
### Resultados
   
E para finalizar o código, foi calculado o valor de k, a classe de equivalência. No exemplo usado k=6, ou seja, para cada estudante existem pelo menos 5 estudantes que possuem dados anonimizados iguais. 

### Observação

Pòr se tratar de um DataSet aleatório, a cada vez que o código for executado serão gerados dados diferentes e, por consequência, um valor de k diferente.
