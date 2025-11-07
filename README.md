# AGENTE IA

==============================
PROGRAMA NECESSÁRIO PARA CONEXÃO SSH

https://bitvise.com/ssh-client-download
==============================
[PAINEL BASE]
EASYPANEL - https://easypanel.io/

[INSTALADOR]
curl -sSL https://get.easypanel.io | sh

REPOSITÓRIOS:

[EVOLUTION-API]
https://github.com/EvolutionAPI/evolution-api

[N8N]
https://github.com/n8n-io/n8n
==============================
CREDENCIAL GEMINI

==============================

PASSO 1

Primeiro, ATUALIZE SUA VPS
COMANDO

apt update && apt upgrade -y && sudo apt dist-upgrade -y

CASO A VPS PEÇA, CONFIRME SEMPRE COM y

verifique sua versão do Linux
COMANDO:

lsb_release -a

PASSO 2 - ATUALIZAR A VPS
SE SUA VPS FOR UBUNTU 22 OU POSTERIOR, PULE ESTA ETAPA(CONTINUE NA ETAPA 3)
SE SUA VPS FOR UBUNTU 20.04 OU ANTERIOR FAÇA OS COMANDOS ABAIXO UM POR VEZ

apt update
apt upgrade -y
sudo apt dist-upgrade -y
sudo apt autoremove -y

shutdown -r now

apt install update-manager-core -y
do-release-upgrade


AGUARDE A VPS REINICIAR E CONECTE NOVAMENTE E SIGA PARA O PRÓXIMO PASSO


=========================================================================
PASSO 3 - INSTALAÇÃO EASYPANEL

PASSO INSTALE O EASYPANEL
COMANDO
  curl -sSL https://get.easypanel.io | sh

CONECTE NA SUA VPS PELO NAVEGADOR 

http://SEUIP:3000

crie uma conta no EASYPANEL
=========================================================================
PASSO 4 - CRIAÇÃO DO PROJETO

  CLIQUE EM CRIAR PROJETO

Nome do projeto deve ficar minúsculo.

CLIQUE EM MODELOS,E MODELOS NOVAMENTE

BUSQUE POR EVOLUTION(IRÁ APARECER EVOLUTION-API) CLIQUE NELE E CLIQUE NO BOTAO DO GITHUB PARA VER SE ESTÁ ATUALIZADA, 
    ALTERE O CÓDIGO NO EASYPANEL PARA FICAR COM A ULTIMA VERSÃO DA EVOLUTION API E CLIQUE EM CRIAR
	
	- AGUARDE A INSTALAÇÃO FINALIZAR
	- QUANDO FINALIZAR
	CRIE UMA KEY -  GERE UMA KEY NO SITE https://www.md5hashgenerator.com

	CLIQUE EM "PAINEL" - 
	CLIQUE EM "EVOLUTION API"
	CLIQUE EM "AMBIENTE"  NA LINHA 160 - COLOQUE A KEY QUE GEROU
	CLIQUE EM IMPLANTAR
	- AGUARDE A FINALIZAÇÃO

BUSQUE POR N8N (IRÁ APARECER N8N) CLIQUE NELE E CLIQUE NO BOTAO DO GITHUB PARA VER SE ESTÁ ATUALIZADO,
    ALTERE O CÓDIGO NO EASYPANEL PARA FICAR COM A ULTIMA VERSÃO DO N8N E CLIQUE EM CRIAR

- AGUARDE A INSTALAÇÃO FINALIZAR

QUANDO FINALIZAR, CLIQUE NO ÍCONE DE ABRIR E CRIE UMA CONTA NO N8N E SOLICITE UMA LICENÇA CONFORME VIDEO

=========================================================================

SISTEMAS INSTALADOS E PRONTOS PARA CRIAR AS INSTANCIAS E CONECTAR SEUS AGENTES

INTEGRAÇÃO EVOLUTION COM N8N
n8n-nodes-evolution-api



