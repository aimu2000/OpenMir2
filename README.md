[English](https://github.com/dwbeta/OpenMir2/blob/master/README.md)  | [中文](https://github.com/dwbeta/OpenMir2/blob/master/README.cn.md)  

[![Main](https://github.com/mirbeta/OpenMir2/actions/workflows/main.yml/badge.svg)](https://github.com/mirbeta/OpenMir2/actions/workflows/main.yml)
[![Dev](https://github.com/mirbeta/OpenMir2/actions/workflows/dev.yml/badge.svg?branch=dev)](https://github.com/mirbeta/OpenMir2/actions/workflows/dev.yml)
[![OSCS Status](https://www.oscs1024.com/platform/badge/OpenMir2.svg?size=small)](https://www.murphysec.com/accept?code=602a83a9b09478f193d69b09c8f3ef11&type=1&from=2)

Legend of Mir 2 game server, support online and multiplayer interaction.

This project refers to the network Delphi code, which can be used with the original 1.76 source code of Legend of Blood for game experience. If you have any questions or problems, please submit Issues.  

### How to use    
## Client Project
>  (https://github.com/mirbeta/MirClient) Here，Use Delphi XE 10.4.

## Server File
> (https://github.com/mirbeta/MirServer) Here，Basic File.

## Startup sequence and project description. 
1. DBSvr (database service, responsible for data storage). 
2. LoginSvr (account login service, responsible for account registration, login, server selection, etc.). 
3. GameSvr (game data engine, responsible for game data processing interaction, spell casting, walking, etc.). 
4. GameGate (game gateway, responsible for sending player data to the game engine, the data interacted by players are all in this service and then forwarded to the data engine for processing). 
5. SelGate (character gateway, responsible for player query, new creation, deletion, etc., and finally processed by DBSvr, the service will not be able to obtain character data after the client logs in if the service is not activated). 
6. LoginGate (login gateway, responsible for forwarding the login data to LoginSvr for processing, the service does not start the client and cannot connect to the game). 

### Images
![](./Images/20220914233717.png)
![](./Images/20220914233713.png)
![](./Images/1632561445962.jpg)
![](./Images/1632561467819.jpg)
![](./Images/1632561488323.jpg)
![](./Images/1632561522104.jpg)
