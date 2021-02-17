<html>
    <head>
        <meta charset="UTF-8">
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
        <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
        <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
        <link rel="stylesheet" type="text/css" href="static/css/common.css" />
       
        <link rel="stylesheet" type="text/css" href="static/css/style.css" />
        <link href='http://fonts.googleapis.com/css?family=Open+Sans:300,700' rel='stylesheet' type='text/css' />
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <script src="https://unpkg.com/scrollreveal/dist/scrollreveal.min.js"></script>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
        <link rel="stylesheet" href="animate.css">
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
        <script src="wow.min.js"></script>
        <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.11"></script>
    </head>

    <style>
        .fundo{
        background-color:black;
        color:white;
        font-size:26px
      }
       .formata{
           color:white;
           font-size:40px;
       }
        .imagemfundo{
    background-image: url(subestacao.png); 
    max-width: 1600px;
    height: 400px;
}
   #navbar{
       top:50px;
   }
        .hidden{
     opacity:0;
}
.visible{
     opacity:1;
}
        H3{
            color:white;
        }
  
    .esconde1{
        display:none
    }
    .navbar1{
        background-color:white;
        color:black;
    }
    .navbar2{
        background-color:white;
        color:black;
    }
    .sticky {
  position: fixed;
 ;
  width: 100%;
 
}

.sticky + .content {
  padding-top: 60px;
  
}
   
    @media (min-width: 800px) and (max-width: 1100px){
       .mobile{
           font-size:24px
       }
    }
    @media (min-width: 400px) and (max-width: 800px){
        .mobile{
           font-size:24px
       }
    }
    @media (max-width: 400px)
{
    .mobile{
           font-size:24px
       }
}
    </style>
    <body>
        
        <script>
            new WOW(
               {
                mobile:true, 
               } 
            ).init();
            </script>
        <script>
        //    jQuery(function($){
   // $(document).ready(function(){
       // window.sr = ScrollReveal();
     
      //sr.reveal('.t', {duration: 3500});
     //   $('.carousel').carousel({
  //interval: 2500
//})
   // });
//});
        </script>
        <script>
   jQuery(function($){
    $(document).ready(function(){
        $("#botao").click(function () {
   
    var texto = $("#senha").val();
    console.log(texto);
    $.ajax({
    url: "http://127.0.0.1:5000//api/v1/resources/books/all",
    data :{
            senha : texto,            
                },
    dataType: 'json',
    type: "POST",
    
   })
  .done(function( data ) {
    console.log(data[1].author)
  });
   
  });
    });
});
        </script>
        
       
         <div class="row">
            
            <div class="col-md-12">
                <center>
                <img src="static/images/logo.png" >
            </center>
            </div>
        
        </div>
            <div class="row">
              
            <div class="col-md-12 ">
                <center>
                <nav  id="navbar" class="navbar sticky-top   navbar-expand-lg  navbar-light navbar1 ">
                    <a class="navbar navbar1" href="index.html">Home</a>
                    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                      <span class="navbar-toggler-icon"></span>
                    </button>
                  
                    <div class="collapse navbar-collapse" id="navbarSupportedContent">
                      <ul class="navbar-nav mr-auto">
                        <li class="nav-item active">
                          <a class="navbar navbar1 " href="empresa.html">Empresa<span class="sr-only">(current)</span></a>
                        </li>
                        
                        <li class="nav-item dropdown">
                          <a class="navbar dropdown-toggle  navbar1" href="projetoel.html" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Projeto Elétrico
                          </a>
                          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <a class="dropdown-item " href="projetoel.html">Diagrama Unifilar e planta elétrica</a>
                            <a class="dropdown-item " href="projetocap.html">Banco de Capacitor</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item " href="painelsol.html">Painel Fotovoltaico</a>
                          </div>
                        </li>
                       
                       
                      
                        <li class="nav-item active">
                                
                            <a class="navbar navbar1 " href="https://api.whatsapp.com/send?phone=5511991385051&text=Bom_dia"><i class="fa fa-whatsapp"></i>&nbsp<span class="sr-only">(current)</span></a>
                          </li>
                          <li class="nav-item active">
                            
                            <a class="navbar navbar1 " href="https://www.facebook.com/braunprojetoseletricos"><i class="fa fa-facebook" style="font-size:22px"></i>&nbsp<span class="sr-only">(current)</span></a>
                          </li>
                          <li class="nav-item active">
                            
                            <a class="navbar navbar1 " href="https://www.instagram.com/braunprojetoseletricos/"><i class="fa fa-instagram" style="font-size:22px"></i>&nbsp<span class="sr-only">(current)</span></a>
                          </li>
                          <li class="nav-item active">
                            
                            <a class="navbar navbar1 " href="https://www.linkedin.com/in/braun-projetos-el%C3%A9tricos-45a172206/"><i class="fa fa-linkedin" style="font-size:22px"></i>&nbsp<span class="sr-only">(current)</span></a>
                          </li>
                        
                      </ul>
                     
                    </div>
                  </nav>
                </center>
            </div>
        </div>
        <script>
            window.onscroll = function() {myFunction()};
            
            var navbar = document.getElementById("navbar");
            var sticky = navbar.offsetTop;
            
            function myFunction() {
              if (window.pageYOffset >= sticky) {
                navbar.classList.add("sticky")
              } else {
                navbar.classList.remove("sticky");
              }
            }
            </script>
        <div class="row">
            
            <div class="col-md-12 imagemfundo">
                <br><br><br><br>
                &nbsp; &nbsp; &nbsp;
                <span id="typed" class="formata"></span>
        </div>
    </div>
       
    <script>
        var typed = new Typed('#typed',{
                    strings:["Construindo um futuro","Com a satisfação do cliente"],
                    backSpeed: 100,
                    typeSpeed: 100,
                    loop: true,
                    
                   shuffle: true
                  });
    </script>
    <div class="row">
           
        <div class="col-md-12">
            <center>
                <H1>Nossos serviços</H1>
            </center>
            </div>
        </div>
        <div class="row">
           
            <div class="col-md-4">
                <!-- 
                <button type="button" id="botao">testando</button>
                <br>
                <input type="text" name="senha" id="senha">
                -->
                <br>
                    <section class="main">
			
                        <ul class="ch-grid">
                            <li>
                                <div class="ch-item ch-img-1">
                                    <div class="ch-info">
                                        <h3>Encomende já o seu Projeto Elétrico</h3>
                                        <p>Com a nossa equipe <a href="http://drbl.in/eOPF"></a></p>
                                    </div>
                                </div>
                              
                                <br>
                            </li>
                            <p class="mobile">Elaboração de projetos elétricos, diagrama unifilar e padrão de entrada. Atendemos
                                as exigências da concessionária de sua região</p>
                            </ul>
                    </section>
                            </div>
                            <div class="col-md-4">
                                <section class="main">
                                <ul class="ch-grid">
                                    <li>
                                <div class="ch-item ch-img-2">
                                    <div class="ch-info">
                                        <h3>Correção do fator de potência</h3>
                                        <p>Com a nossa equipe <a href="http://drbl.in/eKMi"></a></p>
                                    </div>
                                </div>
                                <br>
                            </li>
                            <p class="mobile" >Medições de carga reativa e dimensionamento do banco de capacitores ,melhorando a eficiência energética. Conforme a norma da concessionária de sua regiçao</p>
                        </ul>
                                </section>
                    </div>
                    <div class="col-md-4">
                        <section class="main">
                    <ul class="ch-grid">
                         <li>
                                <div class="ch-item ch-img-3">
                                    <div class="ch-info">
                                        <h3>Peça o seu projeto solar</h3>
                                        <p>Com a nossa equipe<a href="http://drbl.in/ekhp"></a></p>
                                    </div>
                                </div>
                                <br>

                                
                            </li>
                            <p class="mobile">Modelagem de painel fotovoltaico  no telhado de sua residência. Atendendo  requisitos de potência
                                e demanda da concessionária de sua região
                            </p>
                        </ul>
                        
                    </section>
                
            </div>
        </div>
        <br><br>
        <div class="row">
            <div class="col-md-2">
                &nbsp
            </div>
            <div class="col-md-10">
                <center>
                   
                    <h1 class="t"> Conte com a nossa equipe</h1>
                </center>
                    <br>
            </div>
           
        </div>
        <div class="row">
            <div class="col-md-2">
                &nbsp
            </div>
            <div class="col-md-4">
              <!-- <img src="../static/images/profissa.jpg" class="t"> --> 
              <section class="wow slideInLeft" data-wow-duration="2s" > 
                <img src="static/images/profissa.jpg" >

              </section>
                
            </div>

            <div class="col-md-2">
                
                </div>
               
                <div class="col-md-2">
                    <!--  <img src="../static/images/bigben.jpg" class="t"> -->
                   
                    <section class="wow slideInRight" data-wow-duration="2s" > 

                        <img src="static/images/bigben.jpg" >
                    </section>
                </div>
               </div>

        <br><br>
        <div class="container">
        
    </div>
    <div class="row">
        <div class="col-md-12 fundo">
            <center>
            <H1 class="t">  Contato</H1>
            <br>
            <p class="fundo t " >  <i class="fa fa-whatsapp"> (11)95046-6230</i></p>
               
            
            <br>
            <p class="fundo t">
                email:braunprojetoseletricos@gmail.com
            </p>
            <p class="fundo t">
                Atendimento:Segunda a sexta. 7:00 ás 19:00
            </p>
           
              
        </center>
        </div>
        
    
</div>

        
    </body>
</html>
