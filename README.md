# NEANDER – Computador Teórico em VHDL

Este repositório é um fork do projeto original do qual participei, desenvolvido para a disciplina de Sistemas Digitais.

Projeto acadêmico: Implementação completa do computador teórico NEANDER utilizando VHDL.

Repositório original:
https://github.com/EduardoGarzon/NEANDER


##  Contexto Acadêmico

Disciplina: Sistemas Digitais  
Professor: Edmar Bellorini  
Curso: Ciência da Computação  

O projeto consistiu na implementação completa do computador teórico NEANDER, incluindo seus módulos principais e componentes auxiliares.


##  Sobre o NEANDER

O NEANDER é um computador didático utilizado para ensino de arquitetura e organização de computadores.  

Neste projeto foram implementados:

- Unidade Lógica e Aritmética (ULA)
- Módulo de Memória
- Módulo de Controle
- Program Counter (PC)
- Registradores auxiliares
- Unidade de Controle
- Decodificador de instruções

Todos os módulos foram desenvolvidos em VHDL conforme o modelo apresentado em aula.


##  Estrutura do Projeto

O sistema foi dividido nos seguintes módulos:

### 🔹 Módulo ULA
- acumulador.vhdl
- ula.vhdl
- reg_flags.vhdl
- mux5x8.vhdl
- mux2x8.vhdl
- tb_ModuloULA.vhdl

### 🔹 Módulo Memória
- as_ram.vhdl
- Modulo Memória.vhdl
- REGISTRADOR_REM.vhdl
- REGISTRADOR_RDM.vhdl
- mux2x8mem.vhdl
- tb_modulomemoria.vhdl

### 🔹 Módulo Controle
- Unidade de Controle.vhdl
- Módulo de Controle.vhdl
- decodificador.vhdl
- ADD.vhdl
- AND.vhdl
- JMP.vhdl
- JNZf.vhdl
- LDA.vhdl
- HLT.vhdl
- contador.vhdl

### 🔹 Módulo PC
- regPC.vhdl
- pcadder.vhdl
- Módulo PC.vhdl



##  Decisões de Projeto

Algumas decisões importantes adotadas no desenvolvimento:

- Separação do módulo PC e da Unidade de Controle em arquivos independentes.
- Reaproveitamento de componentes como FFJK, registradores de 1 e 8 bits e somadores para evitar redundância.
- Inserção de clock no módulo de memória (`as_ram`) para evitar inconsistências detectadas em testes.
- Implementação das instruções de salto (JN, JZ, JMP, JNZf) conforme modelagem definida na Unidade de Controle.



##  Testes

O projeto inclui arquivos de simulação:

- tb_NEANDER.vhdl
- tb_NEANDER.gtkw

Foi utilizado o exercício “Maior Número” como teste funcional para validação do funcionamento do computador.


##  Participação

Projeto desenvolvido em grupo durante a graduação. Contribuí no desenvolvimento e integração dos módulos do sistema, bem como na implementação e testes das funcionalidades do computador teórico.

Este fork tem como objetivo registrar minha participação acadêmica e compor meu portfólio técnico.
