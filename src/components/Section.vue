<template>
  <v-col cols="12">
    <v-row style="text-align: center;justify-content: center;">
      <h1 class="font-custom" style="font-size: 50px;color: white;">Victor Augusto Barros</h1>
    </v-row>

    <v-row style="text-align: center;justify-content: center;">
      <h3 class="font-custom-goblin" style="font-size: 50px;color: yellow;">Back-end Developer</h3>
    </v-row>

    <v-row style="padding-top:20px">
      <TextDivider word="バックエンドエンジニア" />
    </v-row>

    <v-row style="justify-content: center;">
      <v-spacer></v-spacer>
      <v-col cols="3">
        <v-row style="padding-top: 100px;">
          <div>
            <p class="font-custom justify-text" style="color: white;">
              SOU DESENVOLVEDOR <span style="color:yellow">BACK-END</span> FOCADO EM SEMPRE CONHECER NOVAS TECNOLOGIAS
              INTERESSANTE E APLICAR ELAS EM
              DIVERSOS
              PROJETOS <span style="color:yellow">PESSOAIS</span> E <span style="color:yellow">PROFISSIONAIS</span>.
            </p>
            <br>
            <p class="font-custom justify-text" style="color: white;">
              TENHO <span style="color:yellow">+4 ANOS</span> DE EXPERIÊNCIA COM TECNOLOGIA EM PROJETOS DE DIFERENTES
              ESCALAS, TAIS COMO SIMPLES PROCESSOS
              PARA RESOLVER TAREFAS ESPECÍFICAS A ATÉ PROCESSOS DE GRANDE ESCALA ONDE É NECESSÁRIO TER UMA MAIOR
              <span style="color:yellow">CONFIABILIDADE</span> E <span style="color:yellow">ESCALABILIDADE</span>.
            </p>
          </div>
        </v-row>

      </v-col>
      
      <v-spacer></v-spacer>

      <v-col cols="5" style="padding-top: 100px;">

        <v-carousel style="height: 400px;width: 700px;">
          <v-carousel-item>
            <ProjectCard />
          </v-carousel-item>

          <v-carousel-item>
            <ProjectCard />
          </v-carousel-item>

          <v-carousel-item>
            <ProjectCard />
          </v-carousel-item>
        </v-carousel>

      </v-col>

      <v-spacer></v-spacer>
    </v-row>
  </v-col>
</template>

<script>
import TextDivider from "@/components/TextDivider.vue"
import ProjectCard from "@/components/ProjectCard.vue"

export default {
  name: 'FirstSection',
  components: {
    TextDivider,
    ProjectCard
  }
}
</script>

<style></style>