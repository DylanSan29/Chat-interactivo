<!DOCTYPE html>

<html lang="en" xmlns="http://www.w3.org/1999/xhtml">
<head>
    <meta charset="utf-8" />
    <title>Chat interactivo</title>

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

    <style>
        .login
        {
            width: 600px;
            margin: 0 auto;
            background-color: #ccc;
            padding: 25px;
            text-align: center;
            border: 2px solid #000;
            border-radius: 10px;
            font-size: 20pt;
            box-shadow: 10px 10px 10px #333;
            height: 40%;
            margin-top: 100px;
            display: none;
        }

        input
        {
            font-size: 15pt;
            padding: 10px;
            border-radius: 10px;
        }
        .chat
        {
            width: 1200px;
            margin: 0 auto;
            background-color: #ccc;
            padding: 25px;
            text-align: center;
            border: 2px solid #000;
            border-radius: 10px;
            font-size: 20pt;
            box-shadow: 10px 10px 10px #333;
            height: 90%;
            display: none;
        }
        .chat-mensajes
        {
            width: 100%;
            background-color: #fff;
            border: 2px solid #000;
            border-radius: 10px;
            text-align: left;
            height: 520px;
        }
        .chat-escribir
        {
            margin-top: 10px;
        }

        input[id=text-mensaje]
        {
            width: 92%;
        }
    </style>
</head>
<body>

 <div id="login" class="login">

     <h3>Ingrese su nickname:</h3>
     <input type="text" id="username" />
     <br /><br />
     <input type="button" value="Ingresar al chat" id="button-ingresar" />

 </div>

<div id="chat" class="chat">

    <div class="chat-mensajes" id="chat-mensajes">
        ¡Bienvenido al chat! <br />
    </div>

    <div class="chat-escribir" id="chat-escribir">
        <input type="text" class="text-mensaje" id="text-mensaje" />
        <input type="button" value="Enviar" class="button-enviar" id="button-enviar" />
    </div>

</div>
</body>
<script src="/socket.io/socket.io.js"></script>
<script>
    var socket = io();

 $(document).ready(function () 
 {

     $('#login').fadeIn(500);

 });

 $('#button-ingresar').click(function () 
 {
        var username = $('#username').val();

        if (username=='') {
            alert('Debes escribir un nombre');
        }
        else {

            socket.emit('crearUsuario', username);

            $('#login').fadeOut(500, function () {
                $('#chat').fadeIn(500);
            });
        }
 });
$('#text-mensaje').keypress(function(event)
{
    if (event.wich == 13)
    {
        $('#button-enviar').click();
    }
});
$('#button-enviar').click(function()
{
    var mensaje = $('#text-mensaje').val();

    if(mensaje!='')
    {
        $('#text-mensaje').val('');

        socket.emit('mensajeNuevo', mensaje);
    }
});

socket.on('mensaje', function(data)
{

    var nuevoMensaje = '<b>' + data.usuario + ' dijo:</b>' + data.mensaje;

    $('#chat-mensajes').append(nuevoMensaje + '<br/>');

});
      
 

</script>
</html>