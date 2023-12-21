*Pseudo-Classes e Pseudo-Elementos:* permitem a seleção de diversos elementos, permitindo que possamos aplicar estilos a um elemento específico de acordo com o seu estado ou posição dentro do elemento pai.
    *Pseudo-Classe:* é uma palavra adicionada aos seletores que especifica um espado especial do elemento selecionado. 
    ex: seletor:pseudoclasse{propriedade:valor;}
        div:hover{color:orange}
    *:active* Momento em que o usuário o torna "ativo", por exemplo quando clicamos em um botão e náo soltamos o botão do mouse
        ex: a:active{color:blue;}
     *:visited* Usada para estilizar um link que já foi visitado
        ex: a:visited{color:blue}
     *:focus* Usado para estilizar um elemento quando ele recebe foco. Muito comum para campos de texto.
        ex: input: focus{background:yellow}
    *:first-child e :last-child* Usada para estalizar o primeiro filho ou o ultimo filho do elemento
        ex: li:first-child{color:orange}
            li:last-child{color:red}
    *:nth-child()* Permite a seleção de qualquer elemento no meio de um grupo de elementos.
        ex: li:nht-child(2n+1){color:green}
    *:not()* Também conhecida como pseudo-classe de negação. Ela aceita um argumentto-basicamente um outro "seletor" - escrito entre sinais de arênteses.
*Pseudo-classes de Validação* Os pseudo-classes de validação servem para auxiliar no preeenchimento de campos para que o usuário tenha uma experiência melhor. ex: input:submit
    *:checked* Usada para selecionar um elemento <radio>; <checkbox> ou <option> que esteja marcado ou com estado ativado
        ex para qualquer elemento "checkable": :checked{margin-left:25px}
        ex para qualquer elemento radio: 
        input[type="radio"]:checked{margin-left:25px}
        ex apenas para elementos checkbox:
        input[type="checkbox"]:checked{margin-left:25px}
        ex apenas para elementos option:
        option:checked{color:red}
    *:disabled* Usada para selecionar qualquer elemento desativado.
        ex: input:disabled{background:#ccc}
            input[type="text"]:disabled{background:#ccc}
    *:valid e :invalid* Usada para selecionar campos de formulários cujos dados de entrada estejam de acordo, ou não,com o formato requerido para o campo
        ex: input[type=email]:invalid{background:orange}
            input[type=email]:valid{background:green}
    *:required* Usada para selecionar qualquer elemento de formulário cujo preenchimento é orbigatório.
        input:required{background:red}
*Pseudo-elemento* é uma palavra-chave adicionada a um setor que permite que você selecione uma parte específica do elemento. seletor::pseudoelemento{propriedade:valor}
    *::placeholder* Usada para selecionar um placeholder (texto que fornece ao usuário uma dica que descreve o valor esperado em um determinado campo de entrada) de um elemento. 
        ex: ::placeholder{color:yelow}
    *::first-line* Usada para selecionar a primeira linha de um elemento no nível do bloco
        ex: p::first-line{color:blue}
    *::selection* Usada para selecionar a parte de um elemento por um usuário
        ex: p::selecion{color:red; background:yellow}
    *::marker* Usada para selecionar os marcadores dos itens da lista
        ex: ::marker{color:red; font-size:23px}
    *::before* Cria um elemento antes do elemento especificado. Precisa especificar uma especificidade chamada content
        ex: ::before{content:"10px"; width:100px; margin:100px; background:red}
