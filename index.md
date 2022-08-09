# Segurança em Dispositivos iOS 

<p align="center">
	
<img align="center" src="https://cdn-images-1.medium.com/max/640/1*8IBTekrtpUvI6my1IFP1GA.gif"/>

</p>

Quando falamos sobre a Arquitetura de Segurança de dispositivos iOS, podemos mencionar sete ferramentas que auxiliam na proteção dos mesmos. 

## Assinatura de Código

O primeiro dos métodos que vamos ver é o de Code Signing utilizado pela Apple, ele permite fazer uma **validação da autenticidade das aplicações** de terceiros, o que faz com que sejam liberadas apenas as aplicações provenientes da App Store e, também, que o **Kernel permita a execução apenas de aplicações assinadas**. 

Podemos ver um exemplo disso quando realizamos Jailbreak em um dispositivo. A única forma de rodar um app modificado sem passar por todo o processo que inclui a assinatura, é instalando em um dispositivo jailbroke. De forma convencional e sem esse "root", a única forma de testar um aplicativo é em simuladores como o Test Flight. 

## Segregação de Privilégios 

Um outro ponto bem interessante e importante para a segurança no geral, é a segregação de privilégios ou seja, a gestão de privilégios e acessos. **Definir os privilégios que são necessários de acordo com cada role, e evitar que serviços tenham acessos mais altos**, como admin, sem necessidade.Dessa forma, deixando somente serviços mais importantes como ROOT.
O sistema separa utilizando usuários, grupos, e outros mecanismos de permissão de arquivos do próprio UNIX.

Como exemplo, várias aplicações onde o usuário tem acesso direto, como browser, serviços de e-mail e similares, rodam com o usuário MOBILE. 
Nesse caso, para o atacante escalar o acesso precisaria de uma outra aplicação que possua o usuário ROOT.

## Menor Superfície de Ataque

Um dos principais pontos que sempre é discutido quando falamos de Apple, é o seu sistema mais "fechado". Com isso, podemos ja deduzir que, de certa forma, o seu ambiente também possui uma **menor superfície de ataque**.

O iOS não executa determinados tipos de arquivos, mas o MacOS X sim. Um exemplo disso são os arquivos .psd. Eles são executáveis comumente no Safari mas não no Safari Mobile, e isso acontece com uma série de arquivos e raramente notamos algo assim.




### Outros materiais:  


[![android1](https://user-images.githubusercontent.com/37185061/175828137-0d7e48f0-77a0-4ef3-85ff-28f1fe722adc.png)](https://github.com/wh0isdxk/AndroidRevEngineering)[![developsec1](https://user-images.githubusercontent.com/37185061/175828232-6dda3fd1-e9ee-4ea3-b862-5f335b335695.png)](https://github.com/wh0isdxk/DesenvolvimentoSeguro)[![nutshell1](https://user-images.githubusercontent.com/37185061/175828140-4505c986-191b-4c92-9f51-0345837e2ceb.png)](https://github.com/wh0isdxk/InfosecInANutshell)





<p align="center">

<a href="https://www.buymeacoffee.com/wh0isdxk"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=wh0isdxk&button_colour=FF5F5F&font_colour=ffffff&font_family=Poppins&outline_colour=000000&coffee_colour=FFDD00"></a>

</p>
