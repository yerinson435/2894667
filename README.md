<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>formulario</title>
  </head>

  <body>
    <form action="controlador" method="get">
      <label for="edad">ingrese su edad</label>
      <input
        type="number"
        step="1"
        min="0"
        max="20"
        value="5"
        name="edad"
        disabled
      />
      <div>
        <label for="nombre">nombre</label>
        <input
          type="text"
          name="nombre"
          required
          placeholder="ingrese su nombre"
          id="nombre"
          autofocus
          autocomplete="off"
        />
      </div>
      <div>
        <label for="color">seleccione un color</label>
        <input type="color" id="color" />
      </div>
      <div>
        <label for="email">ingres su correo</label>
        <input type="email" id="email" required />
      </div>
      <div>
        <label for="numero">ingrese su numero</label>
        <input type="text" id="numero" pattern="[0-9] {0,10}" />
      </div>
      <div>
        <label for="ciudad">seleccione su ciudad</label>
        <select name="ciudad" id="ciudad" disabled>
          <option value="1">giron</option>
          <option value="2">bucaramanga</option>
          </select>
      </div>
      <button type="submit">guardar</button>
    </form>
  </body>
</html>
