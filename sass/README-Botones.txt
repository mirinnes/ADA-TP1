/*
--------------------------------------------------------------------------------
Variables que necesitan los botones:

    #BOTON CON FONDO:
    @mixin button-withBackground(
            $buttonBgColor,     //Color de fondo -elegir alguno de los q hay entre las variables de colores- 
            $buttonFontColor,   //Color de la letra 
            $fontSize,          //Tamaño de fuente
            $paddingButtonLR    //Padding Left y Right
            $paddingButtonTB)    //Padding Bottom y Top
    #HOVER: @mixin button-hover-getTransparent($buttonFontColor)
    ---------------------------------------------------------------------------
    #BOTON TRANSPARENTE:
    @mixin button-transparent(
                $buttonFontColor,               //Color de la letra y del Borde
                $fontSize,                      //Tamaño de fuente
                $paddingButtonLR,               //Padding Left y Right
                $paddingButtonTB)               //Padding Bottom y Top  
    #HOVER: @mixin button-hover-getBackground($buttonBgColor)             
--------------------------------------------------------------------------------

/* EJEMPLO DEL USO DE LOS MIXIN PARA BOTON:
    ---Este ejemplo muestra como se usan los include para los botones
    ---Cualquier duda pregunten.

--------------------------------------------------------------------------------

    .clase-boton-CONFONDO {
        //este include agrega los estilos comunes de todos los botones CON FONDO:
        @include button-withBackground(colorDeFondo, colorDeLetra, TamañoFuente, PaddingL-R, PaddingB-T);
        
        //otras propiedades que uds necesiten agregar

        //este include agrega la transicion de hover para que el boton se vuelva TRANSPARENTE:
        @include  button-hover-getTransparent(colorDeLetra);
    }

    .clase-boton-TRANSPARENTE {
        //este include agrega los estilos comunes de todos los botones TRANSPARENTES:
        @include button-transparent(colorDeLetra, TamañoFuente, PaddingL-R, PaddingB-T);
        


        //otras propiedades que uds necesiten agregar



        //este include agrega la transicion de hover para que el boton se vuelva CON FONDO:
        @include  button-hover-getBackground(colorDeFondo);
    }
--------------------------------------------------------------------------------
*/
