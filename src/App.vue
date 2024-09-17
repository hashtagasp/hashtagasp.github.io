<script setup>
import {ref} from "vue";
const showModal = ref(false)
const showModalClick = ref(false)
const showAll = ref(true)
const showAllText = ref("Show All")

const showPushButton = ref(false)
const showPushButtonClick = ref(false)

const showInterDis = ref(false)
const showInterDisClick = ref(false)

const showFilmPost = ref(false)
const showFilmPostClick = ref(false)

const showJourFixe = ref(false)
const showJourFixeClick = ref(false)

const showKurt = ref(false)
const showKurtClick = ref(false)

const showDTF = ref(false)
const showDTFClick = ref(false)

const showRG23 = ref(false)
const showRG23Click = ref(false)

const showContainer_01 = ref(false)
const showContainerClick_01 = ref(false)

const showContainer_02 = ref(false)
const showContainerClick_02 = ref(false)

const showTruaka = ref(false)
const showTruakaClick = ref(false)

const showRG24 = ref(false)
const showRG24Click = ref(false)

const showMAD = ref(false)
const showMADClick = ref(false)

const showSchwarz = ref(false)
const showSchwarzClick = ref(false)

const showWayToo = ref(false)
const showWayTooClick = ref(false)

</script>

<template>
  <main >
    <div class="scroll-snap">
      <section v-if="false"  >
        <div style="scroll-snap-align: center">
          <img src="../src/assets/01.png" alt="trash" style="width: 100%; height: 100%">
        </div>
      </section>

      <section>
        <div style="display: grid; grid-template-columns: 1fr;">

          <!--<div style="position: absolute;margin: 30px; z-index: 20; grid-row-start: 1; grid-column-start: 1; color: rgba(0,0,0,0); margin-right: 120px">
            <h1>CC13 Cloud → Portfolio → Art Direction & Motion</h1>
            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Mit einem Glückspielautomaten im Kulturkiosk, zogen wir den Leuten das Geld aus der Tasche. Unsere Audiovisuelle Installation:
              <button class="buttonProjekt buttonProjekt2" @mouseover="showModal = true" @mouseleave="showModal = false" @click="showModalClick = true">Push the Button</button>
            </p>
          </div>-->
          <div style="position: absolute;margin: 30px; z-index: 20; grid-row-start: 1; grid-column-start: 1; color: rgba(255,0,0,0); margin-right: 120px">
            <h1>
              C13 Cloud → Art Direction & Motion →
              <button v-if="showAll" @click="showAll = false"  class="buttonProjekt buttonProjektShow" >Show Text</button>
              <button v-if="!showAll" @click="showAll = true"  class="buttonProjekt buttonProjektShow">Show Less</button>
            </h1>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Mit einem Glücksspielautomaten im Kulturkiosk zogen wir den Leuten das Geld aus der Tasche. Unsere audiovisuelle Installation:
              <button class="buttonProjekt buttonProjekt2" @mouseover="showPushButton = true" @mouseleave="showPushButton = false" @click="showPushButtonClick = true">Push the Button</button>,
              mit welcher wir bei der Sammelausstellung: <i>Belohnungszentrum</i> der <i>Klasse Cluss</i> partizpierten,
              umfasst einen eigenständig gebauten, programmierten und animierten Glücksspielautomaten mit einem Hauptgewinn in Form einer selbstgegossen Pokal-Kerze mit Verpackung und einem kleinen Sticker als Trostpreis.
              <button class="buttonProjekt buttonProjekt4">@Lilian Hutchinson</button>
              <button class="buttonProjekt buttonProjekt4">@Nick Stäbler</button>
              <button class="buttonProjekt buttonProjekt4">@Tim Fritzsche</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Cluss</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#After Effects</button>
              <button class="buttonProjekt buttonProjekt4">#Silikon</button>
              <button class="buttonProjekt buttonProjekt4">#Styropor</button>
              <button class="buttonProjekt buttonProjekt4">#Sticker</button>
              <button class="buttonProjekt buttonProjekt4">#Packaging</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Installation</button>
              <button class="buttonProjekt buttonProjekt4">#Audiovisual</button>
            </p> <!-- Push the Button -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showPushButton = true" @mouseleave="showPushButton = false" @click="showPushButtonClick = true">Push the Button</button>
              <button class="buttonProjekt buttonProjekt4">@Lilian Hutchinson</button>
              <button class="buttonProjekt buttonProjekt4">@Nick Stäbler</button>
              <button class="buttonProjekt buttonProjekt4">@Tim Fritzsche</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Cluss</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#After Effects</button>
              <button class="buttonProjekt buttonProjekt4">#Silikon</button>
              <button class="buttonProjekt buttonProjekt4">#Styropor</button>
              <button class="buttonProjekt buttonProjekt4">#Sticker</button>
              <button class="buttonProjekt buttonProjekt4">#Packaging</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Installation</button>
              <button class="buttonProjekt buttonProjekt4">#Audiovisual</button>
            </p> <!-- Less Push the Button -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Neben Halunkereien, zeigt sich mein Informatik-, Kunst- und Design-Hintergrund in illustrierten und animierten Plakatentwürfen.
            </p>
            <p v-if="showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Plakate & Veranstaltungen:
            </p>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Für die <button class="buttonProjekt buttonProjekt2" @mouseover="showInterDis = true" @mouseleave="showInterDis = false" @click="showInterDisClick = true">Interdisziplinäre Woche – Interdisciplinary Week</button>,
              wurden wir dafür ausgewählt interdisziplinäre Vorträge und Workshops zu bewerben, mit dem Schwerpunkt Social Media. Entstanden sind hierfür ein animiertes Poster, Banner und Social Media Formate.
              <button class="buttonProjekt buttonProjekt4">@Elisabeth Spengler Castillo</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Adobe Cloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Social Media</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
            </p> <!-- Interdisziplinär -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showInterDis = true" @mouseleave="showInterDis = false" @click="showInterDisClick=true">Interdisziplinäre Woche – Interdisciplanary Week</button>
              <button class="buttonProjekt buttonProjekt4">@Elisabeth Spengler Castillo</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Adobe Cloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Social Media</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
            </p> <!-- Less Interdisziplinär -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showFilmPost = true" @mouseleave="showFilmPost = false" @click="showFilmPostClick = true">Das Ende vom Ende der Welt (Bild)</button>,
              war ein Filmposter-Projekt, welches als Resultat einer Kooperation zwischen der Filmakademie Wien und der ABK Stuttgart enstand. (not in use)
              <button class="buttonProjekt buttonProjekt4">@Klasse Panholzer</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
            </p> <!-- Filmposter-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showFilmPost = true" @mouseleave="showFilmPost = false" @click="showFilmPostClick = true">Das Ende vom Ende der Welt (Bild)</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Panholzer</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
            </p> <!-- Less Filmposter-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showJourFixe = true" @mouseleave="showJourFixe = false" @click="showJourFixeClick = true">Jour Fixe – Practices of Care</button>,
              ist einr annuale Vortragsreihe an der Akademie, welche Themen wie Architektur, Stadtplanung und Nachhaltigkeit diskutiert. Neben einem Siebdruck-Entwurf auf Kraft Paper, entstand für den Pitch ein animiertes Poster und ein Flyer, welche die Veranstaltung bewerben sollten. (not in use)
              <button class="buttonProjekt buttonProjekt4">@Markus Bader</button>
              <button class="buttonProjekt buttonProjekt4">@Blanca Will</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt4">#Blender</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#Illustrator</button>
              <button class="buttonProjekt buttonProjekt4">#Silkscreen</button>
              <button class="buttonProjekt buttonProjekt4">#Motion Design</button>
              <button class="buttonProjekt buttonProjekt4">#3D</button>
            </p> <!-- Jour Fixe-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showJourFixe = true" @mouseleave="showJourFixe = false" @click="showJourFixeClick = true">Jour Fixe – Practices of Care</button>
              <button class="buttonProjekt buttonProjekt4">@Markus Bader</button>
              <button class="buttonProjekt buttonProjekt4">@Blanca Will</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt4">#Blender</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#Illustrator</button>
              <button class="buttonProjekt buttonProjekt4">#Silkscreen</button>
              <button class="buttonProjekt buttonProjekt4">#Motion Design</button>
              <button class="buttonProjekt buttonProjekt4">#3D</button>
            </p> <!-- Less Jour Fixe-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Als einer der ausgewählten Poster, welche zur Feier für <button class="buttonProjekt buttonProjekt2" @mouseover="showKurt = true" @mouseleave="showKurt = false" @click="showKurtClick = true">Kurt Weidemann 2022</button> im Stadtpalais aushingen, konnte sich dieses animierte Poster dazuzählen.
              <button class="buttonProjekt buttonProjekt4">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#PhotoshopAutomation</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>

            </p> <!-- Kurt-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showKurt = true" @mouseleave="showKurt = false" @click="showKurtClick = true">Kurt Weidemann 2022</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#PhotoshopAutomation</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>

            </p> <!-- Less Kurt-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Durch meine Leidenschaft für Bewegbild und da Social Media Beiträge und Plakate oft zu klein sind, rutschte ich schnell in das Erstellen und Konzipieren von Live-Visuals auf Veranstaltungen und Partys.
            </p>
            <p v-if="showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Live Visuals:
            </p>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showDTF = true" @mouseleave="showDTF = false" @click="showDTFClick = true">Down to F*ck</button>,
              war der erste Auftrag für ein Audioreaktives-Live-Visual, welches ich für die Ausstellung & Afterparty der Klasse Brenner konzipieren durfte.
              <button class="buttonProjekt buttonProjekt4">@Klasse Brenner</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>

            </p> <!-- DTF-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showDTF = true" @mouseleave="showDTF = false" @click="showDTFClick = true">Down to F*ck</button>
              <button class="buttonProjekt buttonProjekt4">@Klasse Brenner</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>

            </p> <!-- Less DTF-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Auf Basis des Rundgang-Design 2023, durften wir die Visuals für die
              <button class="buttonProjekt buttonProjekt2" @mouseover="showRG23 = true" @mouseleave="showRG23 = false" @click="showRG23Click = true">Rundgang Afterparty 2023</button> erstellen, mappen und live mixen.
              <button class="buttonProjekt buttonProjekt4">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt4">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt4">#Cavalry</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>

            </p> <!-- Rundgang 2023 -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showRG23 = true" @mouseleave="showRG23 = false" @click="showRG23Click= true">Rundgang Afterparty 2023</button>
              <button class="buttonProjekt buttonProjekt4">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt4">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt4">#Cavalry</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>

            </p> <!-- Less Rundgang 2023 -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Für die Container City(Neue Oper) wurde ich beauftragt jeweils 2 Veranstaltungen mit Live-Visuals zu bespielen. Zum einen
              <button class="buttonProjekt buttonProjekt2" @mouseover="showContainer_01 = true" @mouseleave="showContainer_01 = false" @click="showContainerClick_01 = true">Container City Afterparty</button> und
              <button class="buttonProjekt buttonProjekt2" @mouseover="showContainer_02 = true" @mouseleave="showContainer_02 = false" @click="showContainerClick_02 = true">lay me next to her bones Afterparty</button>.
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>

            </p> <!-- Container City Festival Afterparty-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showContainer_01 = true" @mouseleave="showContainer_01= false" @click="showContainerClick_01 = true">Container City Afterparty</button>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showContainer_02 = true" @mouseleave="showContainer_02 = false" @click="showContainerClick_02= true">lay me next to her bones Afterparty</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>

            </p> <!-- Less Container City Festival Afterparty-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showTruaka = true" @mouseleave="showTruaka = false" @click="showTruakaClick = true">TRAKA Nikolausparty</button> einfach VRUM VRUM, Pabst Blue Ribbon Beer und Trucks. Mottoparty @AKA.
              <button class="buttonProjekt buttonProjekt4">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt4">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Blender</button>
              <button class="buttonProjekt buttonProjekt4">#AfterEffects</button>
              <button class="buttonProjekt buttonProjekt4">#KI</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>
            </p> <!-- Truaka -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showTruaka = true" @mouseleave="showTruaka = false" @click="showTruakaClick = true">TRAKA Nikolausparty</button>
              <button class="buttonProjekt buttonProjekt4">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt4">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">#Blender</button>
              <button class="buttonProjekt buttonProjekt4">#AfterEffects</button>
              <button class="buttonProjekt buttonProjekt4">#KI</button>
              <button class="buttonProjekt buttonProjekt4">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt4">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt4">#Audioreactive</button>
            </p> <!-- Less Truaka -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Außerdem sind in der Pipeline:
            </p>
            <p v-if="showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Work in Progress:
            </p>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showRG24 = true" @mouseleave="showRG24  = false" @click="showRG24Click = true">Rundgangs Design 2024</button>
              Konzept, CI, Werbemittel(Social Media, Plakate, Flyer Sticker, Merch, Maskottchen). (Release Juni/Juli 2024)
              <button class="buttonProjekt buttonProjekt4">@Maryna Zevako</button>
              <button class="buttonProjekt buttonProjekt4">@Aleyna Kohl</button>
              <button class="buttonProjekt buttonProjekt4">@Majken Böckmann</button>
              <button class="buttonProjekt buttonProjekt4">#Blender</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Mascot</button>
              <button class="buttonProjekt buttonProjekt4">#Rundgang2024</button>
              <button class="buttonProjekt buttonProjekt4">#Cat</button>
            </p> <!-- RG24-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showRG24  = true" @mouseleave="showRG24  = false" @click="showRG24Click = true">Rundgangs Design 2024</button>
              <button class="buttonProjekt buttonProjekt4">@Maryna Zevako</button>
              <button class="buttonProjekt buttonProjekt4">@Aleyna Kohl</button>
              <button class="buttonProjekt buttonProjekt4">@Majken Böckmann</button>
              <button class="buttonProjekt buttonProjekt4">#Blender</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Mascot</button>
              <button class="buttonProjekt buttonProjekt4">#Rundgang2024</button>
              <button class="buttonProjekt buttonProjekt4">#Cat</button>
            </p> <!-- Less RG24-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showMAD = true" @mouseleave="showMAD = false" @click="showMADClick = true">MAD Lab CI</button>
              Branding, Logo, Flyer, Website, Merch. (Release März/April 2024)
              <button class="buttonProjekt buttonProjekt4">@Fraziska Brenner</button>
              <button class="buttonProjekt buttonProjekt4">@Miriam Häfele</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Wordpress</button>
            </p> <!-- MAD LAB-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showMAD = true" @mouseleave="showMAD = false" @click="showMADClick = true">MAD Lab CI</button>
              <button class="buttonProjekt buttonProjekt4">@Fraziska Brenner</button>
              <button class="buttonProjekt buttonProjekt4">@Miriam Häfele</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#Wordpress</button>
            </p> <!-- Less MAD LAB-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showSchwarz = true" @mouseleave="showSchwarz = false" @click="showSchwarzClick = true">Schwarzbrennen (Bild)</button>
              Publikation, Installation. (Release Juli 2024)
              <button class="buttonProjekt buttonProjekt4">@Nick Liebig</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Hefe</button>
              <button class="buttonProjekt buttonProjekt4">#Destillation</button>
              <button class="buttonProjekt buttonProjekt4">#Print</button>
            </p> <!-- Schwarz-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showSchwarz = true" @mouseleave="showSchwarz = false" @click="showSchwarzClick = true">Schwarzbrennen (Bild)</button>
              <button class="buttonProjekt buttonProjekt4">@Nick Liebig</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Hefe</button>
              <button class="buttonProjekt buttonProjekt4">#Destillation</button>
              <button class="buttonProjekt buttonProjekt4">#Print</button>
            </p> <!-- Less Schwarz-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showWayToo = true" @mouseleave="showWayToo = false" @click="showWayTooClick = true">WayTooMuch</button>
              Animation, Live Visuals, Plakat (Release Juni/Juli 2024)
              <button class="buttonProjekt buttonProjekt4">@Florian Siegert</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
            </p> <!-- WayMuch-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt2" @mouseover="showWayToo = true" @mouseleave="showWayToo = false" @click="showWayTooClick = true">WayTooMuch</button>
              <button class="buttonProjekt buttonProjekt4">@Florian Siegert</button>
              <button class="buttonProjekt buttonProjekt4">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt4">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt4">#InDesign</button>
              <button class="buttonProjekt buttonProjekt4">#TouchDesigner</button>
            </p> <!-- Less WayMuch-->

            <p style="font-size: 35px; margin-left: 0px">
              <br>
              Skills, Lebenslauf & Kontakt:
              <br>
            </p>

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Programme:
              <button class="buttonProjekt buttonProjekt4">● Adobe Cloud (PS, ID, AI, XD, PR)</button>
              <button class="buttonProjekt buttonProjekt4">● Blender</button>
              <button class="buttonProjekt buttonProjekt4">● TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt4">● Resolume Arena</button>
              <button class="buttonProjekt buttonProjekt4">● Figma</button>
              <button class="buttonProjekt buttonProjekt4">● HTML</button>
              <button class="buttonProjekt buttonProjekt4">● CSS</button>
              <button class="buttonProjekt buttonProjekt4">● Vue.JS</button>
              <button class="buttonProjekt buttonProjekt4">● Python Scripting</button>
              <button class="buttonProjekt buttonProjekt4">● Processing/p5.js</button>
            </p> <!-- Programme-->

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Skills:
              <button class="buttonProjekt buttonProjekt4">● Print Medien</button>
              <button class="buttonProjekt buttonProjekt4">● Digitale Medien</button>
              <button class="buttonProjekt buttonProjekt4">● Video Medien</button>
              <button class="buttonProjekt buttonProjekt4">● Schnelles lernen von Programmen</button>
              <button class="buttonProjekt buttonProjekt4">● Schnelles verstehen von tech. Abläufen</button>
              <button class="buttonProjekt buttonProjekt4">● Gefühl für Coding</button>
            </p> <!-- Skills-->

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Kurz Vita:
              <button class="buttonProjekt buttonProjekt4">● 2015-2018 Hauchler Studio - Ausbildung Grafik Design</button>
              <button class="buttonProjekt buttonProjekt4">● 2018-2019 Hochschule der Medien - Medieninformatik</button>
              <button class="buttonProjekt buttonProjekt4">● 2019-ongoing Staatl. Akademie der bildenden Künste Stuttgart - Kunst, Kommunikationsdesign</button>
            </p> <!-- Lebi-->

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Kontakt:
              <button class="buttonProjekt buttonProjekt4">@christianmiller.tox</button>
              <button class="buttonProjekt buttonProjekt4">christian.mueller2@abk-stuttgart.de</button></p> <!-- Kontakt-->
            <p><br></p>
          </div>
          <div v-if="showPushButton || showPushButtonClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showPushButtonClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Push the Button-->
          <div v-if="showInterDis || showInterDisClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showInterDisClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Interdisziplinä-->
          <div v-if="showFilmPost || showFilmPostClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showFilmPostClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Film-->
          <div v-if="showJourFixe || showJourFixeClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showJourFixeClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Jour Fixe-->
          <div v-if="showKurt|| showKurtClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showKurtClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Kurt-->
          <div v-if="showDTF || showDTFClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showDTFClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- DTF-->
          <div v-if="showRG23 || showRG23Click" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showRG23Click = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- RG23-->
          <div v-if="showContainer_01 || showContainerClick_01" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showContainerClick_01 = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Container 01-->
          <div v-if="showContainer_02 || showContainerClick_02" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showContainerClick_02= false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Container 02-->
          <div v-if="showTruaka || showTruakaClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showTruakaClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Truaka-->
          <div v-if="showRG24 || showRG24Click" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showRG24Click= false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- RG24-->
          <div v-if="showMAD || showMADClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showMADClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- MAD Lab-->
          <div v-if="showSchwarz || showSchwarzClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showSchwarzClick = false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- Schwarz-->
          <div v-if="showWayToo || showWayTooClick" style="grid-row-start: 1; grid-column-start: 1; position: fixed; right: 0; margin-right: 20px; margin-top: 20px">
            <button @click="showWayTooClick= false" style="border-radius: 50%;" class="button button1" >X</button>
          </div> <!-- WayTooMuch-->
          <!-- Shower-->
          <div v-if="showPushButton || showPushButtonClick" class="middle">
            <video autoplay muted loop preload="auto">
              <source src="./assets/0_ptb_02.mp4" type="video/mp4">
            </video>
          </div> <!-- Push The Button-->
          <div v-if="showInterDis || showInterDisClick" class="middle">
            <video height="725" width="408" autoplay muted loop preload="auto">
              <source src="./assets/00_Interdis_01.mp4" type="video/mp4">
            </video>
          </div> <!-- Interdisziplinär-->
          <div v-if="showFilmPost || showFilmPostClick" class="middle">
            <img src="../src/assets/Filmposter_01.png" alt="Das Ende vom Ende der Welt" height="725" width="507px">
          </div> <!-- Filmposter-->
          <div v-if="showJourFixe || showJourFixeClick" class="middle">
            <video autoplay muted loop>
              <source src="./assets/Jour_Fixe_Web_04.mp4" type="video/mp4">
            </video>
          </div> <!-- Jour Fixe-->
          <div v-if="showKurt || showKurtClick" class="middle">
            <video height="750" width="487" autoplay muted loop>
              <source src="./assets/Kurt.mp4" type="video/mp4">
            </video>
          </div> <!-- Kurt-->
          <div v-if="showDTF || showDTFClick" class="middle">
            <video height="750" width="542" autoplay muted loop>
              <source src="./assets/DTF_01.mp4" type="video/mp4">
            </video>
          </div> <!-- DTF-->
          <div v-if="showRG23 || showRG23Click" class="middle">
            <video height="725px" width="408px" autoplay muted loop>
              <source src="./assets/0_RG23.mp4" type="video/mp4">
            </video>
          </div> <!-- Rg23-->
          <div v-if="showContainer_01 || showContainerClick_01" class="middle">
            <video autoplay muted loop>
              <source src="./assets/0_container_01.mp4" type="video/mp4">
            </video>
          </div> <!-- Container 1-->
          <div v-if="showContainer_02 || showContainerClick_02" class="middle">
            <video height="750" width="408" autoplay muted loop>
              <source src="./assets/0_container2_02.mp4" type="video/mp4">
            </video>
          </div> <!-- Container 2-->
          <div v-if="showTruaka || showTruakaClick" class="middle">
            <video autoplay muted loop>
              <source src="./assets/0_traka.mp4" type="video/mp4">
            </video>
          </div> <!-- Truaka-->
          <div v-if="showRG24 || showRG24Click" class="middle">
            <video autoplay muted loop>
              <source src="./assets/RG24.mp4" type="video/mp4">
            </video>
          </div> <!-- Rg24-->
          <div v-if="showMAD || showMADClick" class="middle">
            <video autoplay muted loop>
              <source src="./assets/mad_color-logo-flip.mp4" type="video/mp4">
            </video>
          </div> <!-- Mad-->
          <div v-if="showSchwarz || showSchwarzClick" class="middle">
            <img src="../src/assets/schwarzbrenne.png" alt="vue logo" height="725px" width="352px">
          </div> <!-- schwarz-->
          <div v-if="showWayToo || showWayTooClick" class="middle">
            <video height="725" width="725" autoplay muted loop>
              <source src="./assets/waytoomuch_03.mp4" type="video/mp4">
            </video>
          </div> <!-- waytoomuch-->
          <div style="position: absolute;margin: 30px;grid-row-start: 1; grid-column-start: 1; margin-right: 120px">
            <h1>
              C13 Cloud → Art Direction & Motion →
              <button v-if="showAll" @click="showAll = false"  class="buttonProjekt buttonProjektShow2" >Show All</button>
              <button v-if="!showAll" @click="showAll = true"  class="buttonProjekt buttonProjektShow2">Show Less</button>
            </h1>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Mit einem Glücksspielautomaten im Kulturkiosk zogen wir den Leuten das Geld aus der Tasche. Unsere audiovisuelle Installation:
              <button class="buttonProjekt buttonProjekt1">Push the Button</button>,
              mit welcher wir bei der Sammelausstellung: <i>Belohnungszentrum</i> der <i>Klasse Cluss</i> partizpierten,
              umfasst einen eigenständig gebauten, programmierten und animierten Glücksspielautomaten mit einem Hauptgewinn in Form einer selbstgegossen Pokal-Kerze mit Verpackung und einem kleinen Sticker als Trostpreis.
              <button class="buttonProjekt buttonProjekt3">@Lilian Hutchinson</button>
              <button class="buttonProjekt buttonProjekt3">@Nick Stäbler</button>
              <button class="buttonProjekt buttonProjekt3">@Tim Fritzsche</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Cluss</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#After Effects</button>
              <button class="buttonProjekt buttonProjekt3">#Silikon</button>
              <button class="buttonProjekt buttonProjekt3">#Styropor</button>
              <button class="buttonProjekt buttonProjekt3">#Sticker</button>
              <button class="buttonProjekt buttonProjekt3">#Packaging</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Installation</button>
              <button class="buttonProjekt buttonProjekt3">#Audiovisual</button>
            </p> <!-- Push the Button -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Push the Button</button>
              <button class="buttonProjekt buttonProjekt3">@Lilian Hutchinson</button>
              <button class="buttonProjekt buttonProjekt3">@Nick Stäbler</button>
              <button class="buttonProjekt buttonProjekt3">@Tim Fritzsche</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Cluss</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#After Effects</button>
              <button class="buttonProjekt buttonProjekt3">#Silikon</button>
              <button class="buttonProjekt buttonProjekt3">#Styropor</button>
              <button class="buttonProjekt buttonProjekt3">#Sticker</button>
              <button class="buttonProjekt buttonProjekt3">#Packaging</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Installation</button>
              <button class="buttonProjekt buttonProjekt3">#Audiovisual</button>
            </p> <!-- Less Push the Button -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Neben Halunkereien, zeigt sich mein Informatik-, Kunst- und Design-Hintergrund in illustrierten und animierten Plakatentwürfen.
            </p>
            <p v-if="showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Plakate & Veranstaltungen:
            </p>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Für die <button class="buttonProjekt buttonProjekt1">Interdisziplinäre Woche – Interdisciplnary Week</button>,
              wurden wir dafür ausgewählt interdisziplinäre Vorträge und Workshops zu bewerben, mit dem Schwerpunkt Social Media. Entstanden sind hierfür ein animiertes Poster, Banner und Social Media Formate.
              <button class="buttonProjekt buttonProjekt3">@Elisabeth Spengler Castillo</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Adobe Cloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Social Media</button>
              <button class="buttonProjekt buttonProjekt3">#Generativ Design</button>
            </p> <!-- Interdisziplinär -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Interdisziplinäre Woche – Interdisciplnary Week</button>
              <button class="buttonProjekt buttonProjekt3">@Elisabeth Spengler Castillo</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Adobe Cloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Social Media</button>
              <button class="buttonProjekt buttonProjekt3">#Generativ Design</button>
            </p> <!-- Less Interdisziplinär -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Das Ende vom Ende der Welt (Bild)</button>,
              war ein Filmposter-Projekt, welches als Resultat einer Kooperation zwischen der Filmakademie Wien und der ABK Stuttgart enstand. (not in use)
              <button class="buttonProjekt buttonProjekt3">@Klasse Panholzer</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
            </p> <!-- Filmposter-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Das Ende vom Ende der Welt (Bild)</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Panholzer</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
            </p> <!-- Less Filmposter-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Jour Fixe – Practices of Care</button>,
              ist eine annuale Vortragsreihe an der Akademie, welche Themen wie Architektur, Stadtplanung und Nachhaltigkeit diskutiert. Neben einem Siebdruck-Entwurf auf Kraft Paper, entstand für den Pitch ein animiertes Poster und ein Flyer, welche die Veranstaltung bewerben sollte. (not in use)
              <button class="buttonProjekt buttonProjekt3">@Markus Bader</button>
              <button class="buttonProjekt buttonProjekt3">@Blanca Will</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt3">#Blender</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#Illustrator</button>
              <button class="buttonProjekt buttonProjekt3">#Silkscreen</button>
              <button class="buttonProjekt buttonProjekt3">#Motion Design</button>
              <button class="buttonProjekt buttonProjekt3">#3D</button>
            </p> <!-- Jour Fixe-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Jour Fixe – Practices of Care</button>
              <button class="buttonProjekt buttonProjekt3">@Markus Bader</button>
              <button class="buttonProjekt buttonProjekt3">@Blanca Will</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt3">#Blender</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#Illustrator</button>
              <button class="buttonProjekt buttonProjekt3">#Silkscreen</button>
              <button class="buttonProjekt buttonProjekt3">#Motion Design</button>
              <button class="buttonProjekt buttonProjekt3">#3D</button>
            </p> <!-- Less Jour Fixe-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Als einer der ausgewählten Poster, welche zur Feier für <button class="buttonProjekt buttonProjekt1">Kurt Weidemann 2022</button> im Stadtpalais aushingen, konnte sich dieses animierte Poster dazuzählen.
              <button class="buttonProjekt buttonProjekt3">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#PhotoshopAutomation</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>

            </p> <!-- Kurt-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Kurt Weidemann 2022</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Roberts</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#PhotoshopAutomation</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>

            </p> <!-- Less Kurt-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Durch meine Leidenschaft für Bewegbild und da Social Media Beiträge und Plakate oft zu klein sind, rutschte ich schnell in das Erstellen und Konzipieren von Live-Visuals auf Veranstaltungen und Partys.
            </p>
            <p v-if="showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Live Visuals:
            </p>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Down to F*ck</button>,
              war der erste Auftrag für ein Audioreaktives-Live-Visual, welches ich für die Ausstellung & Afterparty der Klasse Brenner konzipieren durfte.
              <button class="buttonProjekt buttonProjekt3">@Klasse Brenner</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>

            </p> <!-- DTF-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Down to F*ck</button>
              <button class="buttonProjekt buttonProjekt3">@Klasse Brenner</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>

            </p> <!-- Less DTF-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Auf Basis des Rundgang-Design 2023, durften wir die Visuals für die
              <button class="buttonProjekt buttonProjekt1">Rundgang Afterparty 2023</button> erstellen, mappen und live mixen.
              <button class="buttonProjekt buttonProjekt3">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt3">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt3">#Cavalry</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>

            </p> <!-- Rundgang 2023 -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Rundgang Afterparty 2023</button>
              <button class="buttonProjekt buttonProjekt3">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt3">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt3">#Cavalry</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>

            </p> <!-- Less Rundgang 2023 -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              Für die Container City(Neue Oper) wurde ich beauftragt jeweils 2 Veranstaltungen mit Live-Visuals zu bespielen. Zum einen
              <button class="buttonProjekt buttonProjekt1">Container City Afterparty</button> und
              <button class="buttonProjekt buttonProjekt1">lay me next to her bones Afterparty</button>.
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>

            </p> <!-- Container City Festival Afterparty-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Container City Afterparty</button>
              <button class="buttonProjekt buttonProjekt1">lay me next to her bones Afterparty</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>

            </p> <!-- Less Container City Festival Afterparty-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">TRAKA Nikolausparty</button> einfach VRUM VRUM, Pabst Blue Ribbon Beer und Trucks. Mottoparty @AKA.
              <button class="buttonProjekt buttonProjekt3">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt3">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Blender</button>
              <button class="buttonProjekt buttonProjekt3">#AfterEffects</button>
              <button class="buttonProjekt buttonProjekt3">#KI</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>
            </p> <!-- Truaka -->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">TRAKA Nikolausparty</button>
              <button class="buttonProjekt buttonProjekt3">@ABK Licht Licht</button>
              <button class="buttonProjekt buttonProjekt3">#ResolumeArena</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">#Blender</button>
              <button class="buttonProjekt buttonProjekt3">#AfterEffects</button>
              <button class="buttonProjekt buttonProjekt3">#KI</button>
              <button class="buttonProjekt buttonProjekt3">#Projection Mapping</button>
              <button class="buttonProjekt buttonProjekt3">#Generative Design</button>
              <button class="buttonProjekt buttonProjekt3">#Audioreactive</button>
            </p> <!-- Less Truaka -->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Außerdem sind in der Pipeline:
            </p>
            <p v-if="showAll" style="font-size: 35px; margin-left: 0px">
              <br>
              Work in Progress:
            </p>

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Rundgangs Design 2024</button>
              Konzept, CI, Werbemittel(Social Media, Plakate, Flyer Sticker, Merch, Maskottchen). (Release Juni/Juli 2024)
              <button class="buttonProjekt buttonProjekt3">@Maryna Zevako</button>
              <button class="buttonProjekt buttonProjekt3">@Aleyna Kohl</button>
              <button class="buttonProjekt buttonProjekt3">@Majken Böckmann</button>
              <button class="buttonProjekt buttonProjekt3">#Blender</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Mascot</button>
              <button class="buttonProjekt buttonProjekt3">#Rundgang2024</button>
              <button class="buttonProjekt buttonProjekt3">#Cat</button>
            </p> <!-- RG24-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Rundgangs Design 2024</button>
              <button class="buttonProjekt buttonProjekt3">@Maryna Zevako</button>
              <button class="buttonProjekt buttonProjekt3">@Aleyna Kohl</button>
              <button class="buttonProjekt buttonProjekt3">@Majken Böckmann</button>
              <button class="buttonProjekt buttonProjekt3">#Blender</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Mascot</button>
              <button class="buttonProjekt buttonProjekt3">#Rundgang2024</button>
              <button class="buttonProjekt buttonProjekt3">#Cat</button>
            </p> <!-- Less RG24-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">MAD Lab CI</button>
              Branding, Logo, Flyer, Website, Merch. (Release März/April 2024)
              <button class="buttonProjekt buttonProjekt3">@Fraziska Brenner</button>
              <button class="buttonProjekt buttonProjekt3">@Miriam Häfele</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Wordpress</button>
            </p> <!-- MAD LAB-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">MAD Lab CI</button>
              <button class="buttonProjekt buttonProjekt3">@Fraziska Brenner</button>
              <button class="buttonProjekt buttonProjekt3">@Miriam Häfele</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#Wordpress</button>
            </p> <!-- Less MAD LAB-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Schwarzbrennen (Bild)</button>
              Publikation, Installation. (Release Juli 2024)
              <button class="buttonProjekt buttonProjekt3">@Nick Liebig</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Hefe</button>
              <button class="buttonProjekt buttonProjekt3">#Destillation</button>
              <button class="buttonProjekt buttonProjekt3">#Print</button>
            </p> <!-- Schwarz-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">Schwarzbrennen (Bild)</button>
              <button class="buttonProjekt buttonProjekt3">@Nick Liebig</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Hefe</button>
              <button class="buttonProjekt buttonProjekt3">#Destillation</button>
              <button class="buttonProjekt buttonProjekt3">#Print</button>
            </p> <!-- Less Schwarz-->

            <p v-if="!showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">WayTooMuch</button>
              Animation, Live Visuals, Plakat (Release Juni/Juli 2024)
              <button class="buttonProjekt buttonProjekt3">@Florian Siegert</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
            </p> <!-- WayMuch-->
            <p v-if="showAll" style="font-size: 35px; margin-left: 60px">
              <br>
              <button class="buttonProjekt buttonProjekt1">WayTooMuch</button>
              <button class="buttonProjekt buttonProjekt3">@Florian Siegert</button>
              <button class="buttonProjekt buttonProjekt3">#AdobeCloud</button>
              <button class="buttonProjekt buttonProjekt3">#Photoshop</button>
              <button class="buttonProjekt buttonProjekt3">#InDesign</button>
              <button class="buttonProjekt buttonProjekt3">#TouchDesigner</button>
            </p> <!-- Less WayMuch-->

            <p style="font-size: 35px; margin-left: 0px">
              <br>
              Skills, Lebenslauf & Kontakt:
              <br>
            </p>

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Programme:
              <button class="buttonProjekt buttonProjekt3">● Adobe Cloud (PS, ID, AI, XD, PR)</button>
              <button class="buttonProjekt buttonProjekt3">● Blender</button>
              <button class="buttonProjekt buttonProjekt3">● TouchDesigner</button>
              <button class="buttonProjekt buttonProjekt3">● Resolume Arena</button>
              <button class="buttonProjekt buttonProjekt3">● Figma</button>
              <button class="buttonProjekt buttonProjekt3">● HTML</button>
              <button class="buttonProjekt buttonProjekt3">● CSS</button>
              <button class="buttonProjekt buttonProjekt3">● Vue.JS</button>
              <button class="buttonProjekt buttonProjekt3">● Python Scripting</button>
              <button class="buttonProjekt buttonProjekt3">● Processing/p5.js</button>
            </p> <!-- Programme-->

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Skills:
              <button class="buttonProjekt buttonProjekt3">● Print Medien</button>
              <button class="buttonProjekt buttonProjekt3">● Digitale Medien</button>
              <button class="buttonProjekt buttonProjekt3">● Video Medien</button>
              <button class="buttonProjekt buttonProjekt3">● Schnelles lernen von Programmen</button>
              <button class="buttonProjekt buttonProjekt3">● Schnelles verstehen von tech. Abläufen</button>
              <button class="buttonProjekt buttonProjekt3">● Gefühl für Coding</button>
            </p> <!-- Skills-->

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Kurz Vita:
              <button class="buttonProjekt buttonProjekt3">● 2015-2018 Hauchler Studio - Ausbildung Grafik Design</button>
              <button class="buttonProjekt buttonProjekt3">● 2018-2019 Hochschule der Medien - Medieninformatik</button>
              <button class="buttonProjekt buttonProjekt3">● 2019-ongoing Staatl. Akademie der bildenden Künste Stuttgart - Kunst, Kommunikationsdesign</button>
            </p> <!-- Lebi-->

            <p style="font-size: 35px; margin-left: 60px">
              <br>
              Kontakt:
              <button class="buttonProjekt buttonProjekt3">@christianmiller.tox</button>
              <button class="buttonProjekt buttonProjekt3">christian.mueller2@abk-stuttgart.de</button></p> <!-- Kontakt-->
            <p><br></p>
          </div>
        </div>
      </section>
    </div>
  </main>
  <!--
  <i @mouseover="showModal = true" @mouseleave="showModal = false" @click="showModalClick = true" style="color: rgb(0,255,0);text-decoration: underline; text-decoration-style: dotted;">
  <i @mouseover="showModal = true" @mouseleave="showModal = false" @click="showModalClick = true">
  -->
</template>

<style scoped>
h1 {
  font-size: 54px;
}

ul{
  font-size: 30px;
  margin-left: 60px;
}

li::marker{
  color: #00FF00;
}

.overlay{
  flex-wrap: wrap;
  margin: initial;
  display: flex;
  align-items: center;
  justify-content: center;

}
.middle{
  grid-row-start: 1;
  grid-column-start: 1;
  z-index: 15;
  position: fixed;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 1280px;
  height: 720px;
  top: 50%;
  left: 50%;
  margin-top: -360px;
  margin-left: -640px;
}

.button {
  background-color: #04AA6D; /* Green */
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 35px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
  border-radius: 50%;
  font-size: 20px;
  padding: 15px 20px;
}



.button1 {
  background-color: #070707;
  color: #0f0;
  border: 2px solid #00FF00;
}

.button1:hover {
  background-color: #0f0;
  color: #070707;
}

.buttonProjekt {
  background-color: #04AA6D; /* Green */
  border: none;
  color: #070707;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
  border-radius: 100%;
  font-size: 30px;
  padding: 0px 15px;
}

.buttonProjekt1{
  background-color: #0f0;
  color: #070707;
  border: 2px solid #00FF00;
  border-radius: 35px;
  text-decoration: underline;
  text-decoration-style: dotted;
}

.buttonProjekt1:hover {
  background-color: #0f0;
  color: #070707;
  border-radius: 35px;
}

.buttonProjektShow{
  background-color: rgba(0,0,0,0);
  color: rgba(0,0,0,0);
  border-radius: 35px;
  font-size: 45px;
}

.buttonProjektShow2{
  background-color: #0f0;
  color: #070707;
  border-radius: 35px;
  font-size: 45px;
}

.buttonProjekt2{
  background-color: rgba(0,0,0,0);
  color: rgba(0,0,0,0);
  border: 2px solid rgba(0,0,0,0);
  border-radius: 35px;
}

.buttonProjekt2:hover {
  background-color: rgba(0,0,0,0);
  color: rgba(0,0,0,0);
  border-radius: 35px;
}

.buttonProjekt3{
  background-color: #070707;
  color: #0f0;
  border: 2px solid #00FF00;
  border-radius: 100px;
  font-size: 25px;
}

.buttonProjekt4{
  background-color: rgba(0,0,0,0);
  color: rgba(0,0,0,0);
  border: 2px solid rgba(0,0,0,0);
  border-radius: 100px;
  font-size: 25px;
}
</style>