<template>
    <v-divider color="yellow" class="border-opacity-100"></v-divider>
    <div class="replicated-text">
        <text class="moving-text" style="color: yellow;font-size: 30px;">{{ word }}</text>
    </div>
    <v-divider color="yellow" class="border-opacity-100"></v-divider>
</template>
  
<script>
export default {
    name: "TextDivider",
    props: {
        word: {
            type: String,
        },
    },
};
</script>
  
<style>
.replicated-text {
    display: flex;
    width: 100vw;
}

.moving-text {
    white-space: nowrap;
    word-break: break-all;
    animation: scrollTextStart 15s infinite linear;
}

@keyframes scrollTextStart {
    from {
        transform: translateX(0vw);
    }

    to {
        transform: translateX(100vw);
    }
}

@keyframes scrollTextEnd {
    from {
        transform: translateX(100vw);
    }

    to {
        transform: translateX(0vw);
    }
}
</style>
  