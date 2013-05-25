## IE 
### Validação de [inscrições estaduais](http://pt.wikipedia.org/wiki/Inscri%C3%A7%C3%A3o_Estadual "Inscrição Estadual no Wikipedia") em JavaScript (browser e node.js)
Escrito por [@renatoargh](http://www.github.com/renatoargh "Renato Gama") para [@gammasoft](http://www.github.com/gammasoft "Gammasoft")

![IE - Status da build](https://travis-ci.org/gammasoft/ie.png) &nbsp; ![IE - Status das dependencias](https://gemnasium.com/gammasoft/ie.png) &nbsp; ![IE - Última versão](https://badge.fury.io/js/inscricaoestadual.png)

### Instalação
    npm install inscricaoestadual

### Utilização
#### Node.js 

    var ie = require("inscricaoestadual");
    ie(uf, inscricaoEstadual);
    
#### Browser

    <script src="ie.min.js"></script>
    <script>
        var ie = require("./ie");
        ie(uf, inscricaoEstadual);
    </script>

A função `ie` retorna um boleano, indicando se a inscrição estadual é válida ou não.

Onde, `uf` deve ser uma string entre um dos valores 
    
    var estados =
      ["ac", "al", "ap", "am", 
      "ba", "ce", "df", "es",
      "go", "ma", "mt", "ms",
      "mg", "pa", "pb", "pr",
      "pe", "pi", "rj", "rn",
      "rs", "ro", "rr", "sc",
      "sp", "se", "to"];

E `inscricaEstadual` uma string contendo o valor a ser validado. 
Pode-se receber uma string com máscara, pois os separadores `[".", "-", "/", " "]` são desconsiderados para a validação.

### Teste

Para rodar os testes:

    npm install //caso você ainda não tenho o nodeunit
    npm test

Todas as inscrições estaduais nos teste foram obtidas publicamente na internet. 
Se você obteve uma validação falsa para uma inscrição estadual verdadeira, pesquisa no site do [SINTEGRA](http://www.sintegra.gov.br/ "Sintegra") se de fato esta inscrição estadual existe e é valida, neste caso [abra uma notificação](https://github.com/gammasoft/ie/issues/new) aqui no GitHub para apurarmos o caso. 

### Implementados até agora (15 de 27 - 55.55%)
**Região Centro-Oeste**
- [X] Mato Grosso do Sul
- [X] Mato Grosso
- [X] Goiás
- [X] Distrito Federal

**Região Sudeste** 
- [X] Minas Gerais 
- [X] Espírito Santo 
- [ ] Rio de Janeiro 
- [X] São Paulo

**Região Sul**
- [X] Paraná
- [ ] Santa Catarina
- [X] Rio Grande do Sul

**Região Norte**
- [ ] Rondônia
- [X] Acre
- [ ] Amazonas
- [ ] Roraima
- [X] Pará
- [ ] Amapá
- [ ] Tocantins

**Região Nordeste** 
- [X] Maranhão 
- [X] Piauí 
- [X] Ceará 
- [ ] Rio Grande do Norte 
- [ ] Paraíba 
- [X] Pernambuco 
- [ ] Alagoas 
- [ ] Sergipe 
- [ ] Bahia  

-----------------------------------------

#### Faça uma doação :)
[![Faça uma doação!](https://www.paypalobjects.com/pt_BR/BR/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/br/cgi-bin/webscr?cmd=_flow&SESSION=qNGRiSLjATOZ2vcKDXVkTmXi5nz5yqBQNI2wQ-qmHQ4wtKUIIg9Px9HR3QG&dispatch=5885d80a13c0db1f8e263663d3faee8d14f86393d55a810282b64afed84968ec)

#### Licença BSD

Copyright (c) 2013, Renato Mendonça da Gama  
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

- Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer. 
- Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution. 

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
