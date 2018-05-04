# Virtual PinPad - Cappta

<p align="center">
   <img src="https://github.com/Cappta/PinPad-Virtual/tree/master/imgs/logo-cappta.png"/>
</p>

//Descrição Legal

## Configuração

Para configurar o Virtual Pinpad – Cappta, é preciso seguir os seguintes passos:

*	Instale o VSPE, software que veio zipado na pasta Virutal Pinpad – Cappta;

* Após instalar, abra o VSPE e clique em “Create new device”;

<p align="center">
   <img src="https://github.com/Cappta/PinPad-Virtual/tree/master/imgs/new-comport.JPG"/>
</p>

* Clique em avançar;

<p align="center">
   <img src="https://github.com/Cappta/PinPad-Virtual/tree/master/imgs/select-comtype.JPG"/>
</p>

* Escolha uma porta COM para a criação da porta virtual. Dê preferência para um número alto para evitar conflitos com uma possível porta COM real criada anteriormente. Em seguida clique em concluir. 

<p align="center">
   <img src="https://github.com/Cappta/PinPad-Virtual/tree/master/imgs/select-comportnumber.jpg"/>
</p>

* Feito isso, verifique se sua porta COM se encontra neste estado:

<p align="center">
   <img src="https://github.com/Cappta/PinPad-Virtual/tree/master/imgs/verify-comport.jpg"/>
</p>

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

*	Pronto, agora salve o arquivo, vale lembrar que se você colocar a pasta “VirtutalPinpad – Cappta” dentro de alguma pasta que necessite permissão de Administrador para acessar, o software “VirtualPinpad – Cappta” precisará ser executado como administrador.
