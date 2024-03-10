<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/87d332d0-5198-4a2f-b159-38c8c2976954.png"></a>
    <span> Trabalhando com Machine Learning</span>
</h1>

## Criando modelo de previsão - Passo a passo

Para começar a trabalhar com aprendizado de máquina, é fundamental ter um espaço de trabalho dedicado. Esta é a primeira etapa: criar o seu próprio espaço de trabalho, o qual será o ponto de partida para automatizar suas tarefas.

Uma vez que o seu espaço de trabalho estiver configurado, o próximo passo é acessar o ML Studio para iniciar a criação de um "novo projeto de aprendizado de máquina automatizado". Siga cuidadosamente os passos descritos na documentação do Learning para garantir um melhor entendimento e o sucesso da sua empreitada.
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/01.png" width=""/> 

...

## Vamos criar um aprendizado de maquina para a previsão de aluguel de bicicletas:
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/02.png" width=""/> 

O tipo de tarefa é regressão e o nome de ativo de dados e aluguel de bicicletas, com fonte de dados da WEB.
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/03.png" width=""/> 

<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/04.png" width=""/> 

<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/05.png" width=""/> 

...

A documentação do Learning é bem didática e traz todos os valores e configurações para que o trabalho automatizado seja criado:
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/07.png" width=""/> 
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/08.png" width=""/> 
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/09.png" width=""/> 
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/10.png" width=""/> 
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/11.png" width=""/> 
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/12.png" width=""/> 
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/13.png" width=""/> 

...

Chegando na opção "examinar" basta enviar o seu trabalho de treinamento:
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/14.png" width=""/> 

...

Após envio do seu trabalho irá passar pelo proxesso de configuração das execuções e após 15 minutos, podendo o tempo ser menor, estará concluído:
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/15.png" width=""/> 

<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/16.png" width=""/> 

...

Pipeline com as etapas do processo de aprendizado e os testes realizados:
<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/17.png" width=""/> 

## Teste do modelo

Na página do modelo, clique na aba "Pontos de extremidade". Também é possível acessar pelo menu lateral em "Pontos de extremidade". Clique no ponto correspondente ao modelo gerado. Em seguida, acesse a aba "Testar".

Para o teste, utilizei o json abaixo:

``` JASON
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
```

A previsão gerada foi: 376.20.

<img align="right" src="https://github.com/vinicioscarvalho1/DP01---Trabalhando-com-Machine-Learning-Na-Pr-tica/blob/main/images/18.PNG" width=""/> 
