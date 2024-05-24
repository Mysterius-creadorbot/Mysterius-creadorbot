<button id="open-modal">Generar imagen anime HD</button>

<div id="modal" class="modal">
  <div class="modal-content">
    <span class="close-button">&times;</span>
    <h2>Generador de imágenes anime HD</h2>
    <form id="image-form">
      <label for="art-style">Estilo de arte:</label>
      <select id="art-style">
        <option value="anime">Anime</option>
        <option value="manga">Manga</option>
      </select>
.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0, 0, 0, 0.4);
}

.modal-content {
  background-color: #fefefe;
  margin: 15% auto;
  padding: 20px;
  border: 1px solid #888;
  width: 80%;
}

.close-button {
  color: #aaa;
  float: right;
  font-size: 28px;
  font-weight: bold;
}

.close-button:hover,
.close-button:focus {
  color: black;
  text-decoration: none;
  cursor: pointer;
}
      <label for="pose">Pose:</label>
      <input type="text" id="pose">
const modal = document.getElementById("modal");
const btn = document.getElementById("open-modal");
const closeBtn = document.querySelector(".close-button");
const form = document.getElementById("image-form");

btn.onclick = function() {
  modal.style.display = "block";
}

closeBtn.onclick = function() {
  modal.style.display = "none";
}

window.onclick = function(event) {
  if (event.target == modal) {
    modal.style.display = "none";
  }
}

form.onsubmit = function(event) {
  event.preventDefault();
  // Enviar la solicitud al generador de imágenes
  // Aquí deberías implementar la lógica para enviar la solicitud al generador de imágenes
  // y mostrar la imagen generada en el modal o en otro lugar de la página.
  console.log("Formulario enviado");
  modal.style.display = "none";
      <label for="background">Fondo:</label>
      <input type="text" id="background">

      <button type="submit">Generar imagen</button>
    </form>
  </div>
</div>
<!---
Mysterius-creadorbot/Mysterius-creadorbot is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
