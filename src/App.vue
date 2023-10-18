<template>
<div class="container">
  <div class="container_mobile">
      <div class="container_nav_mobile">
        <a href="#about" class="nav_list_about" @click="mobileNavItemsClose()"><div></div><div>ABOUT</div></a>
        <a href="#projects" class="nav_list_projects" @click="mobileNavItemsClose()"><div></div><div>PROJECTS</div></a>
        <a href="#contact" class="nav_list_contact" @click="mobileNavItemsClose()"><div></div><div>CONTACT</div></a>
      </div>
  </div>
  <div class="container_first" id="home">
    <nav class="nav">
      <a href="#home" class="nav_logo" @click="mobileNavItemsClose()">
        <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img"  width="4em"  height="4em" preserveAspectRatio="xMidYMid meet"  viewBox="0 0 24 24"><path d="M9 7h6v2h-2v8h-2V9H9V7M5 3h14a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2m0 2v14h14V5H5z" fill="#020826"/></svg>
      </a>
      <div class="nav_list">
        <a href="#home" class="nav_list_home">HOME</a>
        <a href="#about" class="nav_list_about">ABOUT</a>
        <a href="#projects" class="nav_list_projects">PROJECTS</a>
        <a href="#contact" class="nav_list_contact">CONTACT</a>
      </div>
      <div class="nav_list_mobile">
        <div class="nav_list_mobile_items" @click="mobileNav()">
          <svg class="mobile_open" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="none"><path d="M2 3.75A.75.75 0 0 1 2.75 3h10.5a.75.75 0 0 1 0 1.5H2.75A.75.75 0 0 1 2 3.75zm0 4A.75.75 0 0 1 2.75 7h10.5a.75.75 0 0 1 0 1.5H2.75A.75.75 0 0 1 2 7.75zm0 4a.75.75 0 0 1 .75-.75h10.5a.75.75 0 0 1 0 1.5H2.75a.75.75 0 0 1-.75-.75z" fill="currentColor"/></g></svg>
          <svg class="mobile_close" style="display:none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path d="M24 9.4L22.6 8L16 14.6L9.4 8L8 9.4l6.6 6.6L8 22.6L9.4 24l6.6-6.6l6.6 6.6l1.4-1.4l-6.6-6.6L24 9.4z" fill="currentColor"/></svg>
        </div>
      </div>
    </nav>
    <div class="main" data-aos="zoom-in">
      <div class="main-text">
        <h2 class="main-text_title">Hello,</h2>
        <h1 class="main-text_title">I'm Tudor,</h1>
        <h1 class="main-text_title">Web Developer!</h1>
        <h3 style="margin-bottom: 1rem;">Full Stack developer / Freelacencer</h3>
        
        <button class="main-text_btn" @click="goTo('projects')">View projects</button>
        <div class="main-text_social">
          <p><a href="https://github.com/tudorcrisan1231" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385c.6.105.825-.255.825-.57c0-.285-.015-1.23-.015-2.235c-3.015.555-3.795-.735-4.035-1.41c-.135-.345-.72-1.41-1.23-1.695c-.42-.225-1.02-.78-.015-.795c.945-.015 1.62.87 1.845 1.23c1.08 1.815 2.805 1.305 3.495.99c.105-.78.42-1.305.765-1.605c-2.67-.3-5.46-1.335-5.46-5.925c0-1.305.465-2.385 1.23-3.225c-.12-.3-.54-1.53.12-3.18c0 0 1.005-.315 3.3 1.23c.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23c.66 1.65.24 2.88.12 3.18c.765.84 1.23 1.905 1.23 3.225c0 4.605-2.805 5.625-5.475 5.925c.435.375.81 1.095.81 2.22c0 1.605-.015 2.895-.015 3.3c0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z" fill="currentColor"/></g></svg></a></p>
          <p><a href="https://www.linkedin.com/in/tudor-crisan-3ba77a202/" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M1 2.838A1.838 1.838 0 0 1 2.838 1H21.16A1.837 1.837 0 0 1 23 2.838V21.16A1.838 1.838 0 0 1 21.161 23H2.838A1.838 1.838 0 0 1 1 21.161V2.838zm8.708 6.55h2.979v1.496c.43-.86 1.53-1.634 3.183-1.634c3.169 0 3.92 1.713 3.92 4.856v5.822h-3.207v-5.106c0-1.79-.43-2.8-1.522-2.8c-1.515 0-2.145 1.089-2.145 2.8v5.106H9.708V9.388zm-5.5 10.403h3.208V9.25H4.208v10.54zM7.875 5.812a2.063 2.063 0 1 1-4.125 0a2.063 2.063 0 0 1 4.125 0z" fill="currentColor"/></g></svg></a></p>
          <p><a href="mailto:crisantudor79@yahoo.com" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 36 36"><path class="clr-i-solid clr-i-solid-path-1" d="M32.33 6a2 2 0 0 0-.41 0h-28a2 2 0 0 0-.53.08l14.45 14.39z" fill="currentColor"/><path class="clr-i-solid clr-i-solid-path-2" d="M33.81 7.39l-14.56 14.5a2 2 0 0 1-2.82 0L2 7.5a2 2 0 0 0-.07.5v20a2 2 0 0 0 2 2h28a2 2 0 0 0 2-2V8a2 2 0 0 0-.12-.61zM5.3 28H3.91v-1.43l7.27-7.21l1.41 1.41zm26.61 0h-1.4l-7.29-7.23l1.41-1.41l7.27 7.21z" fill="currentColor"/></svg></a></p>
          <p><a href="https://www.facebook.com/tudor.crisan.9" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M0 12.067C0 18.033 4.333 22.994 10 24v-8.667H7V12h3V9.333c0-3 1.933-4.666 4.667-4.666c.866 0 1.8.133 2.666.266V8H15.8c-1.467 0-1.8.733-1.8 1.667V12h3.2l-.533 3.333H14V24c5.667-1.006 10-5.966 10-11.933C24 5.43 18.6 0 12 0S0 5.43 0 12.067z" fill="currentColor"/></g></svg></a></p>
          <p><a href="https://www.instagram.com/tudor_crisan1231/" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 1024 1024"><path d="M512 378.7c-73.4 0-133.3 59.9-133.3 133.3S438.6 645.3 512 645.3S645.3 585.4 645.3 512S585.4 378.7 512 378.7zM911.8 512c0-55.2.5-109.9-2.6-165c-3.1-64-17.7-120.8-64.5-167.6c-46.9-46.9-103.6-61.4-167.6-64.5c-55.2-3.1-109.9-2.6-165-2.6c-55.2 0-109.9-.5-165 2.6c-64 3.1-120.8 17.7-167.6 64.5C132.6 226.3 118.1 283 115 347c-3.1 55.2-2.6 109.9-2.6 165s-.5 109.9 2.6 165c3.1 64 17.7 120.8 64.5 167.6c46.9 46.9 103.6 61.4 167.6 64.5c55.2 3.1 109.9 2.6 165 2.6c55.2 0 109.9.5 165-2.6c64-3.1 120.8-17.7 167.6-64.5c46.9-46.9 61.4-103.6 64.5-167.6c3.2-55.1 2.6-109.8 2.6-165zM512 717.1c-113.5 0-205.1-91.6-205.1-205.1S398.5 306.9 512 306.9S717.1 398.5 717.1 512S625.5 717.1 512 717.1zm213.5-370.7c-26.5 0-47.9-21.4-47.9-47.9s21.4-47.9 47.9-47.9s47.9 21.4 47.9 47.9a47.84 47.84 0 0 1-47.9 47.9z" fill="currentColor"/></svg></a></p>
        </div>
      </div>

      <div class="main-img" data-aos="zoom-in">
        <!--<lottie-player class="main-lottie1" src="https://assets1.lottiefiles.com/private_files/lf30_tfozcvfo.json"  background="transparent"  speed="1"  style="width: 700px; height:700px;"  loop autoplay v-if="randomNr()<5"></lottie-player>-->
        <lottie-player
          class="main-lottie"
          src="https://assets6.lottiefiles.com/packages/lf20_mragdxra.json"
          background="transparent"
          speed="1"
          loop
          autoplay
        ></lottie-player>
      </div>
    </div>
    <lottie-player
      class="background_lottie_up"
      src="https://assets10.lottiefiles.com/packages/lf20_az79wvq6.json"
      background="transparent"
      speed="1"
      loop
      autoplay
    ></lottie-player>
    <lottie-player
      class="background_lottie_down"
      src="https://assets3.lottiefiles.com/packages/lf20_k19adj4e.json"
      background="transparent"
      speed="1"
      loop
      autoplay
    ></lottie-player>
  </div>
  <div class="container_about" id="about">
    <lottie-player
      class="background_lottie_up invert"
      src="https://assets10.lottiefiles.com/packages/lf20_az79wvq6.json"
      background="transparent"
      speed="1"
      loop
      autoplay
    ></lottie-player>
    <div class="aboutMe">
      <div class="aboutMe_text">
        <h1 class="main-text_title" data-aos="fade-up">About</h1>
        <p data-aos="fade-up">Strongly motivated web developer with a passion for the computer world in general. Open to learn new things anytime, problem solver, a well-organized person with high attention to detail, knowing how to divide his time efficiently. Fan of video games, outdoor activities, and books reading.</p>
       
        <h3 style="color:#020826" data-aos="fade-up">Skills and Experience</h3>
        <p data-aos="fade-up">The main area I work in is front-end development (client-side of the web), but I also work on back-end development (server-side of the web).</p>
        <p data-aos="fade-up">Technologies that I worked with: </p>
        <div class="aboutMe_icons" data-aos="fade-up">
          <div class="aboutMe_icons_left">
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path fill="#e44f26" d="M5.902 27.201L3.655 2h24.69l-2.25 25.197L15.985 30L5.902 27.201z"/><path fill="#f1662a" d="M16 27.858l8.17-2.265l1.922-21.532H16v23.797z"/><path fill="#ebebeb" d="M16 13.407h-4.09l-.282-3.165H16V7.151H8.25l.074.83l.759 8.517H16v-3.091z"/><path fill="#ebebeb" d="M16 21.434l-.014.004l-3.442-.929l-.22-2.465H9.221l.433 4.852l6.332 1.758l.014-.004v-3.216z"/><path fill="#fff" d="M15.989 13.407v3.091h3.806l-.358 4.009l-3.448.93v3.216l6.337-1.757l.046-.522l.726-8.137l.076-.83H15.989z"/><path fill="#fff" d="M15.989 7.151V10.242h7.466l.062-.694l.141-1.567l.074-.83h-7.743z"/></svg> HTML</p>
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path fill="#1572b6" d="M5.902 27.201L3.656 2h24.688l-2.249 25.197L15.985 30L5.902 27.201z"/><path fill="#33a9dc" d="M16 27.858l8.17-2.265l1.922-21.532H16v23.797z"/><path fill="#fff" d="M16 13.191h4.09l.282-3.165H16V6.935h7.75l-.074.829l-.759 8.518H16v-3.091z"/><path fill="#ebebeb" d="M16.019 21.218l-.014.004l-3.442-.93l-.22-2.465H9.24l.433 4.853l6.331 1.758l.015-.004v-3.216z"/><path fill="#fff" d="M19.827 16.151l-.372 4.139l-3.447.93v3.216l6.336-1.756l.047-.522l.537-6.007h-3.101z"/><path fill="#ebebeb" d="M16.011 6.935v3.091H8.545l-.062-.695l-.141-1.567l-.074-.829h7.743z"/><path fill="#ebebeb" d="M16 13.191v3.091H12.601l-.062-.695l-.14-1.567l-.074-.829H16z"/></svg> CSS</p>
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path d="M16 2A14 14 0 1 1 2 16A14 14 0 0 1 16 2z" fill="#c69" fill-rule="evenodd"/><path d="M24.782 7.992c-.634-2.486-4.757-3.3-8.659-1.918a19.605 19.605 0 0 0-6.644 3.811c-2.149 2.01-2.492 3.76-2.351 4.491c.5 2.58 4.033 4.266 5.486 5.517v.007c-.428.211-3.564 1.8-4.3 3.42c-.774 1.712.123 2.94.718 3.105A4.4 4.4 0 0 0 13.78 24.5a4.824 4.824 0 0 0 .472-4.288a5.639 5.639 0 0 1 2.143-.123c2.456.287 2.938 1.82 2.846 2.462a1.62 1.62 0 0 1-.779 1.1c-.172.107-.225.143-.21.223c.021.115.1.111.247.086a1.915 1.915 0 0 0 1.336-1.707c.059-1.5-1.382-3.186-3.934-3.143a6.736 6.736 0 0 0-2.189.3a5.844 5.844 0 0 0-.108-.12c-1.578-1.683-4.494-2.874-4.371-5.137c.045-.823.331-2.989 5.6-5.617c4.32-2.153 7.778-1.56 8.376-.247c.854 1.876-1.848 5.361-6.334 5.864a3.37 3.37 0 0 1-2.833-.718c-.236-.26-.271-.271-.359-.223c-.143.079-.052.309 0 .445a2.659 2.659 0 0 0 1.621 1.274a8.592 8.592 0 0 0 5.258-.52c2.721-1.049 4.843-3.974 4.22-6.419zM13.218 20.663a3.584 3.584 0 0 1-.029 2.092q-.035.106-.077.21t-.091.2a3.911 3.911 0 0 1-.647.943c-.813.887-1.95 1.223-2.437.94c-.526-.305-.263-1.556.68-2.553a9.478 9.478 0 0 1 2.474-1.762z" fill="#fff"/></svg> SCSS</p>
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none" fill-rule="evenodd"><path fill="#F1DC50" d="M0 0h24v24H0z"/><path stroke="#333" stroke-width="2" d="M12 11v8c0 .876-.523 2-2 2c-2.385 0-2.5-2-2.5-2m13.29-5.484c-.6-1.01-1.396-1.516-2.386-1.516C16.856 12 16 13 16 14s.5 2 2.508 2.5c1.278.318 2.492 1 2.492 2.5s-1.315 2-2.5 2c-1.514 0-2.514-.667-3-2"/></g></svg> JS</p>
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path d="M24.4 3.925H30l-14 24.15L2 3.925h10.71l3.29 5.6l3.22-5.6z" fill="#41b883"/><path d="M2 3.925l14 24.15l14-24.15h-5.6L16 18.415L7.53 3.925z" fill="#41b883"/><path d="M7.53 3.925L16 18.485l8.4-14.56h-5.18L16 9.525l-3.29-5.6z" fill="#35495e"/></svg> VUE.JS</p>
            
          </div>
          <div class="aboutMe_icons_right">
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 256 256"><path d="M251.172 116.594L139.4 4.828c-6.433-6.437-16.873-6.437-23.314 0l-23.21 23.21l29.443 29.443c6.842-2.312 14.688-.761 20.142 4.693c5.48 5.489 7.02 13.402 4.652 20.266l28.375 28.376c6.865-2.365 14.786-.835 20.269 4.657c7.663 7.66 7.663 20.075 0 27.74c-7.665 7.666-20.08 7.666-27.749 0c-5.764-5.77-7.188-14.235-4.27-21.336l-26.462-26.462l-.003 69.637a19.82 19.82 0 0 1 5.188 3.71c7.663 7.66 7.663 20.076 0 27.747c-7.665 7.662-20.086 7.662-27.74 0c-7.663-7.671-7.663-20.086 0-27.746a19.654 19.654 0 0 1 6.421-4.281V94.196a19.378 19.378 0 0 1-6.421-4.281c-5.806-5.798-7.202-14.317-4.227-21.446L81.47 39.442l-76.64 76.635c-6.44 6.443-6.44 16.884 0 23.322l111.774 111.768c6.435 6.438 16.873 6.438 23.316 0l111.251-111.249c6.438-6.44 6.438-16.887 0-23.324" fill="#DE4C36"/></svg> GIT</p>
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path fill="#5d87a1" fill-rule="evenodd" d="M8.785 6.865a3.055 3.055 0 0 0-.785.1V7h.038a6.461 6.461 0 0 0 .612.785c.154.306.288.611.441.917l.038-.039a1.074 1.074 0 0 0 .4-.957a4.314 4.314 0 0 1-.23-.4c-.115-.191-.364-.287-.517-.44"/><path fill="#00758f" fill-rule="evenodd" d="M27.78 23.553a8.849 8.849 0 0 0-3.712.536c-.287.115-.745.115-.785.478c.154.153.172.4.307.613a4.467 4.467 0 0 0 .995 1.167c.4.306.8.611 1.225.879c.745.461 1.588.728 2.314 1.187c.422.268.842.612 1.264.9c.21.153.343.4.611.5v-.058a3.844 3.844 0 0 0-.291-.613c-.191-.19-.383-.363-.575-.554a9.118 9.118 0 0 0-1.99-1.932c-.613-.422-1.953-1-2.2-1.7l-.039-.039a7.69 7.69 0 0 0 1.321-.308c.65-.172 1.243-.133 1.912-.3c.307-.077.862-.268.862-.268v-.3c-.342-.34-.587-.795-.947-1.116a25.338 25.338 0 0 0-3.122-2.328c-.587-.379-1.344-.623-1.969-.946c-.226-.114-.6-.17-.737-.36a7.594 7.594 0 0 1-.776-1.457a46.84 46.84 0 0 1-1.551-3.293a20.236 20.236 0 0 0-.965-2.157A19.078 19.078 0 0 0 11.609 5a9.07 9.07 0 0 0-2.421-.776c-.474-.02-.946-.057-1.419-.075a7.55 7.55 0 0 1-.869-.664C5.818 2.8 3.038 1.328 2.242 3.277C1.732 4.508 3 5.718 3.435 6.343A8.866 8.866 0 0 1 4.4 7.762c.133.322.171.663.3 1a22.556 22.556 0 0 0 .987 2.538a8.946 8.946 0 0 0 .7 1.172c.153.209.417.3.474.645a5.421 5.421 0 0 0-.436 1.419a8.336 8.336 0 0 0 .549 6.358c.3.473 1.022 1.514 1.987 1.116c.851-.34.662-1.419.908-2.364c.056-.229.019-.379.132-.53v.184s.483 1.061.723 1.6a10.813 10.813 0 0 0 2.4 2.59A3.514 3.514 0 0 1 14 24.657V25h.427a1.054 1.054 0 0 0-.427-.788a9.4 9.4 0 0 1-.959-1.16a24.992 24.992 0 0 1-2.064-3.519c-.3-.6-.553-1.258-.793-1.857c-.11-.231-.11-.58-.295-.7a7.266 7.266 0 0 0-.884 1.313a11.419 11.419 0 0 0-.517 2.921c-.073.02-.037 0-.073.038c-.589-.155-.792-.792-1.014-1.332a8.756 8.756 0 0 1-.166-5.164c.128-.405.683-1.681.461-2.068c-.111-.369-.48-.58-.682-.871a7.767 7.767 0 0 1-.663-1.237C5.912 9.5 5.69 8.3 5.212 7.216a10.4 10.4 0 0 0-.921-1.489A9.586 9.586 0 0 1 3.276 4.22c-.092-.213-.221-.561-.074-.793a.3.3 0 0 1 .259-.252c.238-.212.921.058 1.16.174a9.2 9.2 0 0 1 1.824.967c.258.194.866.685.866.685h.18c.612.133 1.3.037 1.876.21a12.247 12.247 0 0 1 2.755 1.32a16.981 16.981 0 0 1 5.969 6.545c.23.439.327.842.537 1.3c.4.94.9 1.9 1.3 2.814a12.578 12.578 0 0 0 1.36 2.564c.286.4 1.435.612 1.952.822a13.7 13.7 0 0 1 1.32.535c.651.4 1.3.861 1.913 1.3c.305.23 1.262.708 1.32 1.091"/></svg> MySQL</p>
            <p class="code">
              <svg xmlns="http://www.w3.org/2000/svg" width="0.97em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 256 264"><path fill="#FF2D20" d="M255.856 59.62c.095.351.144.713.144 1.077v56.568c0 1.478-.79 2.843-2.073 3.578L206.45 148.18v54.18a4.135 4.135 0 0 1-2.062 3.579l-99.108 57.053c-.227.128-.474.21-.722.299c-.093.03-.18.087-.278.113a4.15 4.15 0 0 1-2.114 0c-.114-.03-.217-.093-.325-.134c-.227-.083-.464-.155-.68-.278L2.073 205.938A4.128 4.128 0 0 1 0 202.36V32.656c0-.372.052-.733.144-1.083c.031-.119.103-.227.145-.346c.077-.216.15-.438.263-.639c.077-.134.19-.242.283-.366c.119-.165.227-.335.366-.48c.119-.118.274-.206.408-.309c.15-.124.283-.258.453-.356h.005L51.613.551a4.135 4.135 0 0 1 4.125 0l49.546 28.526h.01c.165.104.305.232.454.351c.134.103.284.196.402.31c.145.149.248.32.371.484c.088.124.207.232.279.366c.118.206.185.423.268.64c.041.118.113.226.144.35c.095.351.144.714.145 1.078V138.65l41.286-23.773V60.692c0-.36.052-.727.145-1.072c.036-.124.103-.232.144-.35c.083-.217.155-.44.268-.64c.077-.134.19-.242.279-.366c.123-.165.226-.335.37-.48c.12-.118.269-.206.403-.309c.155-.124.289-.258.454-.356h.005l49.551-28.526a4.13 4.13 0 0 1 4.125 0l49.546 28.526c.175.103.309.232.464.35c.128.104.278.197.397.31c.144.15.247.32.37.485c.094.124.207.232.28.366c.118.2.185.423.267.64c.047.118.114.226.145.35Zm-8.115 55.258v-47.04l-17.339 9.981l-23.953 13.792v47.04l41.297-23.773h-.005Zm-49.546 85.095V152.9l-23.562 13.457l-67.281 38.4v47.514l90.843-52.3ZM8.259 39.796v160.177l90.833 52.294v-47.505L51.64 177.906l-.015-.01l-.02-.01c-.16-.093-.295-.227-.444-.34c-.13-.104-.279-.186-.392-.3l-.01-.015c-.134-.129-.227-.289-.34-.433c-.104-.14-.227-.258-.31-.402l-.005-.016c-.093-.154-.15-.34-.217-.515c-.067-.155-.154-.3-.196-.464v-.005c-.051-.196-.061-.403-.082-.604c-.02-.154-.062-.309-.062-.464V63.57L25.598 49.772l-17.339-9.97v-.006ZM53.681 8.893L12.399 32.656l41.272 23.762L94.947 32.65L53.671 8.893h.01Zm21.468 148.298l23.948-13.786V39.796L81.76 49.778L57.805 63.569v103.608l17.344-9.986ZM202.324 36.935l-41.276 23.762l41.276 23.763l41.271-23.768l-41.27-23.757Zm-4.13 54.676l-23.953-13.792l-17.338-9.981v47.04l23.948 13.787l17.344 9.986v-47.04Zm-94.977 106.006l60.543-34.564l30.264-17.272l-41.246-23.747l-47.489 27.34l-43.282 24.918l41.21 23.325Z"/></svg>
              Laravel
            </p>
            <p class="code"><svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><path fill="currentColor" d="M12.001 0C6.174 0 1.448 4.957 1.448 11.072c0 2.09.552 4.042 1.51 5.71c.25.279.544.484.965.484c1.339 0 1.268-2.065 2.607-2.065c1.34 0 1.411 2.065 2.75 2.065c1.34 0 1.266-2.065 2.606-2.065c.584 0 .928.397 1.24.84c-.221-.205-.48-.348-.82-.348c-1.196 0-1.307 1.678-2.201 2.141v4.51a1.657 1.657 0 0 0 3.312 0V16.45c.308.433.647.815 1.22.815c1.34 0 1.267-2.065 2.606-2.065c.465 0 .774.255 1.04.58a1.108 1.108 0 0 0-.43-.088c-1.159 0-1.297 1.574-2.118 2.094v2.436a1.49 1.49 0 0 0 2.98 0V16.37c.324.466.67.894 1.278.894c.796 0 1.093-.728 1.485-1.32a11.48 11.48 0 0 0 1.074-4.873C22.552 4.957 17.828 0 12 0zm-.566 2.877c2.88 0 5.214 2.784 5.214 5.807c0 3.023-1.545 5.15-5.214 5.15c-3.67 0-5.215-2.127-5.215-5.15s2.335-5.807 5.215-5.807zm-1.403 1.66a1.955 2.158 0 0 0-1.955 2.158a1.955 2.158 0 0 0 1.955 2.158a1.955 2.158 0 0 0 1.955-2.158a1.955 2.158 0 0 0-1.955-2.158zm-.326.664a.978.996 0 0 1 .979.996a.978.996 0 0 1-.979.996a.978.996 0 0 1-.977-.996a.978.996 0 0 1 .977-.996zm-2.95 10.492c-1.074 0-1.272 1.355-1.95 1.965v1.782a1.49 1.49 0 0 0 2.98 0v-3.182c-.264-.324-.577-.564-1.03-.564Z"/></svg> Livewire</p>
          </div>
         
          
          
        </div>
        <button class="main-text_btn" @click="goTo('projects')" data-aos="fade-up">View projects</button>
      </div>
      <div class="aboutMe_lottie" data-aos="fade-down">
        <!--<lottie-player src="https://assets3.lottiefiles.com/packages/lf20_jrd2vhow.json"  background="transparent"  speed="1"  loop autoplay></lottie-player>-->
        <lottie-player class="invers" src="https://assets5.lottiefiles.com/packages/lf20_QOeRfb.json"  background="transparent"  speed="1" loop autoplay></lottie-player>
      </div>
    </div>

  </div>
  <div class="container_projects" id="projects">
    <h1 class="main-text_title projects_title" data-aos="fade-down">Some Things I’ve Built</h1>
    <div v-for="i in this.projects" :key="i.id" class='projects' :data-aos="i.id%2!=0 ? 'fade-up-right' : 'fade-up-left'" data-aos-duration="200">
      <div :class="[i.id%2!=0 ? 'projects_text_right': 'projects_text_left', 'projects_text']" >
        <h3 :class="[i.id%2!=0 ? 'projects_name_right': 'projects_name_left', 'projects_name']">{{i.name}}</h3>
        <p class="projects_description">{{i.description}}</p>
        <div :class="[i.id%2!=0 ? 'projects_code_right': 'projects_code_left', 'projects_code']">
          <p v-for="j in i.code" :key="j" style="margin-right:1.5rem; text-align: right;">{{j}}</p>
        </div>
        <div :class="[i.id%2!=0 ? 'projects_icons_right': 'projects_icons_left', 'projects_icons']">
          <a v-if="i.link[0]" :href='i.link[0]' target="_blank" style="text-decoration:none; color:inherit;" title="GitHub repository"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g stroke-width="1.5" fill="none"><path d="M16 22.027v-2.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7a5.44 5.44 0 0 0-1.5-3.75a5.07 5.07 0 0 0-.09-3.77s-1.18-.35-3.91 1.48a13.38 13.38 0 0 0-7 0c-2.73-1.83-3.91-1.48-3.91-1.48A5.07 5.07 0 0 0 5 5.797a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7a3.37 3.37 0 0 0-.94 2.58v2.87" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 20.027c-3 .973-5.5 0-7-3" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"/></g></svg></a>
          <a v-if="i.link[1]" :href='i.link[1]' target="_blank" style="text-decoration:none;color:inherit;" title="Live Demo"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path d="M17.001 20h-11a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2h4v2h-4v11h11v-4h2v4a2 2 0 0 1-2 2zm-5.3-6.293l-1.41-1.414L16.584 6h-3.583V4h7v7h-2V7.415l-6.3 6.292z" fill="currentColor"/></g></svg></a>
        </div>
      </div>
      <a :href='i.link[1]' target="_blank"  :class="[i.id%2==0 ? 'projects_imgContainer_right': 'projects_imgContainer_left', 'projects_imgContainer']">
        <img :src="i.image" alt="image" class="projects_img">
        <div class="layer"></div>
      </a>
    </div>

    <h3 class="main-text_title projects_title" style="font-size:2.5rem; padding:6rem 0 0 0;" data-aos="fade-up">Other Noteworthy Projects</h3>
    <div class="mini_projects_container">
      <div class="mini_projects"  v-for="i in this.mini_projects" :key="i.id" data-aos="fade-down" data-aos-duration="1000">
        <div class="mini_projects_icons">
          <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path d="M22 19V9a2 2 0 0 0-2-2h-6.764a2 2 0 0 1-1.789-1.106l-.894-1.788A2 2 0 0 0 8.763 3H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></g></svg>
          <div>
            <a :href='i.link[0]' target="_blank" style="text-decoration:none; color:inherit;" title="GitHub repository"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g stroke-width="1.5" fill="none"><path d="M16 22.027v-2.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7a5.44 5.44 0 0 0-1.5-3.75a5.07 5.07 0 0 0-.09-3.77s-1.18-.35-3.91 1.48a13.38 13.38 0 0 0-7 0c-2.73-1.83-3.91-1.48-3.91-1.48A5.07 5.07 0 0 0 5 5.797a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7a3.37 3.37 0 0 0-.94 2.58v2.87" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 20.027c-3 .973-5.5 0-7-3" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"/></g></svg></a>
            <a :href='i.link[1]' target="_blank" style="text-decoration:none;color:inherit;" title="Live Demo"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path d="M17.001 20h-11a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2h4v2h-4v11h11v-4h2v4a2 2 0 0 1-2 2zm-5.3-6.293l-1.41-1.414L16.584 6h-3.583V4h7v7h-2V7.415l-6.3 6.292z" fill="currentColor"/></g></svg></a>
          </div>
        </div>

        <p class="mini_projects_name">{{i.name}}</p>
        <p class="mini_projects_description">{{i.description}}</p>
        <div class="mini_projects_code">
          <p v-for="j in i.code" :key="j">#{{j}}</p>
        </div>
      </div>  
      <button v-if="mini_projects2.length != 0" class="main-text_btn mini_projects_btn" @click="showMore()" ref="view_projects" data-aos="fade-up">Show more</button>    
    </div>
    

  </div>
  <div class="container_contact" id="contact">
    <h1 class="main-text_title container_contact_title" style="text-align:center;" data-aos="fade-up">Let's work together!</h1>
    <form @submit.prevent="submitForm" class="contact">
      <h3 class="contact_title">Contact me</h3>
      <input type="text" placeholder="Enter Name" required class="contact_name" name="name" v-model="formData.name">
      <input type="email" placeholder="Enter your Email" required class="contact_email" name="email" v-model="formData.email">
      <textarea cols="30" rows="10" class="contact_text" required placeholder="Type Message" name="message" v-model="formData.message"></textarea>
      <input type="hidden" name="_autoresponse" value="Thank you for contacting me, I'll come with a message as fast as I can!✌️">

      <div v-if="responseMessage.type && responseMessage.message">
        <div v-if="responseMessage.type=='success'">
          <p class="message message_success">{{responseMessage.message}}</p>
        </div>
        <div v-else>
          <p class="message message_error">
            Something went wrong, please try again!
          </p>
        </div>
      </div>

      <div class="contact_send">
        <button type="submit" class="main-text_btn">Send message</button>
      </div>
      <h3 class="contact_title">or</h3>
      <div class="main-text_social" style="justify-content:center;">
          <p><a href="https://github.com/tudorcrisan1231" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385c.6.105.825-.255.825-.57c0-.285-.015-1.23-.015-2.235c-3.015.555-3.795-.735-4.035-1.41c-.135-.345-.72-1.41-1.23-1.695c-.42-.225-1.02-.78-.015-.795c.945-.015 1.62.87 1.845 1.23c1.08 1.815 2.805 1.305 3.495.99c.105-.78.42-1.305.765-1.605c-2.67-.3-5.46-1.335-5.46-5.925c0-1.305.465-2.385 1.23-3.225c-.12-.3-.54-1.53.12-3.18c0 0 1.005-.315 3.3 1.23c.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23c.66 1.65.24 2.88.12 3.18c.765.84 1.23 1.905 1.23 3.225c0 4.605-2.805 5.625-5.475 5.925c.435.375.81 1.095.81 2.22c0 1.605-.015 2.895-.015 3.3c0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z" fill="currentColor"/></g></svg></a></p>
          <p><a href="https://www.linkedin.com/in/tudor-crisan-3ba77a202/" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M1 2.838A1.838 1.838 0 0 1 2.838 1H21.16A1.837 1.837 0 0 1 23 2.838V21.16A1.838 1.838 0 0 1 21.161 23H2.838A1.838 1.838 0 0 1 1 21.161V2.838zm8.708 6.55h2.979v1.496c.43-.86 1.53-1.634 3.183-1.634c3.169 0 3.92 1.713 3.92 4.856v5.822h-3.207v-5.106c0-1.79-.43-2.8-1.522-2.8c-1.515 0-2.145 1.089-2.145 2.8v5.106H9.708V9.388zm-5.5 10.403h3.208V9.25H4.208v10.54zM7.875 5.812a2.063 2.063 0 1 1-4.125 0a2.063 2.063 0 0 1 4.125 0z" fill="currentColor"/></g></svg></a></p>
          <p><a href="mailto:crisantudor79@yahoo.com" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 36 36"><path class="clr-i-solid clr-i-solid-path-1" d="M32.33 6a2 2 0 0 0-.41 0h-28a2 2 0 0 0-.53.08l14.45 14.39z" fill="currentColor"/><path class="clr-i-solid clr-i-solid-path-2" d="M33.81 7.39l-14.56 14.5a2 2 0 0 1-2.82 0L2 7.5a2 2 0 0 0-.07.5v20a2 2 0 0 0 2 2h28a2 2 0 0 0 2-2V8a2 2 0 0 0-.12-.61zM5.3 28H3.91v-1.43l7.27-7.21l1.41 1.41zm26.61 0h-1.4l-7.29-7.23l1.41-1.41l7.27 7.21z" fill="currentColor"/></svg></a></p>
          <p><a href="https://www.facebook.com/tudor.crisan.9" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path fill-rule="evenodd" clip-rule="evenodd" d="M0 12.067C0 18.033 4.333 22.994 10 24v-8.667H7V12h3V9.333c0-3 1.933-4.666 4.667-4.666c.866 0 1.8.133 2.666.266V8H15.8c-1.467 0-1.8.733-1.8 1.667V12h3.2l-.533 3.333H14V24c5.667-1.006 10-5.966 10-11.933C24 5.43 18.6 0 12 0S0 5.43 0 12.067z" fill="currentColor"/></g></svg></a></p>
          <p><a href="https://www.instagram.com/tudor_crisan1231/" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 1024 1024"><path d="M512 378.7c-73.4 0-133.3 59.9-133.3 133.3S438.6 645.3 512 645.3S645.3 585.4 645.3 512S585.4 378.7 512 378.7zM911.8 512c0-55.2.5-109.9-2.6-165c-3.1-64-17.7-120.8-64.5-167.6c-46.9-46.9-103.6-61.4-167.6-64.5c-55.2-3.1-109.9-2.6-165-2.6c-55.2 0-109.9-.5-165 2.6c-64 3.1-120.8 17.7-167.6 64.5C132.6 226.3 118.1 283 115 347c-3.1 55.2-2.6 109.9-2.6 165s-.5 109.9 2.6 165c3.1 64 17.7 120.8 64.5 167.6c46.9 46.9 103.6 61.4 167.6 64.5c55.2 3.1 109.9 2.6 165 2.6c55.2 0 109.9.5 165-2.6c64-3.1 120.8-17.7 167.6-64.5c46.9-46.9 61.4-103.6 64.5-167.6c3.2-55.1 2.6-109.8 2.6-165zM512 717.1c-113.5 0-205.1-91.6-205.1-205.1S398.5 306.9 512 306.9S717.1 398.5 717.1 512S625.5 717.1 512 717.1zm213.5-370.7c-26.5 0-47.9-21.4-47.9-47.9s21.4-47.9 47.9-47.9s47.9 21.4 47.9 47.9a47.84 47.84 0 0 1-47.9 47.9z" fill="currentColor"/></svg></a></p>
        </div>
    </form>
  </div>
  <div class="container_footer">
    <p>Designed and built by Tudor Crișan</p>
    <p>Copyright 2023 &copy;</p>
  </div>
</div>
</template>

<script>
//https://assets3.lottiefiles.com/packages/lf20_bp5lntrf.json
//https://assets8.lottiefiles.com/packages/lf20_8dphtide.json
//https://assets6.lottiefiles.com/packages/lf20_sktdmalw.json
//https://assets1.lottiefiles.com/private_files/lf30_tfozcvfo.json
//https://assets6.lottiefiles.com/packages/lf20_mragdxra.json
//https://assets10.lottiefiles.com/private_files/lf30_sbsvs4ki.json
//https://assets5.lottiefiles.com/packages/lf20_1tnov7hf.json

import AOS from "aos";
import "aos/dist/aos.css";
import axios from 'axios';

export default {
  name: "App",
  components: {},

  data() {

    // API BASED: lolStatsVue  - Vito Food - Mapty
    // only layout: Natours - Trillo - Nexter - Bankist
    // full stack:  managemnetApp,  
    const projects = [
        {
          id: '1',
          name: 'Project Finder',
          description: "Project Finder is a web application that allows beginner developers and not only to find projects based on the technologies they want to learn. Users can create an account, add their preferred technologies, and search for projects based on those choices. They can also create projects. After creating a project, they have multiple functionalities that they can use, such as chat, task management, user management, and more. Also, I have created a dashboard for the administrator.",
          code: ['Laravel', 'Livewire', 'MySQL', 'Tailwind CSS', 'JS'],
          image: require('./assets/project-finder-banner.webp'),
          link: ['','https://prj-finder.tcn-dev.software/']
        },
        {
          id: '2',
          name: 'Chat app',
          description: "This web application is a real-time chat app. Users can create an account, add friends, and chat with them. They can also can create groups and chat with multiple people at the same time. The app also has a report system and a dashboard for the administrator where he can manage users and reports.",
          code: ['Laravel', 'Livewire', 'MySQL', 'Tailwind CSS', 'JS', 'Docker'],
          image: require('./assets/chatapp-banner.webp'),
          link: ['https://github.com/tudorcrisan1231/realTimeChatApp-MAP-project','https://chatapp.tcn-dev.software/login']
        },
        {
          id: '3',
          name: 'ITEC Project',
          description: "This web app which took second place in the ITEC 16th edition competition, streamlines new employee onboarding. Managers have full access to employee profiles, allowing them to create accounts and update onboarding plans. Old Employees are matched with new hires based on skills and experience, creating a seamless onboarding experience. Additional features like email and in-app notifications, chat systems, and translations make the process even smoother. Demo accounts: johndoe@gmail.com / 12345 and maria@maria.ro / 12345",
          code: ['Laravel', 'Livewire', 'MySQL', 'Tailwind CSS', 'JS'],
          image: require('./assets/itec1.png'),
          link: ['https://github.com/tudorcrisan1231/itec_project','https://itec.tudor-crisan.com']
        },
        {
          id: '4',
          name: 'Playground ERP',
          description: "The web application is designed for playground administrators, who can monitor the time spent by customers in the park and calculate the price based on that time. The administrator can set a custom price, and view statistics about their customers. Customers, in this case, are parents with children.",
          code: ['Laravel', 'Livewire', 'MySQL', 'CSS', 'JS'],
          image: require('./assets/playground.png'),
          link: ['','https://playground.tudor-crisan.com']
        },
        {
          id: '5',
          name: 'LOLStatsV2',
          description: "A stats traker for 'League of legends'. View your match history, rank, level, champions mastery / chest earned, quick overview about your recent matches, live game statistics, advanced data for every game, builds, runes, MVP. Latest LOL news, patch notes, free to play champion rotation and a lot more. Live view unavailable until I receive an authorized API_KEY.",
          code: ['HTML', 'SCSS', 'VUE.JS','NODE.JS'],
          image: require('./assets/lol.png'),
          link: ['https://github.com/tudorcrisan1231/LOLStatsV2','https://www.youtube.com/watch?v=UbXbkygYTt8']
        },

        {
          id: '6',
          name: 'Scoala Lupsa',
          description: 'A web app for school news allows users to view the latest news and documents. As an admin, you can add, edit, or delete news and documents.',
          code: ['Laravel', 'Livewire', 'MySQL', 'CSS', 'JS'],
          image: require('./assets/sc_lupsa.png'),
          link: ['','https://sclupsa.ro/']
        },
        {
          id: '7',
          name: 'Hauze',
          description: 'Hauze.ro is a website that helps people connect with a team of specialists in architecture, design and installations, and stay informed about real estate news and trends.',
          code: ['Laravel', 'Livewire', 'MySQL', 'CSS', 'JS'],
          image: require('./assets/hauze.png'),
          link: ['','https://hauze.ro/']
        },
        {
          id: '8',
          name: 'Vito Food',
          description: 'A web app where you can search for a vast variety of food. View ingredients, cooking time, select how many servings do you want. Add your own recipe or bookmark an existing one.',
          code: ['HTML', 'SCSS', 'JS'],
          image: require('./assets/food.png'), //trebuie pus require cand pun ceva link din assets
          link: ['https://github.com/tudorcrisan1231/vito-food','https://vito-food.netlify.app/']
        },
        {
          id: '9',
          name: 'Mapty',
          description: 'A web app where you can plan your travels / activities, assing them on the map with other customizations',
          code: ['HTML', 'SCSS', 'JS'],
          image: require('./assets/mapty.png'),
          link: ['https://github.com/tudorcrisan1231/Projects/tree/main/map%20app','https://mapty-map-app.netlify.app/']
        }
    ]
    const mini_projects = [
      {
        id: '1',
        name: 'Nexter',
        description: "A landing page for a fictional real estate company.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/nexter-tudor','https://nexter-tudor.netlify.app']
      },
      {
        id: '2',
        name: 'Budget Calculator',
        description: "A web budget calculator where you can add your incomes and expenses.",
        code: ['HTML', 'CSS', 'JS'],
        link: ['https://github.com/tudorcrisan1231/Projects/tree/main/BudgetApp','https://budget-calculator-tudor.netlify.app']
      },
      {
        id: '3',
        name: 'Bankist',
        description: "A landing page for a fictional bank.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/bankist','https://bankist-tudor.netlify.app']
      },
      {
        id: '4',
        name: 'Natours',
        description: "A landing page for a fictional company that organizes nature travels.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/natours-tudor','https://natours-tudor.netlify.app']
      },
      {
        id: '5',
        name: 'Trillo',
        description: "A landing page for a fictional booking company.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/trillo-tudor','https://trillo-tudor.netlify.app']
      },
    ]
    const mini_projects2 = [

    ]
    return {
      projects,
      mini_projects,
      mini_projects2,
      show: false,
      isOpen: false,

      formData: {
        name: '',
        email: '',
        message: ''
      },
      responseMessage: {
        status: null,
        message: null
      },
      apiKey: process.env.VUE_APP_API_KEY,
    }
  },

  created() {
    AOS.init();
  },


  methods: {
    randomNr: function () {
      return Math.floor(Math.random() * 5);
    },

    goTo: function(input) {
      var element = this.$refs[input];
      var top = element.offsetTop;

      window.scrollTo(0, top);
    },

    showMore() {
      if(this.show == false) {

        this.mini_projects = [...this.mini_projects, ...this.mini_projects2];
        this.$refs['view_projects'].innerHTML = 'Show less';
        this.show=true;

      } else {

        this.mini_projects.splice(this.mini_projects.length - this.mini_projects2.length, this.mini_projects.length);
        this.$refs['view_projects'].innerHTML = 'Show more';
        this.show=false;

      }

    },

    mobileNav() { 
      if(this.isOpen == false) {
        document.querySelector('.mobile_open').style.display='none';
        document.querySelector('.mobile_close').style.display='block';
        document.querySelector('.container_mobile').style.marginRight = "0";
        //document.querySelector('.container_mobile').style.display = "block";

        this.isOpen = true;
      } else{
        document.querySelector('.mobile_open').style.display='block';
        document.querySelector('.mobile_close').style.display='none';
        document.querySelector('.container_mobile').style.marginRight = "-100%";
        //document.querySelector('.container_mobile').style.display='block';

        this.isOpen = false;
      }
    },
    mobileNavItemsClose() {
      if(this.isOpen == true) {
        document.querySelector('.mobile_open').style.display='block';
        document.querySelector('.mobile_close').style.display='none';
        document.querySelector('.container_mobile').style.marginRight = "-100%";
      }


      this.isOpen = false;
    },


    submitForm() {
      const apiUrl = `https://portofolio-contacts.tcn-dev.software/api/submit-form?key=${this.apiKey}&name=${this.formData.name}&email=${this.formData.email}&message=${this.formData.message}`;

      // Use axios to make a POST request with form data
      axios.post(apiUrl)
        .then(response => {
          this.responseMessage.type = 'success';
          this.responseMessage.message = response.data.message;

          // Reset the form
          this.formData.name = '';
          this.formData.email = '';
          this.formData.message = '';
        })
        .catch(error => {
          this.responseMessage.type = 'error';
          this.responseMessage.message = error;

          // Reset the form
          this.formData.name = '';
          this.formData.email = '';
          this.formData.message = '';
        });
    }
  },


};
</script>

<style lang="scss">
  @import "./style/style.scss";
</style>
