Title: Simuladores e sintetizadores de HDL
Date: 2018-09-13 08:45
Modified: 2018-10-10 09:40
Category: hdl
Tags: vhdl, verilog, simuladores
Slug: simuladores
Lang: pt_BR
Authors: Bruno Albertini
Summary: Lista de programas para HDL.

Há diversos programas que suportam descrições em HDL. Para começar no seu mundo de projetista de hardware usando VHDL ou Verilog, escolha um programa nesta lista e prepare seu ambiente. Quase todos são um _Integrated Design Environment_ (IDE), ou seja, possuem um ambiente com suporte a descrição incluindo _syntax highlight_, acesso rápido a simulação, síntese e algum sistema de gerenciamento de projetos.

### GHDL
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](https://github.com/ghdl/ghdl/releases) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](http://ghdl.free.fr/)

**HDLs:** VHDL | **SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i> <i style="font-size: 1em;" class="fab fa-linux"></i> <i style="font-size: 1em;" class="fab fa-apple"></i>


O GHDL é um simulador de código aberto para a linguagem VHDL somente, mantido pelo desenvolvedor Tristan Gingold. Permite que você compile e simule sua descrição na sua máquina usando um compilador nativo, o que é bem rápido em comparação aos outros simuladores desta página. Contudo, o GHDL não faz síntese nem simulação temporizada (exceto se você descrever seu circuito usando temporização explícita no VHDL).

Este é o simulador usado para corrigir os exercícios de Sistemas Digitais. Os professores mantém uma máquina virtual com GHDL instalado, atualizado e funcionando, e esta máquina está disponível para os alunos. Veja [este artigo]({filename}vmghdl.md) se deseja trabalhar com esta máquina virtual.

### Active-HDL
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](https://www.aldec.com/students/student.php?id=9) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](https://www.aldec.com/en/products/fpga_simulation/active_hdl_student)

**HDLs:** VHDL, Verilog | **SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i>

Este programa é uma IDE completo e suporta simulação somente. Para síntese, você deve ter instalado um programa de síntese na sua máquina (e.g. Quartus, Vivado, ISE, etc), e a IDE se encarrega de invocá-lo corretamente.

Possui a vantagem de ser mantido por uma empresa terceira ([Aldec](https://www.aldec.com)), independente do fabricante do hardware alvo do seu projeto. O link para download é da versão de estudante e necessita cadastro (use seu email \@usp).

### Quartus
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](http://fpgasoftware.intel.com/?edition=lite) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](https://www.intel.com/content/www/us/en/software/programmable/quartus-prime/download.html)

**HDLs:** VHDL, Verilog | **SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i> <i style="font-size: 1em;" class="fab fa-linux"></i>

O Quartus é um IDE fornecido pela Altera, uma subsidiária da [Intel](https://www.intel.com). Permite simulação através do Modelsim (fornecido com o pacote), incluindo simulação temporizada para os dispositivos fabricados pela Intel. Quando fizer download, tenha certeza que fez download do pacote completo incluindo o Modelsim. O link para download é da versão Lite, que é gratuita para todos e suporta sem licença os dispositivos do programa universitário. Caso esteja trabalhando em algum projeto que utilize um dispositivo não suportado na versão Lite, é possível obter uma licença através do programa universitário (consulte seu orientador).

### Vivado/ISE
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](https://www.xilinx.com/support/download.html) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](https://www.xilinx.com/products/design-tools/vivado.html)

**HDLs:** VHDL, Verilog | **SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i> <i style="font-size: 1em;" class="fab fa-linux"></i>

O Vivado é um IDE fornecido pela [Xilinx](https://www.xilinx.com/). Também permite simulação através do Modelsim (fornecido no pacote), incluindo simulação temporizada para os dispositivos fabricados pela Xilinx. O link para download é genérico, consulte seu professor(a) qual versão irá utilizar (recomendo a Lab Edition pois não precisa de licença alguma). A versão HLx possui ainda suporte a síntese de alto nível.

O ISE é uma versão antiga do IDE da Xilinx disponível somente para Windows. Faça [download](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/design-tools.html) dessa versão somente se for trabalhar com placas antigas (i.e. Spartan-6), caso contrário opte pelo Vivado.

# Programas úteis

### GTKWave
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](https://sourceforge.net/projects/gtkwave/files/) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](http://gtkwave.sourceforge.net/)

**SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i> <i style="font-size: 1em;" class="fab fa-linux"></i> <i style="font-size: 1em;" class="fab fa-apple"></i>

O GTKWave é um visualizador de formas de onda de código aberto baseado no [GTK+](http://www.gtk.org/). Quando estiver simulando a descrição do seu circuito, o seu simulador gera um arquivo [VCD](https://en.wikipedia.org/wiki/Value_change_dump), que deve ser aberto em um visualizador como o GTKWave. Este programa é especialmente útil se você não estiver usando um IDE (e.g. GHDL).

### Atom
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](https://github.com/atom/atom/releases/tag/v1.30.0) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](https://atom.io/)

**SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i> <i style="font-size: 1em;" class="fab fa-linux"></i> <i style="font-size: 1em;" class="fab fa-apple"></i>

O Atom é um editor de textos com suporte a várias linguagens. Eu o utilizo para a maioria dos meus projetos envolvendo HDLs. Para habilitar o suporte a VHDL, instale o pacote `language-vhdl` depois de instalar o atom.

### LogiSim
[<i style="font-size: 1em;" class="fas fa-download"></i> Download](https://github.com/reds-heig/logisim-evolution/releases) |
[<i style="font-size: 1em;" class="fas fa-file-alt"></i> Página](https://github.com/reds-heig/logisim-evolution)

**SOs:** <i style="font-size: 1em;" class="fab fa-windows"></i> <i style="font-size: 1em;" class="fab fa-linux"></i> <i style="font-size: 1em;" class="fab fa-apple"></i>

O LogiSim é uma ferramenta educacional para projetar e simular circuitos digitais. O método de captura é gráfico, ou seja, você desenha o circuito como se estivesse desenhando no papel, na forma de um diagrama, usando portas lógicas. Apesar de suportar HDLs, este não é o foco do projeto. Nota: o projeto original foi descontinuado pelo autor, esta versão é a versão "evolution", que é mantida como software aberto por um grupo de universidades suíças.

# Utilização nas disciplinas
Nas disciplinas teóricas de Sistemas Digitais o GHDL é utilizado para correção dos exercícios, mas não faz muita diferença qual simulador você usa para desenvolver, desde que **não utilize** nenhuma tecnologia dependente de um determinado fabricante. Nestas disciplinas você raramente será solicitado a sintetizar seu circuito.

Nas disciplinas práticas, você invariavelmente irá sintetizar e experimentar seu circuito em uma placa de prototipação. No Laboratório Digital, as placas são do programa universitário da Intel, fabricadas pela Terasic com FPGAs da Intel. Isso significa que você terá que utilizar o Quartus. É possível utilizar o Active-HDL com o Quartus como backend, mas esta configuração ainda não é suportada no laboratório. As disciplinas de Arquitetura de Computadores, apesar de teóricas, possuem forte componente prática e você também precisará de um software que suporte síntese. Contudo, nestas disciplinas a placa utilizada é do programa universitário da Xilinx, fabricadas pela Digilent com FPGAs da Xilinx. O software de síntese deste fabricante é o Vivado (ou ISE para placas antigas), porém a disciplina utiliza o arrajo Active-HDL com o Vivado como backend. Note que o software de síntese só funciona para os dispositivos daquele fabricante, portanto não há como utilizar um software de um fabricante com uma placa de outro (e.g. sintetizar no Vivado e programar a placa da Intel).

Sempre que for configurar seu ambiente, opte pela versão mais atualizada ou consulte qual versão será utilizada na disciplina. Em vários casos, se sua versão for diferente da utilizada no laboratório, você pode ter problemas para levar seu projeto para o laboratório e usar os computadores disponíveis para programar a placa. Em nenhum laboratório há restrições quanto a levar seu próprio notebook, mas consulte sempre o técnico do laboratório ou seu professor(a) para ter certeza que há nenhum problema em ligar a placa no seu próprio equipamento.

A escolha de qual software utilizar é sua, porém aconselho que sempre descreva seu hardware sem utilizar nenhuma construção que dependa de um fabricante específico, assim você pode facilmente transportar seu código de um software para o outro.