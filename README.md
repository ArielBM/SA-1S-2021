# SA-1S-2021




<h1>Diccionario de Datos</h1>



<h3>Usuario</h3>

<table>
<thead>
	<tr>
		<th>Campo</th>
		<th>Tipo</th>
        <th>Dominio</th>
		<th>Descripción</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>ID Usuario</td> 
		<td>caracter</td>
		<td>Alfa-Numerico</td>
     	<td>Alias de la persona que puede gestionar el sistema</td>
	</tr>
	<tr>
		<td>Nombre</td> 
		<td>caracter</td>
		<td>Alfabeto</td>
     	<td>Nombre de la persona que a ingresado en el sistema</td>
	</tr>
	<tr>
		<td>Correo</td> 
		<td>caracter</td>
		<td>Alfa-númerico</td>
     	<td>Correo electronico del usuario del sistema</td>
	</tr>    
    	<tr>
		<td>Contraseña</td> 
		<td>caracter</td>
		<td>Alfa-númerico</td>
     	<td>Valor encriptado de la clave de ingreso de la persona</td>
	</tr>    
  </tbody>
</table>


<h3>Datos  Eleciones</h3>

<table>
<thead>
	<tr>
		<th>Campo</th>
		<th>Tipo</th>
                <th>Dominio</th>
		<th>Descripción</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>ID Elecciones</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Id Identificador unico de la votación a ser dispuesta al publico</td>
	</tr>
	<tr>
		<td>Nombre de la Eleccion</td> 
		<td>Caracter</td>
		<td>Alfa-Númerico</td>
        <td>Nombre que sera puesto a disposición del publico y de como se recocera a elección a 		realizada</td>
	</tr>
    <tr>
		<td>Nombre de la Eleccion</td> 
		<td>Caracter</td>
		<td>Alfa-Númerico</td>
        <td>Nombre que sera puesto a disposición del publico y de como se recocera a elección a 		realizada</td>
	</tr>
    <tr>
		<td>Fecha Habilitación</td> 
		<td>Datetime</td>
		<td>Fecha</td>
        <td>Fecha y hora en la cual se habilita la recepción de votos de la elección ingresada</td>
	</tr>
     <tr>
		<td>Fecha Inabilitación</td> 
		<td>Datetime</td>
		<td>Fecha</td>
        <td>Fecha y hora en la cual ya no se permitirá el ingreso de más votaciones</td>
	</tr>
      <tr>
		<td>Estado</td> 
		<td>int</td>
		<td>0-ingresado,1-Aprobado,2-publicado,3-Cerrado</td>
        <td>Representa el estado en que se encuentra la elección a ser realizada o que ya se a concluido</td>
	</tr>
    </tbody>
</table>

   

<h3>Opciones Elección</h3>

<table>
<thead>
	<tr>
		<th>Campo</th>
		<th>Tipo</th>
        <th>Dominio</th>
		<th>Descripción</th>
	</tr>
</thead>
<tbody>
      <tr>
		<td>ID Opción</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Id Identificador de participante o elemento sometido a elección durante labotación</td>
	</tr>
	<tr>
		<td>ID Elecciones</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Id Identificador único de la votación a ser dispuesta al publico</td>
	</tr>
	<tr>
		<td>Título</td> 
		<td>Caracter</td>
		<td>Alfa-Númerico</td>
        <td>Nombre Representativo del elemento que esta sujeto a selección por los votantes</td>
	</tr>
    <tr>
		<td>Logo</td> 
		<td>imagen</td>
		<td>image</td>
        <td>Imagen o logotivo representantivo del elemento a ser sujeta a votación</td>
	</tr>
    <tr>
		<td>Atribucciones</td> 
		<td>caracter</td>
		<td>Alfa-númerico</td>
        <td>Listado de atribuciónes asocaidos al elemento sometido a elección, formato Json</td>
	</tr>
      <tr>
		<td>Ganador elección</td> 
		<td>int</td>
		<td>Número entero</td>
        <td>Distintivo si la opción es la ganadara de las votaciones,0-No,1-Si</td>
	</tr>
     <tr>
		<td>Número de Votos</td> 
		<td>int</td>
		<td>Número entero</td>
        <td>Conteo del número de votos obtenidos durante las elecciones</td>
	</tr>
    </tbody>
</table>



<h3>Registro</h3>

<table>
<thead>
	<tr>
		<th>Campo</th>
		<th>Tipo</th>
        <th>Dominio</th>
		<th>Descripción</th>
	</tr>
</thead>
<tbody>
      <tr>
		<td>ID Registro</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Id Identificador de la participación de una persona en una votación</td>
	</tr>
	<tr>
		<td>Identificación Persona</td> 
		<td>Caracter</td>
		<td>alfa-númerico</td>
     	<td>Id de documento de identificación de la persona registrada para votar</td>
	</tr>
    <tr>
		<td>Tipo Voto</td> 
		<td>int</td>
		<td>Númerico</td>
        <td>Forma en la que participo la persona en la votación 0-Presencial,1-Virtual</td>
	</tr>
	<tr>
		<td>Estado Votación</td> 
		<td>int</td>
		<td>Númerico</td>
        <td>Estado en el cual esta el registro de votacion de una persona 0-registrado,1-emitido</td>
	</tr>
    </tbody>
</table>



<h3>Persona</h3>

<table>
<thead>
	<tr>
		<th>Campo</th>
		<th>Tipo</th>
        <th>Dominio</th>
		<th>Descripción</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Identificación Persona</td> 
		<td>caracter</td>
		<td>alfa-númerico</td>
     	<td>Número de Identificador del documento emitido para la persona</td>
	</tr>
     <tr>
		<td>Dispositivo Móvil</td> 
		<td>caracter</td>
		<td>alfa-númerico</td>
     	<td>Número de Identificador del documento emitido para la persona</td>
	</tr>
     <tr>
		<td>Número Teléfono</td> 
		<td>int</td>
		<td>Númerico</td>
     	<td>Número de contacto de la persona que se a registrado a las elecciones</td>
	</tr>
         <tr>
		<td>Fotografia de la persona</td> 
		<td>Image</td>
		<td>Imagen</td>
     	<td>Foto de la persona que se a registrado para participar en alguna elección</td>
	</tr>
    </tr>
    <tr>
		<td>Fotografia de Documento de Identificación</td> 
		<td>Image</td>
		<td>Imagen</td>
     	<td>Foto de la persona que se a registrado para participar en alguna elección</td>
	</tr>
    <tr>
		<td>PIN</td> 
		<td>int</td>
		<td>Número</td>
     	<td>Número identificador para acceder a opciones de usuario en aplicativo</td>
	</tr>
    <tr>
		<td>Correo</td> 
		<td>caracter</td>
		<td>alfa-númerico</td>
     	<td>Correo electronico utilizado por el usuario</td>
	</tr>
    <tr>
		<td>Departamento</td> 
		<td>caracter</td>
		<td>Alfabeto</td>
     	<td>Departamento a la que pertenece la Persona</td>
	</tr>
    <tr>
		<td>Municipio</td> 
		<td>caracter</td>
		<td>Alfabeto</td>
     	<td>Municipio a la que pertenece la Persona</td>
	</tr>
    <tr>
		<td>Geolocalización</td> 
		<td>Caracter</td>
		<td>Alfanumerico</td>
     	<td>Punto GPS desde donde la persona a efectuado su registro</td>
	</tr>
    <tr>
		<td>Fecha Registro</td> 
		<td>datetime</td>
		<td>Fecha-hora</td>
     	<td>La fecha y hora que el cliente a ingresado su información al sistema</td>
	</tr>
    </tbody>
</table>


<h3>Votación Presencial</h3>

<table>
<thead>
	<tr>
		<th>Campo</th>
		<th>Tipo</th>
        <th>Dominio</th>
		<th>Descripción</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Identificación Voto</td> 
		<td>int</td>
		<td>Númerico</td>
     	<td>Id identificador del voto cargado en el sistema</td>
	</tr>
    <tr>
		<td>Identificación Persona</td> 
		<td>caracter</td>
		<td>alfa-númerico</td>
     	<td>Número de Identificador del documento emitido para la persona</td>
	</tr>
    <tr>
		<td>ID Elecciones</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Id Identificador unico de la votación a ser dispuesta al publico</td>
	</tr>
    <tr>
		<td>Tipo Persona</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Indica el tipo de persona que efectuo el voto 0-local,1-Extranjero</td>
	</tr>    
    <tr>
		<td>Voto Valido</td> 
		<td>int</td>
		<td>Númerio entero</td>
     	<td>Indica si el voto emitido con el documento ingresado fue registrado como voto 0-No valido,1-Valido</td>
	</tr>    
    </tbody>
</table>
