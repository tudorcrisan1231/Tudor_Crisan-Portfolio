<template>
<div class="container">
  <div class="container_mobile">
      <div class="container_nav_mobile">
        <div class="nav_list_about" @click="goTo('about') + mobileNavItemsClose()"><div></div><div>ABOUT</div></div>
        <div class="nav_list_projects" @click="goTo('projects') + mobileNavItemsClose()"><div></div><div>PROJECTS</div></div>
        <div class="nav_list_contact" @click="goTo('contact') + mobileNavItemsClose()"><div></div><div>CONTACT</div></div>
      </div>
  </div>
  <div class="container_first" ref="home">
    <nav class="nav">
      <div class="nav_logo" @click="goTo('home') + mobileNavItemsClose()">
        <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img"  width="4em"  height="4em" preserveAspectRatio="xMidYMid meet"  viewBox="0 0 24 24"><path d="M9 7h6v2h-2v8h-2V9H9V7M5 3h14a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2m0 2v14h14V5H5z" fill="#020826"/></svg>
      </div>
      <div class="nav_list">
        <div class="nav_list_home" @click="goTo('home')">HOME</div>
        <div class="nav_list_about" @click="goTo('about')">ABOUT</div>
        <div class="nav_list_projects" @click="goTo('projects')">PROJECTS</div>
        <div class="nav_list_contact" @click="goTo('contact')">CONTACT</div>
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
        <h3 style="margin-bottom: 1rem;">Front-end developer / Freelacencer</h3>
        
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
  <div class="container_about" ref="about">
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
        <p data-aos="fade-up">The main area I work in is front end development(client-side of the web).</p>
        <p data-aos="fade-up">Technologies that I worked with: </p>
        <div class="aboutMe_icons" data-aos="fade-up">
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path fill="#e44f26" d="M5.902 27.201L3.655 2h24.69l-2.25 25.197L15.985 30L5.902 27.201z"/><path fill="#f1662a" d="M16 27.858l8.17-2.265l1.922-21.532H16v23.797z"/><path fill="#ebebeb" d="M16 13.407h-4.09l-.282-3.165H16V7.151H8.25l.074.83l.759 8.517H16v-3.091z"/><path fill="#ebebeb" d="M16 21.434l-.014.004l-3.442-.929l-.22-2.465H9.221l.433 4.852l6.332 1.758l.014-.004v-3.216z"/><path fill="#fff" d="M15.989 13.407v3.091h3.806l-.358 4.009l-3.448.93v3.216l6.337-1.757l.046-.522l.726-8.137l.076-.83H15.989z"/><path fill="#fff" d="M15.989 7.151V10.242h7.466l.062-.694l.141-1.567l.074-.83h-7.743z"/></svg> HTML</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path d="M16 2A14 14 0 1 1 2 16A14 14 0 0 1 16 2z" fill="#c69" fill-rule="evenodd"/><path d="M24.782 7.992c-.634-2.486-4.757-3.3-8.659-1.918a19.605 19.605 0 0 0-6.644 3.811c-2.149 2.01-2.492 3.76-2.351 4.491c.5 2.58 4.033 4.266 5.486 5.517v.007c-.428.211-3.564 1.8-4.3 3.42c-.774 1.712.123 2.94.718 3.105A4.4 4.4 0 0 0 13.78 24.5a4.824 4.824 0 0 0 .472-4.288a5.639 5.639 0 0 1 2.143-.123c2.456.287 2.938 1.82 2.846 2.462a1.62 1.62 0 0 1-.779 1.1c-.172.107-.225.143-.21.223c.021.115.1.111.247.086a1.915 1.915 0 0 0 1.336-1.707c.059-1.5-1.382-3.186-3.934-3.143a6.736 6.736 0 0 0-2.189.3a5.844 5.844 0 0 0-.108-.12c-1.578-1.683-4.494-2.874-4.371-5.137c.045-.823.331-2.989 5.6-5.617c4.32-2.153 7.778-1.56 8.376-.247c.854 1.876-1.848 5.361-6.334 5.864a3.37 3.37 0 0 1-2.833-.718c-.236-.26-.271-.271-.359-.223c-.143.079-.052.309 0 .445a2.659 2.659 0 0 0 1.621 1.274a8.592 8.592 0 0 0 5.258-.52c2.721-1.049 4.843-3.974 4.22-6.419zM13.218 20.663a3.584 3.584 0 0 1-.029 2.092q-.035.106-.077.21t-.091.2a3.911 3.911 0 0 1-.647.943c-.813.887-1.95 1.223-2.437.94c-.526-.305-.263-1.556.68-2.553a9.478 9.478 0 0 1 2.474-1.762z" fill="#fff"/></svg> SCSS</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none" fill-rule="evenodd"><path fill="#F1DC50" d="M0 0h24v24H0z"/><path stroke="#333" stroke-width="2" d="M12 11v8c0 .876-.523 2-2 2c-2.385 0-2.5-2-2.5-2m13.29-5.484c-.6-1.01-1.396-1.516-2.386-1.516C16.856 12 16 13 16 14s.5 2 2.508 2.5c1.278.318 2.492 1 2.492 2.5s-1.315 2-2.5 2c-1.514 0-2.514-.667-3-2"/></g></svg> JS</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path d="M24.4 3.925H30l-14 24.15L2 3.925h10.71l3.29 5.6l3.22-5.6z" fill="#41b883"/><path d="M2 3.925l14 24.15l14-24.15h-5.6L16 18.415L7.53 3.925z" fill="#41b883"/><path d="M7.53 3.925L16 18.485l8.4-14.56h-5.18L16 9.525l-3.29-5.6z" fill="#35495e"/></svg> VUE.JS</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="0.89em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 256 289"><path d="M128 288.464c-3.975 0-7.685-1.06-11.13-2.915l-35.247-20.936c-5.3-2.915-2.65-3.975-1.06-4.505c7.155-2.385 8.48-2.915 15.9-7.156c.796-.53 1.856-.265 2.65.265l27.032 16.166c1.06.53 2.385.53 3.18 0l105.74-61.217c1.06-.53 1.59-1.59 1.59-2.915V83.08c0-1.325-.53-2.385-1.59-2.915l-105.74-60.953c-1.06-.53-2.385-.53-3.18 0L20.405 80.166c-1.06.53-1.59 1.855-1.59 2.915v122.17c0 1.06.53 2.385 1.59 2.915l28.887 16.695c15.636 7.95 25.44-1.325 25.44-10.6V93.68c0-1.59 1.326-3.18 3.181-3.18h13.516c1.59 0 3.18 1.325 3.18 3.18v120.58c0 20.936-11.396 33.126-31.272 33.126c-6.095 0-10.865 0-24.38-6.625l-27.827-15.9C4.24 220.885 0 213.465 0 205.515V83.346C0 75.396 4.24 67.976 11.13 64L116.87 2.783c6.625-3.71 15.635-3.71 22.26 0L244.87 64C251.76 67.975 256 75.395 256 83.346v122.17c0 7.95-4.24 15.37-11.13 19.345L139.13 286.08c-3.445 1.59-7.42 2.385-11.13 2.385zm32.596-84.009c-46.377 0-55.917-21.2-55.917-39.221c0-1.59 1.325-3.18 3.18-3.18h13.78c1.59 0 2.916 1.06 2.916 2.65c2.12 14.045 8.215 20.936 36.306 20.936c22.261 0 31.802-5.035 31.802-16.96c0-6.891-2.65-11.926-37.367-15.372c-28.886-2.915-46.907-9.275-46.907-32.33c0-21.467 18.02-34.187 48.232-34.187c33.921 0 50.617 11.66 52.737 37.101c0 .795-.265 1.59-.795 2.385c-.53.53-1.325 1.06-2.12 1.06h-13.78c-1.326 0-2.65-1.06-2.916-2.385c-3.18-14.575-11.395-19.345-33.126-19.345c-24.38 0-27.296 8.48-27.296 14.84c0 7.686 3.445 10.07 36.306 14.31c32.597 4.24 47.967 10.336 47.967 33.127c-.265 23.321-19.345 36.571-53.002 36.571z" fill="#539E43"/></svg> NODE.JS</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path fill="#1572b6" d="M5.902 27.201L3.656 2h24.688l-2.249 25.197L15.985 30L5.902 27.201z"/><path fill="#33a9dc" d="M16 27.858l8.17-2.265l1.922-21.532H16v23.797z"/><path fill="#fff" d="M16 13.191h4.09l.282-3.165H16V6.935h7.75l-.074.829l-.759 8.518H16v-3.091z"/><path fill="#ebebeb" d="M16.019 21.218l-.014.004l-3.442-.93l-.22-2.465H9.24l.433 4.853l6.331 1.758l.015-.004v-3.216z"/><path fill="#fff" d="M19.827 16.151l-.372 4.139l-3.447.93v3.216l6.336-1.756l.047-.522l.537-6.007h-3.101z"/><path fill="#ebebeb" d="M16.011 6.935v3.091H8.545l-.062-.695l-.141-1.567l-.074-.829h7.743z"/><path fill="#ebebeb" d="M16 13.191v3.091H12.601l-.062-.695l-.14-1.567l-.074-.829H16z"/></svg> CSS</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="1em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 256 256"><path d="M251.172 116.594L139.4 4.828c-6.433-6.437-16.873-6.437-23.314 0l-23.21 23.21l29.443 29.443c6.842-2.312 14.688-.761 20.142 4.693c5.48 5.489 7.02 13.402 4.652 20.266l28.375 28.376c6.865-2.365 14.786-.835 20.269 4.657c7.663 7.66 7.663 20.075 0 27.74c-7.665 7.666-20.08 7.666-27.749 0c-5.764-5.77-7.188-14.235-4.27-21.336l-26.462-26.462l-.003 69.637a19.82 19.82 0 0 1 5.188 3.71c7.663 7.66 7.663 20.076 0 27.747c-7.665 7.662-20.086 7.662-27.74 0c-7.663-7.671-7.663-20.086 0-27.746a19.654 19.654 0 0 1 6.421-4.281V94.196a19.378 19.378 0 0 1-6.421-4.281c-5.806-5.798-7.202-14.317-4.227-21.446L81.47 39.442l-76.64 76.635c-6.44 6.443-6.44 16.884 0 23.322l111.774 111.768c6.435 6.438 16.873 6.438 23.316 0l111.251-111.249c6.438-6.44 6.438-16.887 0-23.324" fill="#DE4C36"/></svg> GIT</p>
          <p class="code"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" width="0.9em" height="1em" preserveAspectRatio="xMidYMid meet" viewBox="0 0 460 512"><path d="M156.483 498.57c-28.154 26.468-77.292 11.408-108.562-24.176C6.4 427.148-8.631 337.668 4.754 257.873l151.729 240.696zm32.732-30.512c-18.228-7.747-91.458-45.553-62.463-179.76C80.302 257.764 13.644 234.8 9.378 229.82c0 0 .174 8.073-1.962 23.902l157.637 235.35c3.916-7.718 14.3-13.878 24.162-21.014zm-49.786-79.579c15.543 51.182 43.043 57.232 63.315 69.89L408.585 17.992h2.435L219.913 472.995c19.381 18.274 45.235 36.647 84.038 27.902C463.908 472.324 500.428 214.25 413.902 0C312.147 69.794 235.998 107.428 186.32 181.314c-38.638 57.467-68.612 138.396-46.891 207.165z" fill="currentColor"/></svg> Leaflet</p>
        </div>
        <button class="main-text_btn" @click="goTo('projects')" data-aos="fade-up">View projects</button>
      </div>
      <div class="aboutMe_lottie" data-aos="fade-down">
        <!--<lottie-player src="https://assets3.lottiefiles.com/packages/lf20_jrd2vhow.json"  background="transparent"  speed="1"  loop autoplay></lottie-player>-->
        <lottie-player class="invers" src="https://assets5.lottiefiles.com/packages/lf20_QOeRfb.json"  background="transparent"  speed="1" loop autoplay></lottie-player>
      </div>
    </div>

  </div>
  <div class="container_projects" ref="projects">
    <h1 class="main-text_title projects_title" data-aos="fade-down">Some Things I’ve Built</h1>
    <div v-for="i in this.projects" :key="i.id" class='projects' :data-aos="i.id%2!=0 ? 'fade-up-right' : 'fade-up-left'" data-aos-duration="700">
      <div :class="[i.id%2!=0 ? 'projects_text_right': 'projects_text_left', 'projects_text']" >
        <h3 :class="[i.id%2!=0 ? 'projects_name_right': 'projects_name_left', 'projects_name']">{{i.name}}</h3>
        <p class="projects_description">{{i.description}}</p>
        <div :class="[i.id%2!=0 ? 'projects_code_right': 'projects_code_left', 'projects_code']">
          <p v-for="j in i.code" :key="j" style="margin-right:1.5rem; text-align: right;">{{j}}</p>
        </div>
        <div :class="[i.id%2!=0 ? 'projects_icons_right': 'projects_icons_left', 'projects_icons']">
          <a :href='i.link[0]' target="_blank" style="text-decoration:none; color:inherit;" title="GitHub repository"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g stroke-width="1.5" fill="none"><path d="M16 22.027v-2.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7a5.44 5.44 0 0 0-1.5-3.75a5.07 5.07 0 0 0-.09-3.77s-1.18-.35-3.91 1.48a13.38 13.38 0 0 0-7 0c-2.73-1.83-3.91-1.48-3.91-1.48A5.07 5.07 0 0 0 5 5.797a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7a3.37 3.37 0 0 0-.94 2.58v2.87" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"/><path d="M9 20.027c-3 .973-5.5 0-7-3" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"/></g></svg></a>
          <a :href='i.link[1]' target="_blank" style="text-decoration:none;color:inherit;" title="Live Demo"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path d="M17.001 20h-11a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2h4v2h-4v11h11v-4h2v4a2 2 0 0 1-2 2zm-5.3-6.293l-1.41-1.414L16.584 6h-3.583V4h7v7h-2V7.415l-6.3 6.292z" fill="currentColor"/></g></svg></a>
        </div>
      </div>
      <a :href='i.link[1]' target="_blank"  :class="[i.id%2==0 ? 'projects_imgContainer_right': 'projects_imgContainer_left', 'projects_imgContainer']">
        <img :src="i.image" alt="image" class="projects_img">
        <div class="layer"></div>
      </a>
    </div>

    <h3 class="main-text_title projects_title" style="font-size:2.5rem; padding:6rem 0 3rem 0;" data-aos="fade-up">Other Noteworthy Projects</h3>
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
      <button class="main-text_btn mini_projects_btn" @click="showMore()" ref="view_projects" data-aos="fade-up">Show more</button>    
    </div>
    

  </div>
  <div class="container_contact" ref="contact">
    <h1 class="main-text_title" style="text-align:center;" data-aos="fade-up">Let's work together!</h1>
    <form action="https://formsubmit.co/crisantudor79@yahoo.com" method="POST" class="contact">
      <h3 class="contact_title" data-aos="fade-up">Contact me</h3>
      <input type="text" placeholder="Enter Name" required class="contact_name" name="name" data-aos="fade-up">
      <input type="email" placeholder="Enter a VALID Email" required class="contact_email" name="email" data-aos="fade-up">
      <textarea cols="30" rows="10" class="contact_text" required placeholder="Type Message" name="message" data-aos="fade-up"></textarea>
      <input type="hidden" name="_autoresponse" value="Thank you for contacting me, I'll come with a message as fast as I can!✌️">
      <div class="contact_send">
        <button type="submit" class="main-text_btn" data-aos="fade-up">Send message</button>
      </div>
      <h3 class="contact_title">or</h3>
      <div class="main-text_social" style="justify-content:center;" data-aos="fade-up">
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
    <p>Copyright 2021 &copy;</p>
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

export default {
  name: "App",
  components: {},

  data() {
    const projects = [
        {
          id: '1',
          name: 'LOLStatsV2',
          description: "A stats traker for 'League of legends'. View your match history, rank, level, champions mastery / chest earned, quick overview about your recent matches, live game statistics, advanced data for every game, builds, runes, MVP. Latest LOL news, patch notes, free to play champion rotation and a lot more. Live view unavailable until I receive an authorized API_KEY.",
          code: ['HTML', 'SCSS', 'JS','NODE.JS', 'Riot_API','DDragon'],
          image: require('./assets/lol.png'),
          link: ['https://github.com/tudorcrisan1231/LOLStatsV2','https://www.youtube.com/watch?v=UbXbkygYTt8']
        },
        {
          id: '2',
          name: 'Vito Food',
          description: 'A web app where you can search for a vast variety of food. View ingredients, cooking time, select how many servings do you want. Add your own recipe or bookmark an existing one.',
          code: ['HTML', 'SCSS', 'JS', 'Forkify_API', 'Parcel'],
          image: require('./assets/food.png'), //trebuie pus require cand pun ceva link din assets
          link: ['https://github.com/tudorcrisan1231/vito-food','https://vito-food.netlify.app/']
        },
        {
          id: '3',
          name: 'Chaty',
          description: 'A real-time, all in one chat app where you can communicate with people all over the world.',
          code: ['HTML', 'SCSS', 'VUE.JS', 'FireBase'],
          image: require('./assets/chatt.png'),
          link: ['https://github.com/tudorcrisan1231/chaty-tudor','https://chaty-tudor.netlify.app/']
        },
        {
          id: '4',
          name: 'Mapty',
          description: 'A web app where you can plan your travels / activities, assing them on the map with other customizations',
          code: ['HTML', 'SCSS', 'JS', 'Leaflet_Library'],
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
        name: 'Password generator',
        description: "A web app that generate strong passwords, you can select the length of the password or generate a new random one.",
        code: ['HTML', 'CSS', 'JS'],
        link: ['https://github.com/tudorcrisan1231/Projects/tree/main/password%20generator','https://password-generator-tudor.netlify.app']
      },
      {
        id: '4',
        name: 'Bankist',
        description: "A landing page for a fictional bank.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/bankist','https://bankist-tudor.netlify.app']
      },
      {
        id: '5',
        name: 'Natours',
        description: "A landing page for a fictional company that organizes nature travels.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/natours-tudor','https://natours-tudor.netlify.app']
      },
      {
        id: '6',
        name: 'Weather App',
        description: "Search for any city in the world and find the live weather or for the next 3 days. (Live view is not available because the data provider doesn't exist anymore)",
        code: ['HTML', 'CSS', 'JS'],
        link: ['https://github.com/tudorcrisan1231/weather-app-tudor','#']
      },
    ]
    const mini_projects2 = [
      {
        id: '7',
        name: 'Trillo',
        description: "A landing page for a fictional booking company.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/trillo-tudor','https://trillo-tudor.netlify.app']
      },
      {
        id: '8',
        name: 'Ping Game',
        description: "A simple dice game that you can play with a friend, first who scores 100 points win if a dice falls on 1 your unsaved score is reset.",
        code: ['HTML', 'CSS', 'JS'],
        link: ['https://github.com/tudorcrisan1231/Projects/tree/main/joc%20ping','https://ping-game-tudor.netlify.app']
      },
      {
        id: '9',
        name: 'Music App',
        description: "A tap music app where you can play creating your own music.",
        code: ['HTML', 'SCSS'],
        link: ['https://github.com/tudorcrisan1231/Projects/tree/main/music%20app','https://music-app-tudor.netlify.app/']
      },
    ]
    return {
      projects,
      mini_projects,
      mini_projects2,
      show: false,
      isOpen: false,
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
        console.log('da');
      } else{
        document.querySelector('.mobile_open').style.display='block';
        document.querySelector('.mobile_close').style.display='none';
        document.querySelector('.container_mobile').style.marginRight = "-100%";
        //document.querySelector('.container_mobile').style.display='block';

        this.isOpen = false;
        console.log('nu');
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

  },


};
</script>

<style lang="scss">
  @import "./style/style.scss";
</style>
