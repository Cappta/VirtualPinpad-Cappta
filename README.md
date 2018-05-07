# Virtual PinPad - Cappta

<p align="center">
  <img height="129" width="324" src="https://raw.githubusercontent.com/Cappta/PinPad-Virtual/master/imgs/logo-cappta.png?token=AXf_iyS--vol01oUbFNktm9rcWFdS7m3ks5a9bvQwA%3D%3D">
</p>

###Emulador de PinPad para integração com a Cappta.

## Configuração

Para configurar o Virtual Pinpad – Cappta, é preciso seguir os seguintes passos:

*	Instale o VSPE, software que veio zipado na pasta Virutal Pinpad – Cappta;

* Agora, edite o arquivo “VirtualPinpad.exe.config” que se encontra na pasta “VirtualPinpad – Cappta”. Para isso, clique com o lado direito do mouse sobre o arquivo e clique em “Editar” ou clique em “Abrir com > Bloco de notas”;

* Na key “COM”, edite o valor para o número da porta com que foi configurada previamente.

```
<add key="COM" value="20"/>
```

* Depois edite a key "Scripts" para o local de onde se encontra a sua pasta Scripts. A pasta scripts se encontra originalmente dentro da pasta “VirutalPinpad – Cappta”.

```
<add key="Scripts" value="C: \VirtualPinpad - Cappta\Scripts"/>
```

* Repita esse processo, porém agora para a key “CLI”, apontando para o endereço da pasta CLI, que também se encontra originalmente dentro da pasta “VirutalPinpad – Cappta”.

```
<add key="Scripts" value="C: \VirtualPinpad - Cappta\CLI"/>
```

*	Agora configure a key “VSPE” para o local de instalação do software VSPE instalado anteriormente.

```
<add key="VSPE" value="C:\Program Files (x86)\Eterlogic.com\Virtual Serial Ports Emulator"/>
```

*	Pronto, agora salve o arquivo, vale lembrar que se você colocar a pasta “VirtutalPinpad – Cappta” dentro de alguma pasta que necessite permissão de Administrador para acessar, o software “VirtualPinpad – Cappta” precisará ser executado como administrador.

## Executando o VirtualPinpad - Cappta

Após configurado, ao executar o software VirtualPinpad, seu VSPE será configurado automaticamente.

### :warning: Este passo demora alguns segundos e é recomendado que não use o computador até que apareça a seguinte janela: 

<p align="center">
  <img src="https://github.com/Cappta/PinPad-Virtual/blob/master/imgs/virtualpinpad.jpg?raw=true">
</p>

## Utilizando o VirtualPinpad - Cappta

Para utilizar o VirtualPinpad, basta selecionar um script: 

<p align="center">
  <img src="https://github.com/Cappta/PinPad-Virtual/blob/master/imgs/select-script.jpg?raw=true">
</p>

### Scripts
Temos 5 Scripts padrões:

* Digitado: Script para efetuar uma venda digitada na modalidade crédito;

* Master-BotaoVermelho: Script para simular a ação do PinPad de cancelar a venda na tela de “Digite a senha” em qualquer modalidade (Pressionar o botão vermelho do PinPad). Este script utiliza um cartão com a bandeira “MasterCard”.

* Master-Padrao: Script utilizado para aprovar uma venda em qualquer modalidade. (Crédito e Débito). Este script utiliza um cartão com a bandeira “MasterCard”.

* Visa-BotaoVermelho: Script para simular a ação do PinPad de cancelar a venda na tela de “Digite a senha” em qualquer modalidade (Pressionar o botão vermelho do PinPad). Este script utiliza um cartão com a bandeira “Visa”.

* Visa-Padrao: Script utilizado para aprovar uma venda em qualquer modalidade. (Crédito e Débito). Este script utiliza um cartão com a bandeira “Visa”.

### Visibilidade

Agora, temos a opção de PinPad Visível ou invisível. Essa opção é responsável por decidir se a janela do PinPad apareça no fundo da aplicação:

<p align="center">
  <img src="https://github.com/Cappta/PinPad-Virtual/blob/master/imgs/virtualpinpad-visible.jpg?raw=true">
</p>

Está e a janela que se abrirá caso seja selecionada a opção “Visível”:

<p align="center">
  <img src="https://github.com/Cappta/PinPad-Virtual/blob/master/imgs/pinpad-cli.jpg?raw=true">
</p>

### :heavy_check_mark: Agora é só clicar em “Executar” e pronto, seu VirtualPinpad está configurado e você está pronto para utilizar o nosso CapptaGpPlus.
