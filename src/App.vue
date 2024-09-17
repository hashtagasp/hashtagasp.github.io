<script setup>
import {ref} from "vue";

const showZimmer = ref(false)

const showRG24= ref(false)

const showButton= ref(false)

const showContainer= ref(false)

const showID23= ref(false)

const showBenz= ref(false)

const showTRAKA= ref(false)

const showRGA23= ref(false)

const showDTF= ref(false)

const showKDW24= ref(false)

const showDEVEDW= ref(false)

const showJourFixe= ref(false)

const showID24= ref(false)

const showLS24= ref(false)

const showMAD= ref(false)

const showVita= ref(true)

</script>

<template>
  <header>
    <div class="titleSec">
      <p class="titleP"></p>
      <h1 class="titleH1" v-if="showVita">BAREIS+NICOLAUS<br>PRAKTIKUM [
        <button class="titelBtnActive">PORTFOLIO</button>
        & <button class="titelBtnUnActive" @click="showVita=false">CV</button>  ]
      </h1>
      <h1 class="titleH1" v-if="!showVita">BAREIS+NICOLAUS<br>PRAKTIKUM [
        <button class="titelBtnUnActive" @click="showVita=true">PORTFOLIO</button>
        & <button class="titelBtnActive">CV</button>  ]
      </h1>
    </div>
  </header>
  <main>
    <!--
    <div class="navSec">
      <p class="navP">...</p>
      <p class="navP-Btn">
        <button class="navBtn"><span class="dot"></span> LATEST</button>
        <button class="navBtn"><span class="dot"></span> ADOBE CC</button>
        <button class="navBtn"><span class="dot"></span> MOTION</button>
        <button class="navBtn"><span class="dot"></span> CODING</button>
        <button class="navBtn"><span class="dot"></span> FUN</button>&ensp;|&ensp;
        <button class="navBtn"><span class="dot"></span> VITA</button>
      </p>
    </div> -->
    <!-- Vita -->
    <div class="contentSec" v-if="!showVita">
      <p class="contentPB-White">&emsp;</p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White"><h2>Short CV: </h2></button>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Contri">
              <p class="contentP">Programms:</p>
            </div>
            <div class="contentP-Btn-White">
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE CC</button>
              <button class="contentBtn-White"><span class="dot-White"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-White"><span class="dot-White"></span> CAVALRY</button>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> HTML</button>
              <button class="contentBtn-White"><span class="dot-White"></span> CSS</button>
              <button class="contentBtn-White"><span class="dot-White"></span> VUE.JS</button>
              <button class="contentBtn-White"><span class="dot-White"></span> PYTHON</button>
              <button class="contentBtn-White"><span class="dot-White"></span> PROCESSING</button>
              <button class="contentBtn-White"><span class="dot-White"></span> BLENDER</button>
            </div>

            <div class="contentP-Btn-Contri">
              <p class="contentP"><br>Skills:</p>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> PRINT MEDIA</button>
              <button class="contentBtn-White"><span class="dot-White"></span> DIGITAL MEDIA</button>
              <button class="contentBtn-White"><span class="dot-White"></span> VIDEO MEDIA</button>
              <button class="contentBtn-White"><span class="dot-White"></span> CODING</button>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> LEARNING PROGRAMMS FAST</button>
            </div>

            <div class="contentP-Btn-Contri">
              <p class="contentP"><br>Schools:</p>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> 2015-2018 HAUCHLER STUDIO - APPRENTICESHIP GRAFIK DESIGN</button>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> 2018-2019 HDM STUTTGART - COMPUTER SCIENCE(MEDIA)</button>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> 2019-2021 ABK STUTTGART - FINE ARTS</button>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span> 2021-ON GOING ABK STUTTGART - COMMUNICATION DESIGN</button>
            </div>

            <div class="contentP-Btn-Contri">
              <p class="contentP"><br>Contact:</p>
            </div>
            <div class="contentP-Btn-Contri">
              <button class="contentBtn-White"><span class="dot-White"></span>CHRISTIAN.MUELLER2@STUD.ABK-STUTTGART.DE</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Zimmerservice -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showZimmer"><button class="contentLeft-White" @click="showZimmer= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showZimmer"><button class="contentLeft-White" @click="showZimmer= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showZimmer" @click="showZimmer = true"><h2>Zimmerservice</h2><h3> &ensp;[Poster & Motion]</h3></button>
          <button class="htwo-White" v-if="showZimmer" @click="showZimmer = false"><h2>Zimmerservice</h2><h3> &ensp;[Poster & Motion]</h3></button>
          <div class="contentVideo" v-if="showZimmer">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/zimmerservice.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> CAVALRY</button>
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE AI</button>
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE ID</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showZimmer">
              <button class="contentBtn-White">@JONAS HERMANN</button>
            </div>
            <div class="contentP-Btn-White" v-if="showZimmer">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showZimmer" @click="showZimmer = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showZimmer" @click="showZimmer = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- ABK Rundgang CI 2024 -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showRG24"><button @click="showRG24 = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showRG24"><button @click="showRG24 = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showRG24" @click="showRG24 = true"><h2>ABK Rundgang 2024</h2><h3> &ensp;[CI & Motion]</h3></button>
          <button class="htwo-Black" v-if="showRG24" @click="showRG24 = false"><h2>ABK Rundgang 2024</h2><h3> &ensp;[CI & Motion]</h3></button>
          <div class="contentVideo" v-if="showRG24">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/RG24_Web.mp4" type="video/mp4">
            </video>
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/RG24_Gray.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> CAVALRY</button>
              <button class="contentBtn-Black"><span class="dot"></span> BLENDER</button>
              <button class="contentBtn-Black"><span class="dot"></span> ADOBE AI</button>
              <button class="contentBtn-Black"><span class="dot"></span> ADOBE CC</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showRG24">
              <button class="contentBtn-Black">@ALEYNA KOHL</button>
              <button class="contentBtn-Black">@MARYNA ZEVAKO</button>
              <button class="contentBtn-Black">@MAJKEN BÖCKMANN</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showRG24">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showRG24"><button  class="contentBtn-Open-B" @click="showRG24 = false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showRG24"><button  class="contentBtn-Open-B" @click="showRG24 = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Push The Button-->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showButton"><button class="contentLeft-White" @click="showButton= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showButton"><button class="contentLeft-White" @click="showButton= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showButton" @click="showButton = true"><h2>Push The Button</h2><h3>&ensp;[Coding & Motion]</h3></button>
          <button class="htwo-White" v-if="showButton" @click="showButton = false"><h2>Push The Button</h2><h3>&ensp;[Coding & Motion]</h3></button>
          <div class="contentVideo" v-if="showButton">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/PTB.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE AE</button>
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE AI</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showButton">
              <button class="contentBtn-White">@LILIAN HUTCHINSON</button>
              <button class="contentBtn-White">@NICK STÄBLER</button>
              <button class="contentBtn-White">@TIM FRITZSCHE</button>
            </div>
            <div class="contentP-Btn-White" v-if="showButton">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showButton" @click="showButton = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showButton" @click="showButton = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Container City -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showContainer"><button @click="showContainer = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showContainer"><button @click="showContainer = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showContainer" @click="showContainer = true"><h2>Container City</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <button class="htwo-Black" v-if="showContainer" @click="showContainer = false"><h2>Container City</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <div class="contentVideo" v-if="showContainer">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/CC01.mp4" type="video/mp4">
            </video>
          </div>
          <div class="contentVideo" v-if="showContainer">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/CC02.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-Black"><span class="dot"></span> RESOLUME ARENA</button>
              <button class="contentBtn-Black"><span class="dot"></span> CAVALRY</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showContainer">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showContainer"><button  class="contentBtn-Open-B" @click="showContainer= false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showContainer"><button  class="contentBtn-Open-B" @click="showContainer = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Interdisciplinary Week -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showID23"><button class="contentLeft-White" @click="showID23= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showID23"><button class="contentLeft-White" @click="showID23= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showID23" @click="showID23 = true"><h2>Interdisciplinary Week 2023</h2><h3>&ensp;[CI & Motion]</h3></button>
          <button class="htwo-White" v-if="showID23" @click="showID23 = false"><h2>Interdisciplinary Week 2023</h2><h3>&ensp;[CI & Motion]</h3></button>
          <div class="contentVideo" v-if="showID23">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/IDW23.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE ID</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showID23">
              <button class="contentBtn-White">@ELISABETH SPENGLER CASTILLO</button>
            </div>
            <div class="contentP-Btn-White" v-if="showID23">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showID23" @click="showID23 = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showID23" @click="showID23 = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>


    <!-- Workshops 2024 -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showKDW24"><button @click="showKDW24 = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showKDW24"><button @click="showKDW24 = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showKDW24" @click="showKDW24 = true"><h2>KD Workshops 2024</h2><h3>&ensp;[Poster]</h3></button>
          <button class="htwo-Black" v-if="showKDW24" @click="showKDW24 = false"><h2>KD Workshops 2024</h2><h3>&ensp;[Poster]</h3></button>
          <div class="contentVideo" v-if="showKDW24">

            <img src="./assets/KDW24.png" height="auto" width="100%"/></div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-Black"><span class="dot"></span> BLENDER</button>
              <button class="contentBtn-Black"><span class="dot"></span> ADOBE ID</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showKDW24">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showKDW24"><button  class="contentBtn-Open-B" @click="showKDW24 = false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showKDW24"><button  class="contentBtn-Open-B" @click="showKDW24 = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- TRAKA -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showTRAKA"><button class="contentLeft-White" @click="showTRAKA= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showTRAKA"><button class="contentLeft-White" @click="showTRAKA= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showTRAKA" @click="showTRAKA = true"><h2>TRAKA Nikolausparty</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <button class="htwo-White" v-if="showTRAKA" @click="showTRAKA = false"><h2>TRAKA Nikolausparty</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <div class="contentVideo" v-if="showTRAKA">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/TRAKA.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span>RESOLUME ARENA</button>
              <button class="contentBtn-White"><span class="dot-White"></span>TOUCHDESIGNER</button>
              <button class="contentBtn-White"><span class="dot-White"></span>BLENDER</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showTRAKA">
              <button class="contentBtn-White">@ABK LICHT LICHT</button>
            </div>
            <div class="contentP-Btn-White" v-if="showTRAKA">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showTRAKA" @click="showTRAKA = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showTRAKA" @click="showTRAKA = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Rundgang Afterparty 2023-->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showRGA23"><button @click="showRGA23 = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showRGA23"><button @click="showRGA23 = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showRGA23" @click="showRGA23 = true"><h2>Rundgang Afterparty 2023</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <button class="htwo-Black" v-if="showRGA23" @click="showRGA23 = false"><h2>Rundgang Afterparty 2023</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <div class="contentVideo" v-if="showRGA23">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/RGA23.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-Black"><span class="dot"></span> CAVALRY</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showRGA23">
              <button class="contentBtn-Black">@ABK LICHT LICHT</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showRGA23">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showRGA23"><button  class="contentBtn-Open-B" @click="showRGA23 = false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showRGA23"><button  class="contentBtn-Open-B" @click="showRGA23 = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Down to Fuck -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showDTF"><button class="contentLeft-White" @click="showDTF= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showDTF"><button class="contentLeft-White" @click="showDTF= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showDTF" @click="showDTF = true"><h2>Down to F*ck</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <button class="htwo-White" v-if="showDTF" @click="showDTF = false"><h2>Down to F*ck</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <div class="contentVideo" v-if="showDTF">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/DTF.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> TOUCHDESIGNER</button>
            </div>
            <div class="contentP-Btn-White" v-if="showDTF">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showDTF" @click="showDTF = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showDTF" @click="showDTF = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Mercedes Benz -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showBenz"><button @click="showBenz = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showBenz"><button @click="showBenz = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showBenz" @click="showBenz = true"><h2>Mercedes Benz Museum</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <button class="htwo-Black" v-if="showBenz" @click="showBenz = false"><h2>Mercedes Benz Museum</h2><h3>&ensp;[VJ & Visuals]</h3></button>
          <div class="contentVideo" v-if="showBenz">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/benz01.mp4" type="video/mp4">
            </video>
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/benz02.mp4" type="video/mp4">
            </video>
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/benz03.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> RESOLUME ARENA</button>
              <button class="contentBtn-Black"><span class="dot"></span> TOUCHDESIGNER</button>
              <button class="contentBtn-Black"><span class="dot"></span> CAVALRY</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showBenz">
              <button class="contentBtn-Black">@LILIAN HUTCHINSON</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showBenz">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showBenz"><button  class="contentBtn-Open-B" @click="showBenz = false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showBenz"><button  class="contentBtn-Open-B" @click="showBenz = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- DEVEDW -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showDEVEDW"><button class="contentLeft-White" @click="showDEVEDW= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showDEVEDW"><button class="contentLeft-White" @click="showDEVEDW= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showDEVEDW" @click="showDEVEDW = true"><h2>DEVEDW</h2><h3>&ensp;[unrealised Poster]</h3></button>
          <button class="htwo-White" v-if="showDEVEDW" @click="showDEVEDW = false"><h2>DEVEDW</h2><h3>&ensp;[unrealised Poster]</h3></button>
          <div class="contentVideo" v-if="showDEVEDW">
            <img src="./assets/Filmposter_01.png" height="auto" width="100%"/></div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE PS</button>
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE ID</button>
            </div>
            <div class="contentP-Btn-White" v-if="showDEVEDW">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showDEVEDW" @click="showDEVEDW = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showDEVEDW" @click="showDEVEDW = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Jour Fixe -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showJourFixe"><button @click="showJourFixe = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showJourFixe"><button @click="showJourFixe = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showJourFixe" @click="showJourFixe = true"><h2>Jour Fixe</h2><h3>&ensp;[unrealised Poster & Motion]</h3></button>
          <button class="htwo-Black" v-if="showJourFixe" @click="showJourFixe = false"><h2>Jour Fixe</h2><h3>&ensp;[unrealised Poster & Motion]</h3></button>
          <div class="contentVideo" v-if="showJourFixe">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/JF.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> ADOBE ID</button>
              <button class="contentBtn-Black"><span class="dot"></span> BLENDER</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showJourFixe">
              <button class="contentBtn-Black"><span class="dot"></span> MARKUS BADER</button>
              <button class="contentBtn-Black"><span class="dot"></span> BLANCA WILL</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showJourFixe">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showJourFixe"><button  class="contentBtn-Open-B" @click="showJourFixe = false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showJourFixe"><button  class="contentBtn-Open-B" @click="showJourFixe = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Interdiscilipnary Week 2024 -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showID24"><button class="contentLeft-White" @click="showID24= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showID24"><button class="contentLeft-White" @click="showID24= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showID24" @click="showID24 = true"><h2>Interdisciplinary Week 2024</h2><h3>&ensp;[In Progress]</h3></button>
          <button class="htwo-White" v-if="showID24" @click="showID24 = false"><h2>Interdisciplinary Week 2024</h2><h3>&ensp;[In Progress]</h3></button>
          <div class="contentVideo" v-if="showID24">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/IDW24.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE ID</button>
              <button class="contentBtn-White"><span class="dot-White"></span> CAVALRY</button>
              <button class="contentBtn-White"><span class="dot-White"></span> TOUCHDESIGNER</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showID24">
              <button class="contentBtn-White">@ELISABETH SPENGLER CASTILLO</button>
            </div>
            <div class="contentP-Btn-White" v-if="showID24">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showID24" @click="showID24 = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showID24" @click="showID24 = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- Light-System Workshops -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-Black" v-if="!showLS24"><button @click="showLS24 = true" class="contentLeft-Black">&emsp;</button></p>
      <p class="contentPB-Black" v-if="showLS24"><button @click="showLS24 = false" class="contentLeft-Black">&emsp;</button></p>
      <div class="contentCard-Black">
        <div class="contentTitle">
          <button class="htwo-Black" v-if="!showLS24" @click="showLS24 = true"><h2>Light-System Workshops</h2><h3>&ensp;[In Progress]</h3></button>
          <button class="htwo-Black" v-if="showLS24" @click="showLS24 = false"><h2>Light-System Workshops</h2><h3>&ensp;[In Progress]</h3></button>
          <div class="contentVideo" v-if="showLS24">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/LSW_1.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-Black"><span class="dot"></span> ADOBE ID</button>
              <button class="contentBtn-Black"><span class="dot"></span> CAVALRY</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showLS24">
              <button class="contentBtn-Black"><span class="dot"></span> LILIAN HUTCHINSON</button>
              <button class="contentBtn-Black"><span class="dot"></span> ABK LICHT LICHT</button>
            </div>
            <div class="contentP-Btn-Black">
              <p class="contentP" v-if="showLS24">Hallo</p>
            </div>
          </div>
          <div class="contentOpen" v-if="showLS24"><button  class="contentBtn-Open-B" @click="showLS24 = false" >CLOSE</button></div>
          <div class="contentOpen" v-if="!showLS24"><button  class="contentBtn-Open-B" @click="showLS24 = true" >OPEN</button></div>
        </div>
      </div>
    </div>

    <!-- MAD Lab -->
    <div class="contentSec" v-if="showVita">
      <p class="contentPB-White" v-if="!showMAD"><button class="contentLeft-White" @click="showMAD= true" >&emsp;</button></p>
      <p class="contentPB-White" v-if="showMAD"><button class="contentLeft-White" @click="showMAD= false">&emsp;</button></p>
      <div class="contentCard-White">
        <div class="contentTitle">
          <button class="htwo-White" v-if="!showMAD" @click="showMAD = true"><h2>MAD Lab CI</h2><h3>&ensp;[In Progress]</h3></button>
          <button class="htwo-White" v-if="showMAD" @click="showMAD = false"><h2>MAD Lab CI</h2><h3>&ensp;[In Progress]</h3></button>
          <div class="contentVideo" v-if="showMAD">
            <video height="auto" width="100%" controls muted autoplay loop>
              <source src="./assets/MAD.mp4" type="video/mp4">
            </video>
          </div>
        </div>
        <div class="contentHeader">
          <div>
            <div class="contentP-Btn-Programme">
              <button class="contentBtn-White"><span class="dot-White"></span> ADOBE CC</button>
              <button class="contentBtn-White"><span class="dot-White"></span> WORDPRESS</button>
            </div>
            <div class="contentP-Btn-Contri" v-if="showMAD">
              <button class="contentBtn-White">@MIRIAM HÄFELE</button>
              <button class="contentBtn-White">@FRANZISKA BRENNER</button>
            </div>
            <div class="contentP-Btn-White" v-if="showMAD">
              <p class="contentP">Hallo
              </p>
            </div>
          </div>
          <div class="contentOpen" v-if="showMAD" @click="showMAD = false"><button class="contentBtn-Open-W">CLOSE</button></div>
          <div class="contentOpen" v-if="!showMAD" @click="showMAD = true"><button class="contentBtn-Open-W">OPEN</button></div>
        </div>
      </div>
    </div>





  </main>
</template>

<style scoped>

</style>
