# diagrama-DIO-umlDesafioiPhone

classDiagram
    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet

    class iPhone {
      +tocar() 
      +pausar()
      +selecionarMusica("After Dark")

      +ligar("55XX99999999")
      +atender()
      +iniciarCorreioVoz()

      +exibirPagina("www.google.com.br")
      +adicionarNovaAba()
      +atualizarPagina()
    }

    class ReprodutorMusical {
      +tocar() 
      +pausar()
      +selecionarMusica(String musica)
    }
    ReprodutorMusical : <<interface>>

    class AparelhoTelefonico {
      +ligar(String numero)
      +atender()
      +iniciarCorreioVoz()
    }
    AparelhoTelefonico : <<interface>>

    class NavegadorInternet {
      +exibirPagina(String url)
      +adicionarNovaAba()
      +atualizarPagina()
    }
    NavegadorInternet : <<interface>>
