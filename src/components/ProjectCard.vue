<template>
  <div style="height: 400px; width: 700px; display: inline-flex;">
    <div style="height: 400px; width: 350px;">
      <v-img :src="linkImage" width="350" height="400" cover />
    </div>

    
    <div style="color: white;height: 400px; width: 350px; padding: 20px;background-image: url('src/assets/background3.jpg');">
      <span class="font-custom">TITLE</span> <span style="padding-left: 5px;color: yellow">[ タイトル ]</span>
      <br>
      <div style="padding-top: 10px;">
        <text>{{ title }}</text>
      </div>
      
      <br>
      <span class="font-custom">DESCRIPTION</span> <span style="padding-left: 5px;color: yellow">[ 説明 ]</span>
      <br>
      <div style="padding-top: 10px;">
        <text class="justify-text" style="color: white">{{ description }}</text>
      </div>
      
      <br>
      <span class="font-custom">LINK</span> <span style="padding-left: 5px;color: yellow">[ リンク ]</span>
      <br>    
      <a :href="linkSite" target="_blank">Site</a>
    </div>
  </div>
</template>

<script>

export default {
  name: 'ProjectCard',
  props: {
    title: {
      type: String,
      default: "Interlinker"
    },
    description: {
      type: String,
      default: "Rede Social para cadastro de metas e objetivo com a possibilidade da conclusão de forma cooperativa com outros usuários."
    },
    linkSite: {
      type: String,
      default: "http://interlinker.com.br"
    },
    linkImage: {
      type: String,
      default: "https://images.pexels.com/photos/52500/horse-herd-fog-nature-52500.jpeg?cs=srgb&dl=pexels-pixabay-52500.jpg&fm=jpg"
    },
  }
}
</script>
