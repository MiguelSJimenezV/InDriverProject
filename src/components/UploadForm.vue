<template>
  <form id="form">
    <div class="mb-3">
      <label for="foto" class="form-label">Portada del Tema</label>
      <input
        type="file"
        class="form-control"
        id="foto"
        name="foto"
        accept="image/*"
      />
    </div>
    <div class="mb-3">
      <label for="nombre" class="form-label">Nombre del Artista/Banda</label>
      <input
        type="text"
        class="form-control"
        id="nombre"
        name="nombre"
        required
      />
    </div>
    <div class="mb-3">
      <label for="cancion" class="form-label">Archivo del Tema</label>
      <input
        type="file"
        class="form-control"
        id="cancion"
        name="cancion"
        accept="audio/*"
        required
      />
    </div>
    <div class="mb-3">
      <label for="nombre" class="form-label">Nombre del Tema</label>
      <input
        type="text"
        class="form-control"
        id="nombre"
        name="nombre"
        required
      />
    </div>
    <div class="mb-3">
      <label for="tipo">Tipo de Canción</label>
      <select class="form-select" id="tipo" name="tipo">
        <option value="original">Original</option>
        <option value="remix">Remix</option>
        <option value="cover">Cover</option>
      </select>
    </div>
    <div class="mb-3">
      <label for="explicito" class="form-check-label"
        >Contenido Explícito</label
      >
      <div>
        <input
          class="form-check-input"
          type="radio"
          name="explicito"
          id="explicito-si"
          value="si"
        />
        <label class="form-check-label" for="explicito-si">Sí</label>
      </div>
      <div>
        <input
          class="form-check-input"
          type="radio"
          name="explicito"
          id="explicito-no"
          value="no"
          checked
        />
        <label class="form-check-label" for="explicito-no">No</label>
      </div>
    </div>
    <div class="mb-3">
      <label for="anio" class="form-label">Año de Grabación</label>
      <input
        type="number"
        class="form-control"
        id="anio"
        name="anio"
        min="1990"
        max="2025"
        step="1"
        value="2024"
      />
    </div>
    <div class="mb-3">
      <label for="genero" class="form-label">Género Musical</label>
      <select class="form-select" id="genero" name="genero">
        <option value="Pop">Pop</option>
        <option value="Rap/Trap">Rap/Trap</option>
        <option value="Reggaeton">Reggaeton</option>
        <option value="Techno">Techno</option>
        <option value="Dacehall">Dacehall</option>
        <option value="Lofi">Lofi</option>
        <option value="R&B">R&B</option>
        <option value="Jersey">Jersey</option>
        <option value="Otro">Otro</option>
      </select>
    </div>
    <div class="mb-3">
      <label for="plataformas" class="form-label"
        >Plataformas de Distribución</label
      >
      <select multiple class="form-select" id="plataformas" name="plataformas">
        <option value="spotify">Spotify</option>
        <option value="Youtube">Youtube</option>
        <option value="TikTok">TikTok</option>
        <option value="Instagrm">Instagrm</option>
        <option value="InDriver">InDriver</option>
        <option value="Deezer">Deezer</option>
        <option value="apple">Apple Music</option>
        <option value="amazon">Amazon Music</option>
      </select>
    </div>
    <div class="mb-3">
      <label for="continentes" class="form-label"
        >Continentes de Distribución</label
      >
      <select multiple class="form-select" id="continentes" name="continentes">
        <option value="america">América</option>
        <option value="europa">Europa</option>
        <option value="asia">Asia</option>
        <option value="africa">África</option>
        <option value="oceania">Oceanía</option>
      </select>
    </div>
    <div class="mb-3">
      <label for="autor" class="form-label">Autor</label>
      <input type="text" class="form-control" id="autor" name="autor" />
    </div>
    <div class="mb-3">
      <label for="colaboradores" class="form-label">Colaboradores</label>
      <input
        type="text"
        class="form-control"
        id="colaboradores"
        name="colaboradores"
      />
    </div>
    <button type="submit" class="btn btn-primary">Subir Canción</button>
  </form>
</template>
