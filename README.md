# prueba-entrevista-
Interview web project - Entrevista proyecto web
// Adjunto el codigo de html y js de la prueba tecnica
este codigo tiene 4 partes 
el primero es codigo esta realizado con el fin de desrrollar el menu de kitclub 
en la segunda parte tenemos un tipo de carrucel que esta en la pagina de  kitclub 
en la tercera tenemos el input de la publicacion 
el cuarto y el ultimo tenenmos la publiacacion en donde se muestra la imagen y el texto del anterior input 
//___________________________________________________________________________________________
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>KlipWall</title>
    <link rel="stylesheet" href="xd.css" />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css"
    />
    <link
      rel="stylesheet"
      href="https://cdn.jsdelivr.net/npm/semantic-ui@2.4.2/dist/semantic.min.css"
    />
    <!-- Cropper CSS -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/cropperjs/1.5.12/cropper.min.css"
    />

    <style>
      .close-btn {
        position: absolute;
        top: 10px;
        right: 10px;
        background-color: red;
        color: white;
        border: none;
        border-radius: 50%;
        width: 30px;
        height: 30px;
        cursor: pointer;
        display: flex;
        justify-content: center;
        align-items: center;
      }
      .preview-container {
        position: relative;
        margin-top: 20px;
      }
    </style>
  </head>
  <body>
    <!-- parte 1 -->
    <header class="navbar">
      <div class="navbar-logo">
        <img
          src="https://pantherahub.com/storage/projects/9c379a6a-23c2-413d-9813-573105537510/b1a92306-e6e8-4699-964b-3306b78e06bd.jpg"
          alt="Klipclub Logo"
        />
      </div>
      <nav class="navbar-menu">
        <a href="#">Broadcasts</a>
        <a href="#">Virtual Events</a>
        <a href="#">Artists</a>
        <a href="#">KlipWall</a>
      </nav>
      <div class="navbar-search">
        <input type="text" placeholder="Search" />
        <i class="fas fa-search"></i>
        <!-- Icono de búsqueda -->
        <i class="fas fa-video video-icon"></i>
        <!-- Icono de vídeo -->
      </div>
      <div class="navbar-icons">
        <i class="comment icon"></i>
        <div class="notification-icon">
          <i class="bell icon"></i>
          <span class="notification-count">2</span>
          <!-- Número de notificaciones -->
        </div>
        <div class="user-avatar">
          <img
            src="https://xstore.8theme.com/elementor/demos/book-store/wp-content/uploads/sites/78/2022/05/Eleanor-Pena.jpeg"
            alt="User Avatar"
          />
        </div>
      </div>
    </header>

    <!-- carrucel -->

    <section class="trending-now">
      <h2>Trending Now</h2>
      <div class="carousel-container">
        <div class="carousel">
          <div class="cards">
            <article class="card">
              <img
                src="https://yt3.googleusercontent.com/qaGqChT0ZlmWhnqJ_H3Qjl94zIzQ0KJWsdJUh3nfF4SKID8z7pPXa5Z2pIqzIO-MSO-yny0vSYs=s900-c-k-c0x00ffffff-no-rj"
                alt="Karol G performing"
              />
              <div class="card-content">
                <span class="live-badge">LIVE</span>
                <h3>Karol G Performs "Oki Doki"</h3>
                <p class="tags">
                  <span>#Pop</span><span>#Rock</span><span>#Jazz</span
                  ><span>#Salsa</span>
                </p>
                <div class="artist">
                  <span  class="artist-icon">🎧</span> 
                  <span style="color: white;">Karol G</span>
                </div>
              </div>
            </article>

            <article class="card">
              <img
                src="https://media.cnn.com/api/v1/images/stellar/prod/220918125931-post-malone-fall-st-louis-trnd.jpg?c=16x9&q=h_833,w_1480,c_fill"
                alt="Post Malone performing"
              />
              <div class="card-content">
                <span class="live-badge">LIVE</span>
                <h3>Post Malone Rocks the Stage</h3>
                <p class="tags">
                  <span>#HipHop</span><span>#Rap</span><span>#Pop</span
                  ><span>#Rock</span>
                </p>
                <div class="artist">
                  <span class="artist-icon">🎤</span> 
                  <span style="color: white;">Post Malone</span> 
                </div>
              </div>
            </article>

            <article class="card">
              <img
                src="https://aws-modapedia.vogue.es/prod/designs/v1/assets/640x427/1465.jpg"
                alt="Billie Eilish performing"
              />
              <div class="card-content">
                <span class="live-badge">LIVE</span>
                <h3>Billie Eilish Delivers Emotional Performance</h3>
                <p class="tags">
                  <span>#Pop</span><span>#Alternative</span><span>#Indie</span
                  ><span>#Electro</span>
                </p>
                <div class="artist">
                  <span class="artist-icon">🎤</span> 
                  <span style="color: white;">Billie Eilish</span>
                </div>
              </div>
            </article>

            
            <article class="card">
              <img
                src="https://images.seattletimes.com/wp-content/uploads/2023/07/07222023_swift_213100.jpg?d=2040x1479"
                alt="Taylor Swift performing"
              />
              <div class="card-content">
                <span class="live-badge">LIVE</span>
                <h3>Taylor Swift's Spectacular Show</h3>
                <p class="tags">
                  <span>#Country</span><span>#Pop</span><span>#Folk</span
                  ><span>#Indie</span>
                </p>
                <div class="artist">
                  <span class="artist-icon">🎸</span>
                  <span style="color: white;" > Taylor Swift</span>
                </div>
              </div>
            </article>
          </div>
        </div>

        <div class="carousel-dots">
          <span class="dot active"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          
        </div>
      </div>
    </section>

    <!-- aca se acaba el carrucel -->

    <!-- parte 3 -->
    <div class="klipwall-container">
      <h1 class="ui header" style="color: #f2f2f2">KlipWall</h1>
      <div class="klipwall-post-box">
        <img
          src="https://xstore.8theme.com/elementor/demos/book-store/wp-content/uploads/sites/78/2022/05/Eleanor-Pena.jpeg"
          alt="User Avatar"
          class="user-avatar"
        />
        <textarea
          class="post-input"
          placeholder="What are you thinking?"
        ></textarea>
      </div>
      <div class="preview-container"></div>
      <div class="expanded-options">
        <div class="left-options">
          <button class="add-button" id="image-upload-btn">
            <i class="fas fa-image"></i>
          </button>
          <input
            type="file"
            id="image-upload"
            accept="image/*"
            style="display: none"
          />
          <button class="add-button" id="video-upload-btn">
            <i class="fas fa-video"></i>
          </button>
          <input
            type="file"
            id="video-upload"
            accept="video/*"
            style="display: none"
          />
          <button class="add-button" id="audio-upload-btn">
            <i class="fas fa-microphone"></i>
          </button>
          <input
            type="file"
            id="audio-upload"
            accept="audio/*"
            style="display: none"
          />
          <button id="edit-image-btn" class="add-button" style="display: none">
            <i class="fas fa-edit"></i> Editar Imagen
          </button>
          <button
            id="confirm-crop-btn"
            class="add-button"
            style="display: none"
          >
            <i class="fas fa-check"></i> Confirmar Recorte
          </button>
        </div>
        <div class="right-options">
          <select class="privacy-select">
            <option value="public">Público</option>
            <option value="friends">Amigos</option>
            <option value="only-me">Solo yo</option>
          </select>
          <button class="post-button" id="post-btn">Post</button>
          <button class="cancel-icon-button" id="cancel-btn">&times;</button>
        </div>
      </div>
    </div>

    <!-- Mover el div de publicaciones aquí abajo -->
    <div class="posts-container">
      <!-- Aquí se insertarán las publicaciones -->
    </div>
    <!-- Scripts -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/cropperjs/1.5.12/cropper.min.js"></script>
    <script>
      const postInput = document.querySelector(".post-input");
      const expandedOptions = document.querySelector(".expanded-options");
      const previewContainer = document.querySelector(".preview-container");
      const imageUploadInput = document.getElementById("image-upload");
      const videoUploadInput = document.getElementById("video-upload");
      const audioUploadInput = document.getElementById("audio-upload");
      const postButton = document.getElementById("post-btn");
      const editImageButton = document.getElementById("edit-image-btn");
      const confirmCropButton = document.getElementById("confirm-crop-btn");
      let cropperInstance; 
      const maxImages = 4; // Número máximo de imágenes permitidas
      let imageCount = 0; // Contador de imágenes actuales

      // Imagen - Usando el botón con el ícono de imagen
      document
        .getElementById("image-upload-btn")
        .addEventListener("click", function () {
          if (imageCount < maxImages) {
            imageUploadInput.click(); // Abre el diálogo de carga de imagen
          } else {
            alert("Has alcanzado el límite máximo de imágenes.");
          }
        });

      imageUploadInput.addEventListener("change", function (event) {
        const file = event.target.files[0];
        if (file) {
          const reader = new FileReader();
          reader.onload = function (e) {
            if (imageCount < maxImages) {
              const imgElement = document.createElement("img");
              imgElement.src = e.target.result;
              imgElement.id = `croppr-image-${imageCount}`;
              imgElement.style.maxWidth = "100%";
              imgElement.style.display = "block";
              previewContainer.innerHTML = ""; 
              previewContainer.appendChild(imgElement);

              // Initialize Cropper.js
              if (cropperInstance) {
                cropperInstance.destroy();
              }
              cropperInstance = new Cropper(imgElement, {
                aspectRatio: 1,
                viewMode: 1,
                autoCropArea: 0.8,
                responsive: true,
                background: false,
              });

              
              confirmCropButton.style.display = "block";

              
              const closeButton = document.createElement("button");
              closeButton.classList.add("close-btn");
              closeButton.innerHTML = "&times;";
              closeButton.addEventListener("click", function () {
                previewContainer.innerHTML = "";
                imageUploadInput.value = ""; 
                editImageButton.style.display = "none"; 
                confirmCropButton.style.display = "none"; 
                if (cropperInstance) cropperInstance.destroy(); 
                imageCount--; 
              });
              previewContainer.appendChild(closeButton);

              imageCount++; 

              if (imageCount >= maxImages) {
                document.getElementById("image-upload-btn").style.display =
                  "none"; 
              }
            }
          };
          reader.readAsDataURL(file);
        }
      });

      // Video
      document
        .getElementById("video-upload-btn")
        .addEventListener("click", function () {
          videoUploadInput.click(); // Abre el diálogo de carga de video
        });

      videoUploadInput.addEventListener("change", function (event) {
        const file = event.target.files[0];
        if (file) {
          const videoElement = document.createElement("video");
          videoElement.src = URL.createObjectURL(file);
          videoElement.controls = true;
          previewContainer.innerHTML = ""; 
          previewContainer.appendChild(videoElement);
        }
      });

      // Audio
      document
        .getElementById("audio-upload-btn")
        .addEventListener("click", function () {
          audioUploadInput.click(); // Abre el diálogo de carga de audio
        });

      audioUploadInput.addEventListener("change", function (event) {
        const file = event.target.files[0];
        if (file) {
          const audioElement = document.createElement("audio");
          audioElement.src = URL.createObjectURL(file);
          audioElement.controls = true;
          previewContainer.innerHTML = "";
          previewContainer.appendChild(audioElement);
        }
      });

      postInput.addEventListener("focus", () => {
        postInput.style.height = "100px"; 
        expandedOptions.style.display = "flex"; 
      });

      postInput.addEventListener("blur", () => {
        if (postInput.value === "") {
          postInput.style.height = "40px"; 
          expandedOptions.style.display = "none"; 
        }
      });

      confirmCropButton.addEventListener("click", function () {
        if (cropperInstance) {
          
          const canvas = cropperInstance.getCroppedCanvas();
          canvas.toBlob((blob) => {
            const urlImagen = URL.createObjectURL(blob);

            
            const croppedImgElement = document.createElement("img");
            croppedImgElement.src = urlImagen;
            croppedImgElement.style.maxWidth = "100%";
            croppedImgElement.style.display = "block";

            
            previewContainer.innerHTML = "";
            previewContainer.appendChild(croppedImgElement);

            
            cropperInstance.destroy();
            cropperInstance = null;
            confirmCropButton.style.display = "none";
            editImageButton.style.display = "none";
          });
        } else {
          alert("No hay imagen para recortar.");
        }
      });

      postButton.addEventListener("click", function () {
        const postContent = postInput.value.trim();
        if (!postContent && !previewContainer.innerHTML) {
          alert("No hay contenido para publicar.");
          return;
        }

        const postContainer = document.querySelector(".posts-container");
        const newPost = document.createElement("div");
        newPost.classList.add("post");

        // Crear el contenido de la publicación
        const postHeader = `
              <div class="post-header">
                  <img src="https://xstore.8theme.com/elementor/demos/book-store/wp-content/uploads/sites/78/2022/05/Eleanor-Pena.jpeg" alt="User Avatar" class="user-avatar" />
                  <div class="post-info">
                      <span class="user-name">Eleanor Pena</span>
                      <span class="post-time">Hace 1 minuto</span>
                      <span class="post-privacy"><i class="fas fa-globe"></i></span>
                  </div>
              </div>
          `;
        const postText = `<div class="post-text">${postContent}</div>`;
        newPost.innerHTML = postHeader + postText;

        // Agregar imágenes si hay disponibles
        const imgElement = previewContainer.querySelector("img");
        if (imgElement) {
          const imgClone = imgElement.cloneNode(true);
          imgClone.style.maxWidth = "100%";
          const postImages = document.createElement("div");
          postImages.classList.add("post-images");
          postImages.appendChild(imgClone);
          newPost.appendChild(postImages);
        }

        // Agregar videos si hay disponibles
        const videoElement = previewContainer.querySelector("video");
        if (videoElement) {
          const videoClone = videoElement.cloneNode(true);
          videoClone.controls = true;
          const postVideo = document.createElement("div");
          postVideo.classList.add("post-media");
          postVideo.appendChild(videoClone);
          newPost.appendChild(postVideo);
        }

        // Agregar audios si hay disponibles
        const audioElement = previewContainer.querySelector("audio");
        if (audioElement) {
          const audioClone = audioElement.cloneNode(true);
          audioClone.controls = true;
          const postAudio = document.createElement("div");
          postAudio.classList.add("post-media");
          postAudio.appendChild(audioClone);
          newPost.appendChild(postAudio);
        }

        postContainer.appendChild(newPost);

        // Reset inputs
        postInput.value = "";
        previewContainer.innerHTML = "";
        imageUploadInput.value = "";
        videoUploadInput.value = "";
        audioUploadInput.value = "";
        editImageButton.style.display = "none";
        confirmCropButton.style.display = "none";
        imageCount = 0;
        document.getElementById("image-upload-btn").style.display =
          "inline-block";
        alert("Publicación realizada con éxito!");
      });
    </script>
    <script>
      document
        .getElementById("cancel-btn")
        .addEventListener("click", function () {
          // Restablecer la entrada de texto
          postInput.value = "";
          postInput.style.height = "40px"; // Colapsar el textarea
          expandedOptions.style.display = "none"; // Ocultar opciones adicionales

          // Restablecer la vista previa de imágenes y otros elementos
          previewContainer.innerHTML = "";
          imageUploadInput.value = ""; // Limpiar entrada de archivo
          imageCount = 0; // Reiniciar contador de imágenes
          document.getElementById("add-image-btn").style.display =
            "inline-block"; // Mostrar botón de añadir imagen

          // Restablecer la instancia de Cropper si existe
          if (cropperInstance) {
            cropperInstance.destroy();
            cropperInstance = null;
          }

          // Ocultar botones de edición y confirmación
          editImageButton.style.display = "none";
          confirmCropButton.style.display = "none";
        });
    </script>

    <script>
      const carousel = document.querySelector(".carousel");
      const dots = document.querySelectorAll(".dot");
      let currentIndex = 0;

      function showSlide(index) {
        const cardWidth = document.querySelector(".card").offsetWidth + 20; 
        carousel.style.transform = `translateX(-${index * cardWidth}px)`;

        
        dots.forEach((dot) => dot.classList.remove("active"));

        
        dots[index].classList.add("active");
      }

      dots.forEach((dot, index) => {
        dot.addEventListener("click", () => {
          currentIndex = index;
          showSlide(currentIndex);
        });
      });

      
      showSlide(currentIndex);
    </script>
  </body>
</html>
