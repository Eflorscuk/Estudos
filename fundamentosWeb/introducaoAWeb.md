# Introdução à Web

## Breve história
1950. Computador Eletrônico
1960. ARPANET - Departamento de Defesa Americano (primeira tentativa da Internet)
1970. TCP/IP - Robert E. Kahn & Vint Cerf
1980. WWW - Tim Bernes-Lee
1990. Internet chega ao Brasil

## A Internet

É uma grande rede de computador.

### Topologias
1. Centralizada, se o nó central deixa de funcionar, toda a rede para de funcionar.
2. Distribuída, rotas de um computador para outro, mesmo que parte da rede fique fora do ar. A Internet não existe um poder central.
3. Web (Teia), vários níveis de rede. Grandes Backbones que ultrapassam um continente para outro. Provedores.

## TCP/IP - Transmission Control Protocol / Internet Protocol
TCP. Orientado à Conexão e Confiável, em contrapartida tem UDP, que é contrário ao TCP, é um protocolo mais leve e é Orientado ao Melhor Esforço.

TCP é baseado em handshake, ou seja, tem que conversar entre as pontas.

IP. É o protocolo responsável para fazer o roteamento entre redes.

O TCP/IP é um software e é separado em layers:

Pilha TCP/IP
-> Aplicação: HTTP, FTP, SMTP..., Comunicação Processo-A-Processo, Número da Porta
-> Transporte: TCP (Confiável), UDP (Melhor esforço), comunicação Host-A-Host, Confiabilidade, Integridade
-> Internet: IP - Internet Protocol, Conexão entre redes, Transferência de Pacotes
-> Rede / Física: Ethernet, Wi-Fi, Endereço MAC, Física (Hardware) e Enlace (Software)

A dependência das camadas é a camada de cima usa a de baixo.

## Anatomia do IPv4
1. Classe A:
	182.168.100.230
	Um número separado em 4 partes de 0 até 255
	A primeira parte é a Rede e as três últimas partes para definir o Host
	Temos poucas redes muitas máquinas
	255.0.0.0 -> Máscara de subrede
	Ela tem o mesmo número do IP
	Todos marcado com bit 1 é para mapear a rede, todos marcados com 0 
	para mapear os computadores na rede
2. Classe B:
	Duas primeiras partes do endereço IP para mapear a rede e as outras duas 	para mapear o Host
	Pode ter o mesmo número IP do primeiro exemplo
	255.255.0.0 -> Máscara de subrede
	Todos marcados com bit 1 é para mapear a rede, todos marcados com 0para 	mapear os computadores na rede
3. Classe C:
	Mesmo IP
	3 primeiras partes mapeiam uma rede e a última a host
	limitado a 255 máquinas nesta rede
	255.255.255.0
	Todos marcados com bit 1 é para mapear a rede, todos marcados com 0 para	mapear os computadores na rede

## Conceito de Porta
É um processo. Para conectar um computador com o outro é necessário saber o IP do computador e o processo (a Porta)
