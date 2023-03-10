# Consulta de Localidades de UF
## Desafio da Neoway
 
### Algumas Observações Durante a Construção do Código:
* Conhecia tanto Selenium e BeautifulSoup, porém nunca havia trabalhado a fundo com ambos.
  * Então eu basicamente fiquei da hora que recebi o desafio 09:00 da manhã 25/01 às 21:06 25/01 estudando e tentando resolver.
  * Então foi um desafio muito interessante, consegui desenvolver com bastante esforço um código legal acredito eu.
  * Aprendi bastante, tive que aprender a utilizar as bibliotecas, lendo a documentação, vídeos.
* Tenho muito a aprender e a me desenvolver e isso é algo que eu gosto muito de fazer.
* Com certeza tem maneiras melhores de resolver o desafio, mas no momento, da forma que eu fiz, resolveu.

## Vamos ao Desafio:

> Eu tentei realizar de algumas formas o desafio, em todas elas eu via que me levava a utilizar Selenium e BeautifulSoup,
>tentei realizar primeiro somente com Selenium, então fui atrás da documentação e vídeos, mas me deparava sempre com algum problema, para encontrar os elementos HTML, posteriormente fui tentar com o BeatifulSoup, encontrei problemas diferentes, já na manipução da página, identificar quantidade de páginas etc...
>Então vi que conseguia integrar as duas bibliotecas, foi onde aos poucos fui conseguindo realizar os passos para acessar toda a informação referente a cada UF.

>Para resolver, por exemplo, a questão do webdriver, no caso do chrome, ao invés de ter que baixar o driver localmente, deixei de forma dinâmica, para não ter que ficar fazendo manualmente, visto que já tenho um ambiente só para isso, fica mais fácil, pois então é rodar o código, que já identifica a versão do navegador utilizado. A solução para esta situação foi utilizando as seguintes bibliotecas:
```py
from webdriver_manager.chrome import ChromeDriverManager
from selenium.webdriver.chrome.service import Service

servico = Service(ChromeDriverManager().install())
driver = webdriver.Chrome(service=servico)
```

## Rodar o Código

* Informações Importantes, é necessário ter o Anaconda Instalado na Máquina.

1. Realize o clone do Repositório, podendo usar o comando do git cli no terminal:
```sh
gh repo clone cordeiro-dados/Neoway
```
* Ou baixando o Zip do Repositório.
  * Que para este caso, se encontra na Branch neoway

## Configurar o Environment
* Ao abrir a Pasta ou Repositório na máquina, abrindo o terminal, execute o seguinte comando:
```sh
conda env create -f env.yml
```
>Esse comando faz com que baixa o Environment criado para o projeto, em seguida execute um dos dos códigos informados em seguida.

* Para executar o código, primeiramente deve-se acessar o terminal dentro da pasta onde clonou e executar o seguinte comando:
```sh
conda activate ufs-env
```
* Caso não funcione, o seguinte código também dá:
```sh
source activate ufs-env
```
* Verifique no terminal se está no Ambiente (ufs-env).
* Verifique também se o Interpreter está o ufs-env: </br>
![Screenshot](img.png)
* Após, execute então o arquivo Python:
```sh
python data.py
```
